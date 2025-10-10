<%*
let teamsID = await tp.system.prompt("Teams-ID","")
titleName = tp.date.now("YYMMDD") + "-" + teamsID
await tp.file.rename(titleName);
await tp.file.move( teamsID + "/" + titleName)
-%>


```ad-husk-orange
title: Forkortelser:
collapse: closed
> **Tips:** På iphone og mac kan du legge inn følgende teksterstatninger. Da kan du skrive tekst merket i fet skrift under og få tekst som følger

**brn** barnet
**ans** ansatt 
**daBrn** det andre barnet 
**dnans** den ansatte
**sseg** setter seg 
**rseg** reiser seg 
```

> [!info]- Før observasjon
> ![[_Før observasjon]]

# Observasjon
<%tp.date.now("YYMMDD")%>-<% teamsID %>-Observasjon

**Teams-ID:** <%tp.file.folder(true)%>
**Dato:** <%tp.date.now("DD.MM.YYYY")%>
**Fokus:**
- <%tp.file.cursor(2)%>

## Deskriptive notater
<%tp.file.cursor(3)%>

## Beskrivelse av …

### Barnet
> [!Husk-orange]- Kan handle om
> - Hvordan tolker du barnet?
> - Barnets interesser - Hva søker barnet seg mot?
> - Barnets engasjement 
> - Hvordan deltar barnet i aktiviteter som observeres?
> - Barnets interesser - Hva søker barnet seg mot?
> - Barnets engasjement 
> - Hvordan deltar barnet i aktiviteter som observeres?
> - Hvilke behov blir observert?
> - Hvordan påvirkes deltagelse av nedsatt funksjonsevne? 
Barnet gjør bla bla
### Barnegruppen
> [!Husk-orange]- Kan handle om
> Kort beskrivelse av barnegruppe
> Ressurser i gruppen? Observeres andre behov? 
> Hvordan bidrar andre barn til barnets deltakelse?

### Ansatte
> [!Husk-orange]- Kan handle om
> Hvordan ansatte bruker kunnskap og kompetanse med barnet?
> Hvordan bruker ansatte andre barn for å fremme barnets deltakelse?
> Hvordan 
> Hva gjøres av ansatte og for at barnet kan delta?
> Hvordan ivaretar ansatte barnets behov? 

### Fysisk utforming
> [!Husk-orange]- Kan handle om
> Kart-bilde av barnehagen:
> Hvor ligger avdelingen i bygget?
> Dører, adkomst og gjennomstrømning: 
> Lydforhold:
> Lysforhold:
> Møblering: 
> Tilgang til leker:
> Visuell støtte:
> Andre hjelpemidler: 
> 
> Hvordan er barnets generelle mulighet til å være til stede i de ulike rommene?
> Observeres det tydelige barrierer i fysisk miljø?

## Etter observasjon
> [!info]- Nyttig info fra notat
> ![[_etter observasjon]]


