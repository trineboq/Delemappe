<%*
const callouts = {
	"|float-left|300"   :  "Bilde - Venstre 300",
	"|float-right|300"  :  "Bilde - Høyre 300"
};

const type = await tp.system.suggester(
	Object.values(callouts), 
	Object.keys(callouts), 
	true, 
	'Velg type'
);

tR += type

%>