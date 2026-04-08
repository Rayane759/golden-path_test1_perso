# Golden Path

Bienvenue sur le **Golden Path** — le guide de référence pour créer un nouveau projet conforme aux standards de la plateforme.

---

## Objectif

Ce guide vous accompagne pas à pas dans la création d'un projet, de l'initialisation du dépôt jusqu'au premier déploiement sur Kubernetes.  
À chaque étape, vous trouverez les actions à réaliser, des fichiers d'exemple et des liens vers la documentation technique des équipes.

!!! info "Ce que ce guide n'est pas"
    Le Golden Path ne génère pas de code à votre place. Il vous guide, vous fournit des exemples et centralise les ressources dont vous avez besoin.

---

## Cas d'usage couverts

Ce guide s'applique aux projets répondant aux critères suivants :

| Composant     | Technologie         |
|---------------|---------------------|
| Backend       | Java (Spring Boot)  |
| Frontend      | React               |
| Base de données | PostgreSQL        |
| Déploiement   | Kubernetes          |

!!! warning "Votre projet ne correspond pas ?"
    Si votre stack diffère (VM, autre langage, autre BDD), contactez l'équipe platform avant de commencer : `LIEN_CONTACT_EQUIPE_PLATFORM`

---

## Les 8 étapes du guide

```
Phase 1 · Dépôt GitLab          Créer et structurer votre dépôt
Phase 2 · Backend Java           Générer et configurer le projet Spring Boot
Phase 3 · Frontend React         Initialiser le projet React (si applicable)
Phase 4 · Containerisation       Créer les Dockerfiles
Phase 5 · Pipeline CI            Configurer GitLab CI
Phase 6 · Secrets & Sécurité     Configurer Vault et GitLeaks
Phase 7 · Déploiement K8s        Créer le chart Helm et ouvrir la MR GitOps
Phase 8 · Documentation          Compléter le README et le Runbook
```

---

## Avant de commencer

Vérifiez que vous disposez des accès suivants avant de démarrer :

- [ ] Accès à GitLab : `LIEN_GITLAB`
- [ ] Accès à Vault : `LIEN_VAULT`
- [ ] Accès au repo GitOps : `LIEN_REPO_GITOPS`
- [ ] Accès au registry Docker : `LIEN_REGISTRY`

!!! tip "Accès manquants ?"
    Suivez la procédure de demande d'accès : `LIEN_DEMANDE_ACCES`

---

**Prêt ?** Commencez par la [Phase 1 — Dépôt GitLab](guide/1-depot.md).