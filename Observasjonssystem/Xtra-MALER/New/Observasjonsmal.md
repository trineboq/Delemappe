<%*
let Identifikator = await tp.system.prompt("Skriv identifikator som lar deg (ikke utenforstående) identifisere den som observasjon gjelder","")
titleName = tp.date.now("YYMMDD") + "-" + Identifikator
await tp.file.rename(titleName);
await tp.file.move( "ObsNotater/" + Identifikator + "/" + titleName)
-%>
# Observasjon
**ID:** <% Identifikator %>
**Dato:** <%tp.date.now("DD.MM.YYYY")%>
**Fra:** <%tp.date.now("HH:mm")%>
**Til:** 
**Antall voksne av totalt:** 
**Antall barn av totalt:** 

## Informasjon fra ansatte
> **Gjennom observasjonen opplyser ansatte om ...**

## Mine notater


## Spørsmål
> **Ga observasjonen et representativt bilde av barnets behov?**
> 

## Deskriptive notater
