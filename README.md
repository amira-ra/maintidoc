# MaintiDoc – Livrable 1 : cadrage, corpus et architecture

**Module** : IA générative multimodale – EMSI 2026 – **Enseignante** : Pr. Mariam Cherrabi

## Équipe
Travail individuel : **Amira RMAILI**.

## Objectif du projet
MaintiDoc est un assistant documentaire multimodal et agentique pour la maintenance : à partir d'une question et d'une photo, il retrouve dans un corpus autorisé les passages et figures pertinents, consulte l'historique des interventions via un outil MCP, répond avec des sources vérifiées et prépare un ticket créé seulement après approbation humaine. Il ne pilote aucune machine et ne garantit aucun diagnostic.

## Contenu du ZIP
```
L1_MaintiDoc_RMAILI.zip
└── L1_MaintiDoc_RMAILI/
    ├── L1_MaintiDoc_RMAILI_Rapport.pdf       rapport complet (parties 2.1 à 2.6)
    ├── L1_MaintiDoc_RMAILI_LienGitHub.txt    URL du dépôt GitHub
    ├── README.md             ce fichier
    └── L1_MaintiDoc_RMAILI_Corpus/
        ├── inventaire.csv    registre des 40 documents (20 colonnes)
        ├── prompts_corpus.md prompts P01 à P11 (outil, date)
        ├── documents/famille_1/  pompes (17 PDF)
        ├── documents/famille_2/  compresseurs (17 PDF)
        └── images/           6 photos synthétiques
```

## Structure du dépôt GitHub
```
maintidoc/
├── README.md
├── .gitignore
├── docs/diagrammes/   sources Mermaid (.mmd) et images (.png)
└── corpus/            inventaire.csv, prompts_corpus.md, documents/, images/
```

## Corpus
40 documents synthétiques (aucune donnée réelle) : pompes (POMPE-A-01, POMPE-C-01) et compresseurs (COMP-B-02, COMP-D-01). Groupes d'accès : `techniciens_pompes`, `techniciens_compresseurs`, `responsables`. Cas de test : 2 conflits de versions, 1 document piégé, cas ambigus, documents réservés.
