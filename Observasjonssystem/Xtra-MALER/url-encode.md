<%*
let noteContent = tp.file.selection();

// Dekoder prosentkodingen i teksten
let newContent = encodeURIComponent(noteContent);

return newContent;
%>