# Phase 1 · Dépôt GitLab

## Objectif de cette phase

À la fin de cette phase, vous disposez d'un dépôt GitLab structuré, avec les conventions de base en place.

---

## Étape 1.1 — Créer le dépôt GitLab

!!! abstract "Action"
    Créer manuellement un nouveau dépôt GitLab dans le namespace de votre équipe.

**Règles de nommage du dépôt :**

- Minuscules uniquement
- Mots séparés par des tirets : `my-service`
- Pas de préfixe d'équipe dans le nom (le namespace GitLab fait office de préfixe)

→ Documentation complète sur les conventions de nommage : `LIEN_CONVENTIONS_NOMMAGE`  
→ Créer un dépôt sur GitLab : `LIEN_DOC_GITLAB_CREATION_REPO`

!!! tip
    Cochez **"Initialize repository with a README"** lors de la création pour ne pas démarrer avec un repo vide.

---

## Étape 1.2 — Appliquer la structure de dépôt standard

!!! abstract "Action"
    Créer l'arborescence de dossiers suivante à la racine de votre repo.

```
mon-service/
├── backend/              ← code source Java
├── frontend/             ← code source React (si applicable)
├── helm/                 ← charts Helm pour le déploiement K8s
├── docs/
│   └── adr/              ← Architecture Decision Records
├── .gitlab-ci.yml        ← pipeline CI (créé en Phase 5)
├── .editorconfig
├── .gitignore
├── README.md
└── RUNBOOK.md
```

**Fichiers de configuration à créer :**

=== ".editorconfig"

    Copiez le fichier standard et adaptez si nécessaire :

    → Exemple `.editorconfig` : `EXEMPLE_EDITORCONFIG`

=== ".gitignore"

    Utilisez le `.gitignore` standard pour un projet Java + React :

    → Exemple `.gitignore` : `EXEMPLE_GITIGNORE`

---

## Étape 1.3 — Configurer les conventions de commit

!!! abstract "Action"
    Ajouter un fichier `.gitmessage` à la racine du repo et le configurer localement.

→ Conventions de commit adoptées par l'équipe : `LIEN_CONVENTIONS_COMMIT`  
→ Exemple de `.gitmessage` : `EXEMPLE_GITMESSAGE`

Une fois le fichier créé, exécuter la commande suivante **dans votre repo local** :

```bash
git config commit.template .gitmessage
```

!!! warning
    Cette commande est à exécuter par chaque développeur après avoir cloné le repo. Elle ne se propage pas automatiquement.

---

## Checklist de fin de phase

Avant de passer à la phase suivante, vérifiez les points suivants :

- [ ] Le dépôt GitLab est créé dans le bon namespace
- [ ] La structure de dossiers est en place
- [ ] `.editorconfig` et `.gitignore` sont committés
- [ ] Les conventions de commit sont configurées localement

---

**Phase suivante ->** [Phase 2 · Backend Java](2-backend.md)