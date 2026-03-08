<%*
// Hent utvalget
let noteContent = tp.file.selection();
// Opprett et array av linjer
let newContent = noteContent;
newContent = newContent.trim();
newContent = newContent.replace(/^ +/gm, '');
// Returner den komplette callout-blokken
return newContent;
-%>