<%*
// Hent utvalget
let noteContent = tp.file.selection();
// Opprett et array av linjer
let lines = noteContent.split('\n');
// Lag en ny streng med linjer uten prefikset ">"
let newContent = "";
lines.forEach(l => {
  if (l.startsWith('\*\*Koder\*\*')) {
    // Fjern prefikset ">" fra linjer som allerede har det
    l = l.replace(/$/, " ([[" + tp.file.title + "]])");
    l = l.replace(/  +/, " ");
  }
  newContent += l + "\n";
});
%>
<%newContent%>