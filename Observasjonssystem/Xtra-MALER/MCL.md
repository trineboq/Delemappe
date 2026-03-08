<%*

// Hent innhold
const sel = tp.file.selection()?.trim() || "";
const clip = (await tp.system.clipboard())?.trim() || "";

// Funksjon for å formatere tekst som >> callout
const fmt = txt => txt.replace(/\n+/gm, "\n>> ");

// --- MENYSTRUKTUR ---

const menu = {
    "Multicolumn": {
        "Fra valgt": `> [!multi-column]\n>\n>> [!blank-container]\n>> ${fmt(sel)}`,
        "Fra utklipp": `> [!multi-column]\n>\n>> [!blank-container]\n>> ${fmt(clip)}`
    },

    "Blank-container": {
        "Fra valgt": `>> [!blank-container]\n>> ${fmt(sel)}`,
        "Fra utklipp": `>> [!blank-container]\n>> ${fmt(clip)}`
    },

    "Float": {
        "Venstre liten":  "> [!blank-container|float-left-small] ",
        "Venstre medium": "> [!blank-container|float-left-medium] ",
        "Venstre stor":   "> [!blank-container|float-left-large] ",
        "Høyre liten":    "> [!blank-container|float-right-small] ",
        "Høyre medium":   "> [!blank-container|float-right-medium] ",
        "Høyre stor":     "> [!blank-container|float-right-large] "
    },

    "Bilder": {
        "Venstre 300": "> [!blank-container|float-left|300] ",
        "Høyre 300":   "> [!blank-container|float-right|300] "
    },

    "YAML / CSS": {
        "Wide-page": "Wide-page",
        "Gallery-view": "Gallery-view"
    },

    "Tagger": {
        "List-card": " #mcl/list-card ",
        "Grid-liste": " #mcl/list-grid ",
        "Kolonneliste": " #mcl/list-column "
    }
};

// --- STEG 1: Velg kategori ---
const category = await tp.system.suggester(
    Object.keys(menu),
    Object.keys(menu),
    true,
    "Velg kategori"
);

// --- STEG 2: Velg alternativ ---
const choice = await tp.system.suggester(
    Object.keys(menu[category]),
    Object.values(menu[category]),
    true,
    "Velg type"
);

// Returner valgt tekst
tR += choice;

%>
