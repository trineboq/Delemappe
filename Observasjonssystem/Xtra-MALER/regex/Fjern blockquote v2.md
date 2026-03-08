<%*
// Hent utvalget
let noteContent = tp.file.selection();
// Opprett et array av linjer
let lines = noteContent.split('\n');
// Lag en ny streng med linjer uten prefikset ">"
let newContent = "";
lines.forEach(l => {
  if (l.startsWith('>')) {
    // Fjern prefikset ">" fra linjer som allerede har det
    l = l.replace(/^>/, "");
  }
  // Fjern eventuelle mellomrom på starten av linjer
  l = l.replace(/^\s+/, "");
  newContent += l + "\n";
});
// Fjern det siste linjeskiftet
newContent = newContent.replace(/(\n)+$/, "");
// Returner den oppdaterte teksten
return newContent;
%>