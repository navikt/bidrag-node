# bidrag-node
Github node Actions spesialisert for team bidrag

### Continuous integration
![](https://github.com/navikt/bidrag-node/workflows/build%20actions/badge.svg)

### Hovedregel for design:
Alt blir utført av bash-scripter slik at det enkelt kan testes på reell kodebase uten å måtte bygge med github.

Det er lagt inn en workflow for å bygge alle actions med npm og ncc. Derfor er det bare filene `/<action>/index.js` og `/<action>/<bash>.sh` som skal
endres når man skal forandre logikk i "action".

### Changelog

Versjon | Endringstype | Beskrivelse
--------|--------------|------------
v1      | Opprettet    | `build-with-ncc`: bygg av node komponenter med ncc
