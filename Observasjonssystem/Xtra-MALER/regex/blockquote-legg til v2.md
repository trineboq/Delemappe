<%*
// Hent utvalget
let noteContent = tp.file.selection();
// Opprett et array av linjer
let lines = noteContent.split('\n');
// Lag en ny streng med oppdaterte linjer
let newContent = "";
lines.forEach(l => {
  let formattedLine = l.trim(); // Fjern mellomrom på begynnelsen og slutten av linjen
  if (!formattedLine.startsWith('> ')) {
    // Legg til prefikset ">" i linjer som ikke har det
    newContent += '>' + formattedLine + "\n";
  } else {
    // Legg til ekstra ">" i linjer som allerede har minst ett ">"
    let prefix = '';
    while (formattedLine.startsWith('>') && !formattedLine.startsWith('> ')) {
      prefix += '>';
      formattedLine = formattedLine.substring(1).trim();
    }
    newContent += prefix + '> ' + formattedLine + "\n";
  }
});
// Fjern det siste linjeskiftet
newContent = newContent.replace(/(\n)+$/, "");
// Returner den oppdaterte teksten
return newContent;
-%>