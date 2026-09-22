# 📊 Analyse Économétrique : Déterminants de la Durée en Emploi en France

> **Projet académique de Data Analysis / Économétrie (L3 Économie-Gestion)** — Étude empirique des trajectoires professionnelles de jeunes actifs à partir de l'enquête *Génération 98* du CEREQ.

---

## 🚀 Contexte et Objectifs
Comprendre la dynamique du marché du travail et la stabilité professionnelle des jeunes actifs est un enjeu clé en analyse de données socio-économiques. Ce projet vise à identifier et quantifier les déterminants individuels et structurels qui influencent la **durée en emploi (en mois)** de sortants de formation initiale.

L'étude combine rigueur statistique, nettoyage de données et modélisation économétrique sous **Stata**.

---

## 🛠️ Stack Technique
* **Langage & Outils :** Stata
* **Méthodologies statistiques :**
  * Statistiques descriptives univariées et bivariées (distributions, tests de normalité, coefficients de corrélation, diagrammes).
  * Modélisation par les **Moindres Carrés Ordinaires (MCO)** et introduction de formes quadratiques.
  * Tests de validation et de robustesse : **Test de Fisher** (signifiance globale), **Test de Student** (signifiance individuelle), et détection d'hétéroscédasticité (**Goldfeld-Quandt, Gleisjer, Breusch-Pagan**).

---

## 📂 Structure du Projet et Traitement des Données
1. **Nettoyage et Préparation des Données (`Data Cleaning`) :**
   * Gestion des valeurs manquantes et suppression des valeurs aberrantes (ex. traitement des extrêmes sur le salaire horaire et l'âge).
   * Regroupement des modalités catégorielles à faible effectif (secteurs d'activité, niveaux de diplôme, tranches de taille d'entreprise) pour garantir la significativité statistique.
2. **Exploration Univariée & Bivariée :**
   * Analyse de la distribution de la variable expliquée (`duree`) et des variables explicatives (âge, salaire, sexe, diplôme, taille d'entreprise, nombre d'entreprises antérieures).
   * Mise en évidence de relations non-linéaires (notamment l'effet quadratique du salaire sur la durée d'emploi).
3. **Modélisation MCO & Résultats :**
   * Estimation d'un modèle linéaire multiple expliquant ~42% de la variance de la durée en emploi ($R^2 = 0.4172$).
   * **Principaux enseignements :** 
     * Impact positif de l'âge et du salaire (avec des rendements croissants puis décroissants).
     * Effet structurel fort de l'historique de mobilité (le nombre d'entreprises antérieures réduit mécaniquement la durée de la séquence en cours).
4. **Diagnostics économétriques :**
   * Mise en évidence d'une hétéroscédasticité des résidus via les tests de Goldfeld-Quandt, Gleisjer et Breusch-Pagan, nécessitant d'interpréter les résultats avec prudence malgré la convergence des estimateurs sur grand échantillon ($N = 5548$).

---

## 📈 Aperçu des Résultats clés
* **Modèle globalement significatif** ($F = 247.43, p < 0.001$).
* Le **nombre d'entreprises traversées** et la **situation professionnelle actuelle** s'avèrent être les déterminants les plus puissants de la stabilité en emploi dans cet échantillon.

---

## 👤 Auteur
* **Eric Lin** — Étudiant en Master 1 Data Sciences for Social Sciences (Université Paris Nanterre) & Licence en Économie-Gestion (Université Paris-Panthéon-Assas)
