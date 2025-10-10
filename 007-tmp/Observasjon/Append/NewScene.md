<%*
let Scene = await tp.system.prompt("Ny situasjon (Gi beskrivende navn):","");
let Brn = await tp.system.prompt("Antall barn:","");
let Voksne = await tp.system.prompt("Antall voksne:","")
-%>

### <% Scene %> (Antall barn: <% Brn %>; Antall ansatte: <% Voksne %>)
<% tp.date.now("HH:mm:ss") %>: <% tp.file.cursor(1) %>
