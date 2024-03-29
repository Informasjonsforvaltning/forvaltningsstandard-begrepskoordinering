# Forvaltningsstandard for begrepsharmonisering og begrepsdifferensiering

For revisjon av _Forvaltningsstandard for begrepsharmonisering og begrepsdifferensiering_.

Klikk på Issues og deretter New issue for å melde inn endringsbehov og endringsforslag. Det forutsetter at du har registrert deg som bruker på GitHub, med den fordelen at vi lettere kan få tak i deg for ev. avklaringsspørsmål.

[\- _Digitaliseringsdirektoratet / Norwegian Digitalisation Agency_](https://digdir.no/)

## Publisering
 - Gjeldende versjon av standarden blir publisert til: https://data.norge.no/specification/forvaltningsstandard-begrepskoordinering
 - "Redaktørens utkast" blir publisert til: https://informasjonsforvaltning.github.io/forvaltningsstandard-begrepskoordinering

## Å bidra direkte
For å bidra til utviklingen av denne standarden, må du clone den til din datamaskin og opprette en pull request.

### Clone til din datamaskin
For at det følgende skal virke på din maskin, må du ha programvare installert:  
 - [Git](https://git-scm.com/)
 - en tekst-editor, f.eks. [Atom editor](https://atom.io/)


 Dersom du bruker Atom kan du gjøre som følger:  
  - Trykk `Ctrl+Shift+P`
  - Skriv `GitHub: Clone` og trykk Enter
  - I Clone from legger du inn følgende url `https://github.com/Informasjonsforvaltning/forvaltningsstandard-begrepskoordinering.git`

Alternativt i kommando-linje:
```
% git clone https://github.com/Informasjonsforvaltning/forvaltningsstandard-begrepskoordinering.git
% cd forvaltningsstandard-begrepskoordinering
% atom .                                # dersom du har installert Atom
```
### Gjøre endringer
Denne standarden er laget i [AsciiDoc](http://asciidoc.org/) med hjelp av verktøyet [Asciidoctor](https://asciidoctor.org/).

Alle endringer må gjøre ved å endre eller legge til filer i docs-folderen. Se for eksempel på følgende veileder for god AsciiDoc praksis: https://asciidoctor.org/docs/asciidoc-recommended-practices

En typisk git-arbeidsflyt vil være som følger:
```
% git checkout master
% git pull
% git checkout -b <ny branch>
% ... # gjør endringer i din valgte editor
% git add <filer som er endra>          # legger endringer klare for commit
% git commit -m "Fornuftig feilmeldng"  # utføre commit
% git push                              # publisere branch og gjøre klar for PR
```
Dersom du bruker Atom har du støtte for alt dette i Git-panelet.

Gå til https://github.com/Informasjonsforvaltning/forvaltningsstandard-begrepskoordinering/pulls og opprett `New pull request`

#### Forhåndsvise
Dersom du bruker [Atom editor](https://atom.io/) kan du installere pakken [AsciiDoc Assistant Package](https://atom.io/packages/asciidoc-assistant).
Du vil da få syntax-uthevelse og forhåndsvisning.

#### Generere html og pdf lokalt

For at det følgende skal virke på din maskin, må du ha programvare installert:  
 - [docker](https://www.docker.com/products/docker-desktop)

```
% docker run -it -v $(pwd):/documents asciidoctor/docker-asciidoctor
bash-5.0# asciidoctor -D docs -o index.html docs/main.adoc
bash-5.0# asciidoctor-pdf -D docs -o document.pdf docs/main.adoc
```
Åpne filen index.html i din nettleser.

- [AsciidocFX](https://asciidocfx.com/) er et annet alternativ for generering av html og pdf lokalt


#### Teste html i en webserver på din maskin
Dersom du vil teste html på en server på din maskin, kan du f.eks. installere [Live Server](https://pypi.org/project/live-server/)
For dette trenger du å installere Python på din datamaskin:
- [python](https://www.python.org/downloads/)

```
% python -m pip install --user live-server
% live-server docs
```
Åpne en nettleser og gå til http://localhost:8888
