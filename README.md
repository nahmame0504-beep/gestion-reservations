# TP 3 : Gestion des Relations et Cascades avec JPA / Hibernate

## Description du Projet
Ce projet est une application Java SE mettant en œuvre la gestion des relations avancées avec **JPA (Java Persistence API)** et **Hibernate**. L'objectif principal est de simuler un système de gestion de réservations de salles de réunion tout en expérimentant la persistance en cascade, la suppression orpheline (`orphanRemoval`) et le mapping des relations bidirectionnelles.

---

## Fonctionnalités & Concepts Démonstrés
- **Relation Bidirectionnelle `@OneToMany` / `@ManyToOne`** : Association entre `Utilisateur` <-> `Reservation` et `Salle` <-> `Reservation`.
- **Cascade & Suppression Orpheline** : Persistance en cascade (`CascadeType.ALL`) et suppression automatique des réservations détachées (`orphanRemoval = true`).
- **Relation Bidirectionnelle `@ManyToMany`** : Association entre `Salle` <-> `Equipement` gérée avec une table de jonction (`salle_equipement`).
- **Moteur de Persistance** : Utilisation de la base de données en mémoire **H2** gérée via `persistence.xml`.

---

## Structure du Projet

```text
gestion-reservations/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           ├── App.java
│   │   │           └── model/
│   │   │               ├── Equipement.java
│   │   │               ├── Reservation.java
│   │   │               ├── Salle.java
│   │   │               └── Utilisateur.java
│   │   └── resources/
│   │       └── META-INF/
│   │           └── persistence.xml
└── pom.xml
```


https://github.com/user-attachments/assets/019004b4-6daf-4c52-a341-6dddb1fea0ad


