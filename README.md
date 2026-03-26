# Projet Simulation Numérique - Factorisation de Matrices de Rang Faible

## 📋 Informations Générales

**Établissement** : ENSEEIHT (École Nationale Supérieure d'Électrotechnique, d'Électronique, d'Informatique, d'Hydraulique et des Télécommunications)

**Année Académique** : 2024-2025

**Groupe** : B1

**Étudiant(e)** : Nicolas Bailliet

**Collaborateur** : Antoine Pichon (projet effectué en binôme)

**Contact** : xavier.vasseur@gmail.com

## 🎯 Objectif du Projet

Ce projet vise à analyser et implémenter des algorithmes de factorisation structurée de matrices de grande taille. L'accent est mis sur les méthodes suivantes :

- **Interpolative Decomposition (ID)**
- **CUR-ID Decomposition**
- **Non-negative Matrix Factorization (NMF)**

L'objectif est d'approcher une matrice $A$ par un produit de matrices de rang faible, en comparant différents algorithmes selon plusieurs critères :
- ⏱️ Temps de calcul
- 🔢 Complexité opératoire
- 🎯 Précision numérique

## 📚 Cours Liés

Ce projet s'appuie sur les contenus des cours suivants :
- Calcul Scientifique
- Algèbre Linéaire pour le Data Mining
- Optimisation II

## 🛠️ Stack Technique

### Langages et Frameworks
- **Langage** : Python 3
- **Calcul numérique** : NumPy
- **Algèbre linéaire** : SciPy
- **Traitement d'images** : PIL (Pillow)
- **Visualisation** : Matplotlib

### Prérequis
- Connaissance basique de Python
- Maîtrise élémentaire de NumPy
- Familiarité avec l'algèbre linéaire

## 📅 Calendrier des Séances

| Date | Type | Groupe | Horaire | Lieu |
|------|------|--------|---------|------|
| 5/3/25 | C/TD | B1-B2 | 08:00-10:00 | A301 |
| 12/3/25 | TP | B1 | 10:00-12:00 | C304 |
| 12/3/25 | TP | B1 | 16:00-18:00 | C202 |
| 19/3/25 | TP | B2 | 16:00-18:00 | C304 |
| 26/3/25 | TP | B2 | 16:00-18:00 | As204 |

## 📝 Structure du Projet

### Composants Principaux

Le projet est organisé sous forme d'un **Jupyter Notebook** contenant :

1. **Introduction** - Contexte et concepts fondamentaux
2. **Partie A** - Implémentation basique des algorithmes de factorisation
3. **Partie B** - Applications sur images
4. **Partie C** - Questions de compréhension sur les algorithmes
5. **Partie D** - Implémentation d'algorithmes populaires pour comparaison

### Données

Le projet utilise les fichiers suivants :
- `PSN_2024_2025.ipynb` - Notebook principal
- Images au format `.jpg` pour les applications pratiques :
  - `Armand_Duplantis_Profile.jpg`
  - `BMX.jpg`
  - `Gabriel_Medina.jpg`
  - `Gym_Japanese_Team.jpg`
  - `Leon_Marchand.jpg`
  - `Remco_Evenepoel.jpg`
  - `Sprint.jpg`
  - `Triathlon_Start.jpg`
  - `Yamada_Siklosi.jpg`

### Documentation

Dossier `docs/` contenant :
- `Projet simu numérique.pdf` - Description du projet
- `doc_simu.pdf` - Documentation technique
- `nmf_kdd11.pdf` - Référence sur la factorisation non-négative

## 🚀 Comment Utiliser

### Lancer le Notebook

```bash
jupyter notebook PSN_2024_2025.ipynb
```

### Structure de Travail

Vous devez :
1. ✅ Insérer tous vos commentaires et codes **uniquement** dans le Notebook
2. ✅ Créer autant de cellules que nécessaire (texte et code)
3. ✅ Travailler avec les images fournies
4. ✅ Rendre le Notebook complété avec tous les résultats

## 📊 Concepts Clés

### Factorisation de Rang Faible

Approcher une matrice $A$ par :

$$A \approx U V^T$$

où $U \in \mathbb{R}^{m \times r}$ et $V \in \mathbb{R}^{n \times r}$ avec $r << \min(m,n)$.

### Décomposition Interpolative (ID)

Sélectionne des colonnes (ou lignes) de la matrice originale pour former une base de faible rang.

### CUR-ID

Variante combinant les approches CUR (Column-row) et ID pour une approximation optimale.

### Factorisation Non-Négative (NMF)

Factorisation contrainte où tous les éléments de $U$ et $V$ sont non-négatifs, utile pour certaines applications d'images.

## 📌 Détermination Adaptative du Rang

Le projet fournit une fonction pour estimer le rang d'une matrice :

Pour une matrice $A$, on cherche un réel orthogonal $Q$ tel que :

$$\|A - Q Q^T A \|_F \le \epsilon \|A \|_F$$

où $\|\cdot\|_F$ est la norme de Frobenius et $\epsilon$ est une tolérance définie par l'utilisateur.

## ⚙️ Volume de Travail

Le volume de travail demandé est **raisonnable** et progressif, avec un guidage à chaque étape.

## 📬 Contacts et Support

Pour toute question concernant ce projet :
- **Responsable** : Xavier Vasseur
- **Email** : xavier.vasseur@gmail.com
- **Objet recommandé** : [PSN 2025]

## 📄 Évaluation

✅ L'évaluation se base **uniquement** sur le Notebook rendu.

### Date Limite de Rendu
**11 avril 2025 à midi**

## 📖 Références Principales

- Algèbre linéaire numérique (SVD, QR, etc.)
- Algorithmes de décomposition de matrices de rang faible
- Optimisation et approximation matricielle
- Factorisation non-négative de matrices

## 📁 Structure du Répertoire

```
low-rank-matrix-factorization/
├── PSN_2024_2025.ipynb          # Notebook principal
├── README.md                     # Ce fichier
├── docs/
│   ├── Projet simu numérique.pdf
│   ├── doc_simu.pdf
│   └── nmf_kdd11.pdf
├── Images/
│   ├── Armand_Duplantis_Profile.jpg
│   ├── BMX.jpg
│   ├── Gabriel_Medina.jpg
│   ├── Gym_Japanese_Team.jpg
│   ├── Leon_Marchand.jpg
│   ├── Remco_Evenepoel.jpg
│   ├── Sprint.jpg
│   ├── Triathlon_Start.jpg
│   └── Yamada_Siklosi.jpg
└── .git/                         # Version control
```

---

*Projet de Simulation Numérique - ENSEEIHT 2024-2025*
