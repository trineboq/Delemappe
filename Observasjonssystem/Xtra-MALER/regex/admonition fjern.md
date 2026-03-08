<%*
// Hent utvalget
let noteContent = tp.file.selection();
// Opprett et array av linjer
let newContent = noteContent;
newContent = newContent.trim();
newContent = newContent.replace(/^```+(ad.*){0,1}\n/gm, '');
newContent = newContent.replace(/```+/gm, '');
newContent = newContent.replace(/\ncollapse: .*/gm, '');
newContent = newContent.replace(/\ncollapse: .*/gm, '');;
newContent = newContent.replace(/\ntitle: \n/gm, '\n');
newContent = newContent.replace(/\ntitle: (.+)/gm, '\n###### $1');
return newContent;
%>