# LOG6302A - tree-sitter Template

This directory provides a Dockerfile template for using tree-sitter as the
parser generator for software analysis required in LOG6302A labs.

Ce répertoire fournit un modèle de Dockerfile pour utiliser tree-sitter comme
générateur de parseur en vue des analyses de logiciels requises pour les
laboratoires de LOG6302A.

## Instructions

```
docker build -t log6302a-tree-sitter .
```

```
docker run -v /path/to/your/files:/app -it log6302a-tree-sitter bash
```

## Visitor

You can walk the parsed syntax tree using the native [tree cursor](https://tree-sitter.github.io/tree-sitter/using-parsers/4-walking-trees.html)
API or one of tree-sitter's many [bindings](https://tree-sitter.github.io/tree-sitter/index.html).

Vous pouvez parcourir l'arbre de syntaxe issu du parsage en utilisant l'API
native [tree cursor](https://tree-sitter.github.io/tree-sitter/using-parsers/4-walking-trees.html)
ou l'un des nombreux [bindings](https://tree-sitter.github.io/tree-sitter/index.html) de tree-sitter.
