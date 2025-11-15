# Exercice 1 : Gestion d’un étudiant avec tableau de notes
### Objectif

Créer une classe Etudiant avec un ID auto-incrémenté.

Gérer un tableau dynamique de notes (agrandissement automatique).

Calculer la moyenne des notes.

Afficher les informations de l’étudiant de manière lisible.

----

### Points clés

Attributs :

id

nom

prenom

notes[]

nbNotes

Constructeur :

Initialise id, nom, prenom et crée un tableau notes de taille 5.

Méthodes :

ajouterNote(double) → ajoute une note et agrandit le tableau si nécessaire.

calculerMoyenne() → retourne 0 si pas de notes, sinon calcule la moyenne.

afficherNotes() → affiche toutes les notes de l’étudiant.

toString() → affiche l’étudiant avec son ID et sa moyenne formatée.

---

### Résultat attendu

<img width="1113" height="238" alt="TP41" src="https://github.com/user-attachments/assets/3f4b701c-45fb-49c9-b2d5-385e6a306501" />

---

# Exercice 2 : Association Étudiant ↔ Filière (avec tableaux)
## Objectif

Mettre en œuvre deux classes liées par une association un-à-plusieurs.

Une filière regroupe plusieurs étudiants.

Gérer un tableau dynamique pour les étudiants (agrandissement automatique).

Permettre l’affichage des informations des étudiants et des filières.

---

## Points clés

Classe Étudiant :

Attributs : id, nom, prenom, filiere.

Méthodes : setFiliere(), toString().

Classe Filiere :

Attributs : id, nom, etudiants[], nbEtudiants.

Méthodes : ajouterEtudiant(), afficherEtudiants(), toString().

Agrandissement automatique du tableau si nécessaire.

Association :

Filiere contient plusieurs Étudiant.

Chaque Étudiant connaît sa Filiere.

## Résultat attendu

<img width="1116" height="497" alt="TP42" src="https://github.com/user-attachments/assets/460b8347-19a5-4d71-9262-646181049731" />

---

# Exercice 3 : Gestion des articles
## Objectif

Développer deux classes métier Categorie et Article avec auto-incrémentation des IDs.

Pratiquer l’utilisation de tableaux et boucles pour gérer et afficher des collections d’objets.

Afficher les articles classés par catégorie sans utiliser de collections avancées.

---

## Points clés
Classe Categorie

Attributs :

id (auto-incrémenté)

libelle (ex. "Ordinateur Portable")

code (ex. "O PR")

Méthodes :

Constructeur Categorie(String libelle, String code)

Getters et setters

toString() lisible

Classe Article

Attributs :

id (auto-incrémenté)

code (ex. 14, 4, 74, 785)

designation (ex. "DELL INSPIRON")

categorie (objet Categorie)

Méthodes :

Constructeur Article(int code, String designation, Categorie categorie)

Getters et setters

toString() exactement au format : id code designation

Classe de test TestApp

Créer un tableau Categorie[] avec deux catégories.

Créer un tableau Article[] avec quatre articles répartis sur les catégories.

Boucler pour afficher chaque catégorie et les articles qui lui appartiennent.

---

## Résultat attendu

<img width="1117" height="346" alt="TP43" src="https://github.com/user-attachments/assets/8d5fd054-cad3-4faf-924a-5a716ad8cdaa" />

---

# Exercice 4 : Gestion d’Auteurs, Livres et Bibliothèques
## Objectif

Créer des classes Java avec id auto-incrémenté (Auteur, Livre, Bibliotheque).

Gérer les associations :

un-à-plusieurs : Auteur → Livres

plusieurs-à-plusieurs : Bibliothèque ↔ Livres

Instancier des objets et afficher leurs relations.

---

## Points clés
Classe Auteur

Attributs : id, nom, livres (liste des livres écrits)

Méthodes :

Constructeur Auteur(String nom)

ajouterLivre(Livre livre) pour l’association bidirectionnelle

toString() indiquant le nombre de livres

Classe Livre

Attributs : id, titre, auteur

Méthodes :

Constructeur Livre(String titre, Auteur auteur) (liaison automatique à l’auteur)

toString() affichant id, titre et auteur

Classe Bibliotheque

Attributs : id, nom, collection (Set pour éviter doublons)

Méthodes :

ajouterLivre(Livre livre)

toString() indiquant la taille de la collection

Programme de test (Main.java)

Création de deux auteurs et trois livres

Création de deux bibliothèques et ajout des livres correspondants

Affichage :

Les auteurs et leurs livres

Les bibliothèques et les livres qu’elles contiennent

---

## Résultat attendu

<img width="1116" height="400" alt="TP44" src="https://github.com/user-attachments/assets/37aa7616-e1fb-4540-a4a4-df00bfaaf51d" />



