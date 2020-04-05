# Forvaltningsstandard for begrepsharmonisering og begrepsdifferensiering

For revisjon av _Forvaltningsstandard for begrepsharmonisering og begrepsdifferensiering_.

Klikk på Issues og deretter New issue for å melde inn endringsbehov og endringsforslag. Det forutsetter at du har registrert deg som bruker på GitHub, med den fordelen at vi lettere kan få tak i deg for ev. avklaringsspørsmål.

[\- _Digitaliseringsdirektoratet / Norwegian Digitalisation Agency_](https://digdir.no/)


## Bidra
For å bidra til utviklingen av denne standarden, må du clone den til din datamaskin og opprette en pull request.
### Clone til din datamaskin
Dersom du bruker [Atom editor](https://atom.io/) kan du gjøre som følger:  
 - Trykk `Ctrl+Shift+P`
 - Skriv `GitHub: Clone` og trykk Enter
 - I Clone from legger du inn følgende url `https://github.com/Informasjonsforvaltning/forvaltningsstandard-begrepskoordinering.git`

### Gjøre endringer

Denne standarden er laget i [AsciiDoc](http://asciidoc.org/) med hjelp av verktøyet [Asciidoctor](https://asciidoctor.org/).

Alle endringer må gjøre ved å endre eller legge til filer i docs-folderen. Se for eksempel på følgende veileder for god AsciiDoc praksis: https://asciidoctor.org/docs/asciidoc-recommended-practices

#### Forhåndsvisning
Dersom du bruker [Atom editor](https://atom.io/) kan du installere pakken [AsciiDoc Assistant Package](https://atom.io/packages/asciidoc-assistant).
Du vil da få syntax-uthevelse og forhåndsvisning.

#### Generer html, pdf og epub lokalt

For at det følgende skal virke på din maskin, må du ha følgende programvare installert:  
 - [docker](https://www.docker.com/products/docker-desktop)
 - [python](https://www.python.org/downloads/)

```
% docker run -it -v $(pwd):/documents asciidoctor/docker-asciidoctor
bash-5.0# asciidoctor -D docs -o index.html docs/main.adoc
bash-5.0# asciidoctor-pdf -D docs -o document.pdf docs/main.adoc
bash-5.0# asciidoctor-epub3 -D docs -o document.epub docs/main.adoc
```
Åpne filen index.html i din nettleser.

Dersom du vil teste html på en server på din maskin, kan du feks installere [Live Server](https://pypi.org/project/live-server/)
```
% python -m pip install --user live-server
% live-server docs
```
Åpne en nettleser og gå til http://localhost:8888

### Publisere endringsforslag
Etter at du har utført endringene, og publisert disse til en branch du har skrive-tilgang til, må du opprette en [pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request)

Dersom du bruker [Atom editor](https://atom.io/) kan du gjøre som følger:
 - Lag en ny branch med et passende navn
 - Åpne `Git`-panelet (nede til høyre)
 - Commit endringene med en fornuftig melding
 - Publiser endringene dine ved å trykke `Publish`
 - Gå til https://github.com/Informasjonsforvaltning/forvaltningsstandard-begrepskoordinering/pulls og opprett `New pull request`
