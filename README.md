## ¿De qué trata?

Este diagrama muestra cómo se guarda la información de una biblioteca: qué libros hay, quién los escribió y qué editorial los publicó.

## Las tres tablas

- **Autores:** guarda a las personas que escriben los libros. Cada autor tiene un número único (`ID_Autor`) y su nombre.
- **Editores:** guarda las editoriales que publican los libros. También tiene un número único (`ID_Editor`) y el nombre.
- **Libros:** guarda cada libro con su número único (`ID_Libro`) y su título. Además tiene dos campos que lo conectan con su autor (`ID_Autor`) y su editor (`ID_Editor`).

## ¿Cómo se conectan?

- Un autor puede tener muchos libros, pero cada libro tiene un solo autor.
- Un editor puede publicar muchos libros, pero cada libro tiene un solo editor.

Por eso en el diagrama aparece `1` del lado de `Autores` y `Editores`, y `N` (muchos) del lado de `Libros`.

## ¿Por qué está bien organizado?

Porque cada dato se guarda una sola vez. Por ejemplo, el nombre de un autor no se repite en cada uno de sus libros. Solo se guarda en la tabla `Autores` y los libros lo “señalan” con su número. Así la información es más ordenada y fácil de actualizar, y eso es lo que se busca con la Tercera Forma Normal (3FN).

## Diagrama

[Abrir diagrama en draw.io](https://app.diagrams.net/#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fsofiaperez-gi%2FDiagrama_Reto1%2Fmain%2Fdiagrama_er_libros%2520%25284%2529.drawio)
