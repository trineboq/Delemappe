<%*
let noteContent = tp.file.selection();

// Dekoder prosentkodingen i teksten
let newContent = decodeURIComponent(noteContent);

return newContent;
%>