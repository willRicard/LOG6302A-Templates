# LOG6302A - JavaCC Template

This directory provides a Dockerfile template for using JavaCC as the parser
generator for software analysis required in LOG6302A labs.

Ce répertoire fournit un modèle de Dockerfile pour utiliser JavaCC comme
générateur de parseur en vue des analyses de logiciels requises pour les
laboratoires de LOG6302A.

## Instructions

```
docker build -t log6302a-javacc .
```

```
docker run -v /path/to/your/files:/app -it log6302a-javacc bash
```

## Visitor

If your visitor class is named `MyPHPVisitor`, edit `PHP.jj` to add the following:

Si votre classe de visiteur s'appelle `MyPHPVisitor`, ajoutez les lignes suivantes à `PHP.jj`:

```java
public static void main ( String args [ ] ) {
    // ...
    try {
        // REPLACE `parser.PhpPage();` WITH / REMPLACER `parser.PhpPage()` par:
        MyVisitor visitor = new MyVisitor();
        visitor.jjAccept(visitor, null);
    } catch (ParseException e) {
        // JavaCC error handling ...
    }
}
```
