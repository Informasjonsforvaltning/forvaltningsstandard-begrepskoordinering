# Forvaltningsstandard for begrepsharmonisering og begrepsdifferensiering

For revisjon av _Forvaltningsstandard for begrepsharmonisering og begrepsdifferensiering_.

Klikk på Issues og deretter New issue for å melde inn endringsbehov og endringsforslag. Det forutsetter at du har registrert deg som bruker på GitHub, med den fordelen at vi lettere kan få tak i deg for ev. avklaringsspørsmål.

\- _Digitaliseringsdirektoratet / Norwegian Digitalisation Agency_ (https://digdir.no/)

## Generate locally
```
% docker run -it -v $(pwd):/documents asciidoctor/docker-asciidoctor
bash-5.0# asciidoctor -D docs -o index.html docs/main.adoc
bash-5.0# asciidoctor-pdf -D docs -o document.pdf docs/main.adoc
bash-5.0# asciidoctor-epub3 -D docs -o document.epub docs/main.adoc
```
