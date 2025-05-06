# JavaMetricator

# Analyseur de Tests Java (TLOC / TAssert / TPCM)

## 📌 Description

Ce projet Java permet d'analyser automatiquement des fichiers `.java` afin de mesurer la qualité des tests via trois métriques principales :

- **TLOC (Test Lines of Code)** : Nombre de lignes de code significatives (hors commentaires et lignes vides).
- **TAssert** : Nombre d'assertions (`assert`) utilisées dans le code.
- **TPCM (Test Percentage Coverage Metric)** : Ratio `TAssert / TLOC` mesurant l'intensité des tests.

L'outil peut générer un fichier CSV contenant ces métriques, trier les classes selon leur couverture de test, et identifier celles qui sont potentiellement sous-testées.

---

## 📁 Structure du projet

```bash
.
├── TLOC.java           # Calcule les lignes de code significatives
├── TAssert.java        # Compte le nombre d'assertions
├── tls.java            # Analyse un dossier, génère un fichier CSV
├── tropcomp.java       # Trie les classes selon leur couverture TPCM
└── output.csv          # (Généré automatiquement) Résultats des métriques
