<%*
/* --- 1. Velg kodespråk --- */
const languages = {
    "JavaScript": "javascript",
    "CSS": "css",
    "JSON": "json",
    "Markdown": "md",
    "HTML": "html",
    "Python": "python",
    "Bash": "bash",
    "YAML": "yaml"
};
const lang = await tp.system.suggester(
    Object.keys(languages),
    Object.values(languages),
    true,
    "Velg kodespråk"
);

/* --- 2. Hent innhold --- */
let clipboard = await tp.system.clipboard();
let selection = tp.file.selection();
let elseContent = tp.file.cursor(1);
let contentIs = selection !== "" ? selection : clipboard || elseContent;
/* --- 3. Rens og formater innhold --- */
let content = contentIs
    .split("\n")
    .map(line => `${line}`)
    .join("\n")
    .replace(/\n[\t ]*\n/gm, '\n');
%>
```<%lang%>
<%content%>
```
