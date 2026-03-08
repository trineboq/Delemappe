<%*
const typeSelect = {
	"center"         : "Center",
	"draft"          : "Draft",
	"code"           : "Code",
	"cite"           : "Cite",
	"web"            : "Web",
	"lecture"        : "Lecture",
	"lecturenb"      : "LectureNB",
	"clip"           : "📋 Clip = Div direkte kopi",
	"KI"             : "🟣 KI - Direkte kopi fra Kunstig intelligens",
	"Yellow"         : "🟡 Yellow",
	"Green"          : "🟢 Green = Bokrelatert",
	"Orange"         : "🟠 Orange = Lister",
	"Viktig"         : "❗ Viktig",
	"Pink"           : "🔴 Rosa",
	"Magenta"        : "🌸 Magenta",
	"Blue"           : "🔵 Blå",
	"Cyan"           : "🔵 Lyseblå (cyan)",
	"Purple"         : "🟣 Lilla (purple)",
	"header"         : "#️⃣ header",
	"info"           : "ℹ️ Info",
	"link"           : "🔗 link/lenke",
	"quote"          : "💬Quote",
	"meta"           : "Meta",
	"arkiv"          : "Arkiv",
	"multi-column"   : "Multi-column",
	"blank-container": "Blank-container"
};
const type = await tp.system.suggester(
	Object.values(typeSelect), 
	Object.keys(typeSelect), 
	true, 
	"Velg type"
);
const dotSelect = {
	"```"    : "x3",
	"````"   : "x4", 
	"`````"  : "x5",
	"``````" : "x6"
};
const dot = await tp.system.suggester(
	Object.values(dotSelect), 
	Object.keys(dotSelect), 
	true, 
	"Velg antall apostrofer"
);
const foldSelect = {
	""                   : "Ingen",
	"\ncollapse: open"   : "Åpen",
	"\ncollapse: closed" : "Lukket"
}
const fold = await tp.system.suggester(
	Object.values(foldSelect), 
	Object.keys(foldSelect), 
	true, 
	"Velg visningstype"
);
let clipboard = await tp.system.clipboard();
let selection = tp.file.selection();
let elseContent = tp.file.cursor(1);
if (selection === "") {
	contentIs = clipboard
}	else {
	contentIs = selection
};
let content = contentIs.split("\n").map(line =>`${line}`).join("\n").replace(/ /g, " ").replace(/\n[\t ]*\n/gm, '\n');

const calloutHead = `${dot}ad-${type}${fold}\ntitle: `;

const calloutFoot = `\n${dot}\n`;

tR += calloutHead + content + calloutFoot
%>