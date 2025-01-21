# LOG6302A - ANTLR Template

This directory provides a Dockerfile template for using ANTLR as the parser
generator for software analysis required in LOG6302A labs.

Ce répertoire fournit un modèle de Dockerfile pour utiliser ANTLR comme
générateur de parseur en vue des analyses de logiciels requises pour les
laboratoires de LOG6302A.

## Instructions

```
docker build -t log6302a-antlr .
```

```
docker run -v /path/to/your/files:/app -it log6302a-antlr bash
```

## Visitor

You can use the PHP grammar from the [official repository](https://github.com/antlr/grammars-v4/tree/master/php). Walk the parse tree using the supported language of your choice.

Vous pouvez utiliser la grammaire PHP du [dépôt officiel](https://github.com/antlr/grammars-v4/tree/master/php). Parcourez l'arbre de parsage en utilisant le langage supporté de votre choix.
