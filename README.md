# Introduction au versioning avec GIT  <!-- omit in toc -->

## Sommaire <!-- omit in toc -->

- [Le versionning ?](#le-versionning-)
  - [VCS](#vcs)
- [Installation](#installation)
- [Repository](#repository)
- [Les commits](#les-commits)
  - [A quoi ça sert](#a-quoi-ça-sert)
  - [Quand en faire](#quand-en-faire)
  - [Qu'est-ce que ça contient](#quest-ce-que-ça-contient)
  - [Message de commit](#message-de-commit)
- [Les branches](#les-branches)
  - [A quoi servent les branches](#a-quoi-servent-les-branches)
  - [Quand faire des branches](#quand-faire-des-branches)
  - [Qu'est ce que ça contient](#quest-ce-que-ça-contient-1)
  - [Bien nommer les branches](#bien-nommer-les-branches)
- [Organiser son modèle de branches](#organiser-son-modèle-de-branches)
  - [Gitflow](#gitflow)
  - [Trunk-based](#trunk-based)
- [Les pull requests](#les-pull-requests)
- [Les issues](#les-issues)
- [Les flags et les releases](#les-flags-et-les-releases)
- [Automatiser pour de la CI/CD](#automatiser-pour-de-la-cicd)
- [Les outils](#les-outils)
  - [Intégrés (exemple avec vs code)](#intégrés-exemple-avec-vs-code)
  - [Externes](#externes)

## Le versionning ?

### VCS

- Version Control Systems
- outil permettant de suivre et gérer les changements de code sur une application
- permet à plusieurs développeur.ses de travailler sur le même projet en limitant les conflits
- historique :
  - 1970 : Source Code Control System, traçage basique des versions
  - début 1980 : Revision Control System, rajoute les branches et les merge
  - fin 1980 : Concurent Version System, développement concurrent
  - 2000 : Apache Subversion (SVN), améliore les performances de CVS
  - 2005 : après un conflit de license entre la fondation Linux et le versionning utilisé (BitKeeper), Linus Torvalds met au point Git

## Installation

- sur WSL / linux :

```bash
apt-get install git
```

- sur mac :

```bash
brew install git
```

## Repository

- espace de stockage permettant de sauvegarder le code de son application, l'historique de ses changements, les branches, ...
- repository distant (ou remote) : une version sauvegardée sur le cloud (de github, gitlab, bitbucket, ...)
- repository local : une version sauvegardée sur un ordinateur

## Les commits

### A quoi ça sert

- snapshot du code à un moment précis
- 

### Quand en faire

- le plus souvent possible
  - pour pouvoir rollback avec précision en cas d'erreur
  - pour marquer l'étape du développement d'une fonctionnalité
  - pour mieux découper et organiser son travail

### Qu'est-ce que ça contient

- nom de l'auteur.ice du code
- timestamp
- message de commit
- code modifié :
  - ajout de nouveaux fichiers
  - suppression de fichiers
  - modification des contenus des fichiers

### Message de commit

- bien nommer permet :
  - de faciliter le travail à plusieurs
    - les autres comprennent plus facilement les évolutions du code
  - de faciliter la code review
    - comprendre l'objectif d'une évolution
  - améliorer l'historique
    - l'enchainement des commits permet de tracer les évolutions
  - automatiser
    - certains outils se basent sur les titres des commits pour
      - déployer une mise à jour
      - modifier la doc
      - envoyer des notifications (mail, slack, ...)
- utiliser une convention, comme <https://www.conventionalcommits.org/en/v1.0.0/>
  - `[type] scope : description`
    - `type` : feature, fix, test, documentation, ...
    - `scope` : numéro de ticket, fonctionnalité en train d'être développée, ...
    - `description`: court résumé de l'évolution

## Les branches

### A quoi servent les branches

### Quand faire des branches

### Qu'est ce que ça contient

### Bien nommer les branches

## Organiser son modèle de branches

### Gitflow

### Trunk-based

## Les pull requests

## Les issues

## Les flags et les releases

## Automatiser pour de la CI/CD

github actions

## Les outils

### Intégrés (exemple avec vs code)

### Externes

Exemple avec gitkraken et github desktop
