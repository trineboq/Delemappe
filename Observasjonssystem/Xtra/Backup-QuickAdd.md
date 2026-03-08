Hvis du skulle miste enkelte handlinger ved en feil kan du rette opp raskt som følger:

1. Kopier koden under (Trykk på knappen "JSON")
2. Åpne innstillinger > QuickAdd > Import package
3. Lim inn i skrivefelt 
4. Importer


```JSON
{
  "schemaVersion": 1,
  "quickAddVersion": "2.12.0",
  "createdAt": "2026-03-08T19:09:50.992Z",
  "rootChoiceIds": [
    "59dadd14-59d6-47cf-9bab-1159b37f766f",
    "cff3180e-2e4a-4d1d-83f6-03910b5c2bea",
    "1d972be4-ee00-45e4-95e7-597c373621b3",
    "16199ed4-2e89-48d0-b7f0-ab349274523b",
    "64fb31c8-c4a1-4881-bce3-c7d82ab00ba4",
    "94e07fba-f717-4e4c-b48b-1852fe94e6f4",
    "35e3f22b-de1a-499b-a296-2411b55d2e15",
    "5f36a713-1e27-4a79-8284-98850aa752ea",
    "21fe5355-217b-4813-a826-e4acc2db710d",
    "429f0b1a-db73-4354-b937-a89d7c621d27",
    "51979bab-d6cf-4009-aa01-a442ea6124f9",
    "64340162-284a-4ea9-848c-68cfc2a2838e",
    "944b8b27-e6a3-427e-90bd-f52f80b81838"
  ],
  "choices": [
    {
      "choice": {
        "id": "59dadd14-59d6-47cf-9bab-1159b37f766f",
        "name": "Ny linje",
        "type": "Multi",
        "command": false,
        "choices": [
          {
            "id": "e9aef02d-df10-4191-acd4-3b6cd5b6a6f6",
            "name": "Ny aktivitet (Bunn) ⏭️",
            "type": "Capture",
            "command": true,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "activeFileWritePosition": "bottom",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "\n### {{GLOBAL_VAR:ObsSituasjoner}}; Antall barn: {{value:Antall barn}}; Antall voksne: {{value:Antall ansatte}}; Fra kl: {{TIME:HH:mm}}; Til kl: \n**{{TIME:HH:mm:ss}}:** {{value:Hvem hvor hva (første beskrivelse i ny aktivitet)}} <%tp.file.cursor(2)%>"
            },
            "insertAfter": {
              "enabled": false,
              "after": "### Fysisk utforming",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top"
            },
            "newLineCapture": {
              "enabled": false,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "none"
            }
          },
          {
            "id": "ed1fd49e-1e3b-422c-96eb-a13974f1e620",
            "name": "Ny deskriptiv (Bunn) ⏱️",
            "type": "Capture",
            "command": true,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "**{{TIME:HH:mm:ss}}:** {{value:Beskriv det du ser, og hører}} <%tp.file.cursor(2)%>"
            },
            "insertAfter": {
              "enabled": false,
              "after": "### Fysisk utforming",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top"
            },
            "newLineCapture": {
              "enabled": false,
              "direction": "below"
            },
            "prepend": true,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "none"
            }
          },
          {
            "id": "da9d1275-7c52-478f-ab41-524743de39f3",
            "name": "Ny Notatmarkør (Bunn) 🗒️",
            "type": "Capture",
            "command": true,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "**{{TIME:HH:mm:ss}}:** ;**{{GLOBAL_VAR:DeskriptivTagg}}:**; {{value:Notat om dette}} <%tp.file.cursor(2)%>"
            },
            "insertAfter": {
              "enabled": false,
              "after": "### Fysisk utforming",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top"
            },
            "newLineCapture": {
              "enabled": false,
              "direction": "below"
            },
            "prepend": true,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "none"
            }
          },
          {
            "id": "e43dbaa4-56d3-44e2-a2a3-fb81a0171bb6",
            "name": "Ny aktivitet (under)",
            "type": "Capture",
            "command": true,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "\n### {{GLOBAL_VAR:ObsSituasjoner}}; Antall barn: <%tp.file.cursor(1)%>; Antall ansatte: <%tp.file.cursor(2)%>; Fra kl: {{TIME:HH:mm}}; Til kl: \n**{{TIME:HH:mm:ss}}:** {{value:Hvem hvor hva (første beskrivelse i ny aktivitet)}} <%tp.file.cursor(3)%>"
            },
            "insertAfter": {
              "enabled": false,
              "after": "### Fysisk utforming",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top"
            },
            "newLineCapture": {
              "enabled": true,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "wholeFile"
            }
          },
          {
            "id": "bedaabd4-fa55-4b86-aac9-49b07d272dde",
            "name": "Ny Notatmarkør (Under) 🗒️",
            "type": "Capture",
            "command": true,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "**{{TIME:HH:mm:ss}}:** ;**{{GLOBAL_VAR:DeskriptivTagg}}:**; "
            },
            "insertAfter": {
              "enabled": false,
              "after": "### Fysisk utforming",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top"
            },
            "newLineCapture": {
              "enabled": true,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "none"
            }
          },
          {
            "id": "8808ecb4-99ad-4c05-9802-bdff581ff9b1",
            "name": "Inline DeskriptivTagg",
            "type": "Capture",
            "command": true,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": " ;**{{GLOBAL_VAR:DeskriptivTagg}}:**; <%tp.file.cursor()%>"
            },
            "insertAfter": {
              "enabled": false,
              "after": "",
              "insertAtEnd": false,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top",
              "inline": false,
              "replaceExisting": false,
              "blankLineAfterMatchMode": "auto"
            },
            "newLineCapture": {
              "enabled": false,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "wholeFile"
            }
          },
          {
            "id": "160ecfcd-046b-4ba6-84ba-2e076954bf59",
            "name": "Ny deskriptiv (Under)",
            "type": "Capture",
            "command": true,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "**{{TIME:HH:mm:ss}}:** "
            },
            "insertAfter": {
              "enabled": false,
              "after": "### Fysisk utforming",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top"
            },
            "newLineCapture": {
              "enabled": true,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "wholeFile"
            },
            "isDndShadowItem": true
          }
        ],
        "collapsed": false
      },
      "pathHint": [
        "Ny linje"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "cff3180e-2e4a-4d1d-83f6-03910b5c2bea",
        "name": "Div Format",
        "type": "Multi",
        "command": false,
        "choices": [
          {
            "id": "01be70cd-ace7-4dcc-a60f-7876a0642097",
            "name": "Spørsmålformat",
            "type": "Capture",
            "command": false,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "> **{{VALUE:Spørsmål til senere (trenger ikke spm.tegn)}}?**\n> \n"
            },
            "insertAfter": {
              "enabled": true,
              "after": "## Spørsmål",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top",
              "inline": false,
              "replaceExisting": false,
              "blankLineAfterMatchMode": "auto"
            },
            "newLineCapture": {
              "enabled": false,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "none"
            }
          },
          {
            "id": "7c0a8932-eeed-437a-97af-b05834b5e3ae",
            "name": "Info-Format",
            "type": "Capture",
            "command": false,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "> {{VALUE:Ansatte informerer før/under/etter (med klokkeslett)}} ({{TIME}})\n"
            },
            "insertAfter": {
              "enabled": true,
              "after": "## Informasjon fra ansatte",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top",
              "inline": false,
              "replaceExisting": false,
              "blankLineAfterMatchMode": "auto"
            },
            "newLineCapture": {
              "enabled": false,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "none"
            }
          },
          {
            "id": "e77ef54c-726e-4815-9408-89080a981810",
            "name": "Notat-tagg Format",
            "type": "Capture",
            "command": false,
            "appendLink": false,
            "captureTo": "",
            "captureToActiveFile": true,
            "captureToCanvasNodeId": "",
            "activeFileWritePosition": "cursor",
            "createFileIfItDoesntExist": {
              "enabled": false,
              "createWithTemplate": false,
              "template": ""
            },
            "format": {
              "enabled": true,
              "format": "#{{GLOBAL_VAR:NoteTagg}} {{VALUE:Notat:}} ({{time}})\n"
            },
            "insertAfter": {
              "enabled": true,
              "after": "## Mine notater",
              "insertAtEnd": true,
              "considerSubsections": false,
              "createIfNotFound": false,
              "createIfNotFoundLocation": "top",
              "inline": false,
              "replaceExisting": false,
              "blankLineAfterMatchMode": "auto"
            },
            "newLineCapture": {
              "enabled": false,
              "direction": "below"
            },
            "prepend": false,
            "task": false,
            "openFile": false,
            "fileOpening": {
              "location": "tab",
              "direction": "vertical",
              "mode": "default",
              "focus": true
            },
            "templater": {
              "afterCapture": "none"
            }
          }
        ],
        "collapsed": true
      },
      "pathHint": [
        "Div Format"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "1d972be4-ee00-45e4-95e7-597c373621b3",
        "name": "Linje start",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Linje start",
          "id": "3944df58-c091-49b8-b72a-be698c615c9d",
          "commands": [
            {
              "name": "Select active line",
              "type": "EditorCommand",
              "id": "ef00cba6-5114-452e-a570-cf971356b7d8",
              "editorCommandType": "Select active line"
            },
            {
              "name": "Move caret left",
              "type": "Obsidian",
              "id": "237c8588-c51a-48c1-943b-1a2301a336f8",
              "commandId": "editor:move-caret-left"
            }
          ]
        }
      },
      "pathHint": [
        "Linje start"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "16199ed4-2e89-48d0-b7f0-ab349274523b",
        "name": "Linje slutt",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Linje slutt",
          "id": "10b1ffa0-fd5b-4713-beff-02dcba11b35b",
          "commands": [
            {
              "name": "Select active line",
              "type": "EditorCommand",
              "id": "3abd108c-30da-4963-b5f6-c13c40261136",
              "editorCommandType": "Select active line"
            },
            {
              "name": "Move caret right",
              "type": "Obsidian",
              "id": "165662fc-703d-47c0-ab07-85c82e94b5c2",
              "commandId": "editor:move-caret-right"
            }
          ]
        }
      },
      "pathHint": [
        "Linje slutt"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "64fb31c8-c4a1-4881-bce3-c7d82ab00ba4",
        "name": "Quote",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Quote",
          "id": "5116ae65-22da-4fc4-8783-8da9d81f12a1",
          "commands": [
            {
              "name": "Untitled Capture Choice",
              "type": "NestedChoice",
              "id": "1d0a6e09-f25b-48a5-a4aa-5a109bf209c7",
              "choice": {
                "id": "ba4d8f61-9c53-444c-b6fe-b69ea6a33d4e",
                "name": "Untitled Capture Choice",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": " \"<% tp.file.cursor() %>\""
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Templater: Jump to next cursor location",
              "type": "Obsidian",
              "id": "61e4a9a3-ddda-48bc-b091-2a9dff574d31",
              "commandId": "templater-obsidian:jump-to-next-cursor-location"
            }
          ]
        }
      },
      "pathHint": [
        "Quote"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "94e07fba-f717-4e4c-b48b-1852fe94e6f4",
        "name": "Parathesis",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Parathesis",
          "id": "c0bcf0b2-adc7-4a3b-9418-6b4df9069524",
          "commands": [
            {
              "name": "Untitled Capture Choice",
              "type": "NestedChoice",
              "id": "33ec3337-952d-4e79-a6df-83c397150c26",
              "choice": {
                "id": "ba4d8f61-9c53-444c-b6fe-b69ea6a33d4e",
                "name": "Untitled Capture Choice",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": " (<% tp.file.cursor() %>)"
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Templater: Jump to next cursor location",
              "type": "Obsidian",
              "id": "8cc17c5f-fe03-4e67-a979-613eb9dab607",
              "commandId": "templater-obsidian:jump-to-next-cursor-location"
            }
          ]
        }
      },
      "pathHint": [
        "Parathesis"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "35e3f22b-de1a-499b-a296-2411b55d2e15",
        "name": "Legg til spørsmål",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Legg til spørsmål",
          "id": "b329d462-940e-4301-92d9-5bf9238047e7",
          "commands": [
            {
              "name": "Legg til cursorplassering for senere",
              "type": "NestedChoice",
              "id": "5ca3d45d-c302-487d-907c-ed0262519360",
              "choice": {
                "id": "42df7d49-1ed3-422c-91fa-884196414a32",
                "name": "Legg til cursorplassering for senere",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(1)%>"
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Spørsmålformat",
              "type": "Choice",
              "id": "72f5d51a-2cb0-4ec9-a0cb-eaf1311e49f2",
              "choiceId": "01be70cd-ace7-4dcc-a60f-7876a0642097"
            },
            {
              "name": "Templater: Jump to next cursor location",
              "type": "Obsidian",
              "id": "8e172039-0a94-4d57-bfd7-e207397ed0cc",
              "commandId": "templater-obsidian:jump-to-next-cursor-location"
            }
          ]
        }
      },
      "pathHint": [
        "Legg til spørsmål"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "5f36a713-1e27-4a79-8284-98850aa752ea",
        "name": "Legg til notat (med tagg)",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Legg til notat (med tagg)",
          "id": "03020f80-cb9d-4016-b274-e6c03c6dfb32",
          "commands": [
            {
              "name": "Legg til cursorplassering for senere",
              "type": "NestedChoice",
              "id": "4aa617ac-06e2-472c-a1ec-5ca8b34ec71a",
              "choice": {
                "id": "42df7d49-1ed3-422c-91fa-884196414a32",
                "name": "Legg til cursorplassering for senere",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(1)%>"
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Notat-tagg Format",
              "type": "Choice",
              "id": "20a5f427-8942-47a7-988b-8a0ae6c40ebc",
              "choiceId": "e77ef54c-726e-4815-9408-89080a981810"
            },
            {
              "name": "Templater: Jump to next cursor location",
              "type": "Obsidian",
              "id": "ecb093c2-6a55-432f-929b-85eff4a70dcd",
              "commandId": "templater-obsidian:jump-to-next-cursor-location"
            }
          ]
        }
      },
      "pathHint": [
        "Legg til notat (med tagg)"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "21fe5355-217b-4813-a826-e4acc2db710d",
        "name": "Legg til info fra ansatte",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Legg til info fra ansatte",
          "id": "83772910-4a2a-44b3-b117-3cff6496317d",
          "commands": [
            {
              "name": "Info-Format",
              "type": "Choice",
              "id": "6357a077-cce4-4f2e-88c3-5966f483b651",
              "choiceId": "7c0a8932-eeed-437a-97af-b05834b5e3ae"
            }
          ]
        }
      },
      "pathHint": [
        "Legg til info fra ansatte"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "429f0b1a-db73-4354-b937-a89d7c621d27",
        "name": "Gå til siste notat",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Gå til siste notat",
          "id": "e3a8eb5a-5567-4435-b69b-7ba9099f0434",
          "commands": [
            {
              "name": "plasser tpCursor2 der du er",
              "type": "NestedChoice",
              "id": "4f05bbab-ee23-48aa-a830-90dbec14fef9",
              "choice": {
                "id": "ad1b9dc2-a300-480e-9a75-ae5f993ed9be",
                "name": "plasser tpCursor2 der du er",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(2)%>"
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Plasser tpCursor1 i MineNotater-overskrift",
              "type": "NestedChoice",
              "id": "ab695294-3032-42cf-9468-7ad944fe3db1",
              "choice": {
                "id": "27d27e15-7a68-4c69-9ad8-695bc603fd95",
                "name": "Plasser tpCursor1 i MineNotater-overskrift",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(1)%>"
                },
                "insertAfter": {
                  "enabled": true,
                  "after": "## Mine notater",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": true,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Templater: Jump to next cursor location",
              "type": "Obsidian",
              "id": "70b0bbeb-56c4-47da-93a2-419e5d6c251c",
              "commandId": "templater-obsidian:jump-to-next-cursor-location"
            }
          ]
        }
      },
      "pathHint": [
        "Gå til siste notat"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "51979bab-d6cf-4009-aa01-a442ea6124f9",
        "name": "Gå til siste Info",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Gå til siste Info",
          "id": "fddd9aaa-0339-4dc2-a6df-37184b67e1e7",
          "commands": [
            {
              "name": "plasser tpCursor2 der du er",
              "type": "NestedChoice",
              "id": "6d34d30f-cb4f-4f98-bd22-98a9bd342857",
              "choice": {
                "id": "ad1b9dc2-a300-480e-9a75-ae5f993ed9be",
                "name": "plasser tpCursor2 der du er",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(2)%>"
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Plasser tpCursor1 i Info-overskrift",
              "type": "NestedChoice",
              "id": "76792407-ffeb-4151-a078-3c55f9c17f5e",
              "choice": {
                "id": "27d27e15-7a68-4c69-9ad8-695bc603fd95",
                "name": "Plasser tpCursor1 i Info-overskrift",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(1)%>"
                },
                "insertAfter": {
                  "enabled": true,
                  "after": "## Informasjon fra ansatte",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": true,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Templater: Jump to next cursor location",
              "type": "Obsidian",
              "id": "e15ecfef-b1f7-43e8-a55d-3b74767bf2c5",
              "commandId": "templater-obsidian:jump-to-next-cursor-location"
            }
          ]
        }
      },
      "pathHint": [
        "Gå til siste Info"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "64340162-284a-4ea9-848c-68cfc2a2838e",
        "name": "Gå til siste spørsmål",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Gå til siste spørsmål",
          "id": "8ee8452f-d4cb-4e0d-84c0-598ea5676e0c",
          "commands": [
            {
              "name": "plasser tpCursor2 der du er",
              "type": "NestedChoice",
              "id": "9931540b-5ce8-42fb-926a-cf7d94258af3",
              "choice": {
                "id": "ad1b9dc2-a300-480e-9a75-ae5f993ed9be",
                "name": "plasser tpCursor2 der du er",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(2)%>"
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Plasser tpCursor1 i Spm-overskrift",
              "type": "NestedChoice",
              "id": "29500b07-47da-4aa5-998b-809fe5532a3c",
              "choice": {
                "id": "27d27e15-7a68-4c69-9ad8-695bc603fd95",
                "name": "Plasser tpCursor1 i Spm-overskrift",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "<%tp.file.cursor(1)%>"
                },
                "insertAfter": {
                  "enabled": true,
                  "after": "## Spørsmål",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": true,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Templater: Jump to next cursor location",
              "type": "Obsidian",
              "id": "ee2e25b2-56d4-4b61-b25e-1aa3d1f764aa",
              "commandId": "templater-obsidian:jump-to-next-cursor-location"
            }
          ]
        }
      },
      "pathHint": [
        "Gå til siste spørsmål"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "944b8b27-e6a3-427e-90bd-f52f80b81838",
        "name": "Avslutt obs",
        "type": "Macro",
        "command": true,
        "runOnStartup": false,
        "macro": {
          "name": "Avslutt obs",
          "id": "ce793c97-6410-4cce-b593-81535b5eaf0f",
          "commands": [
            {
              "name": "Legg til sluttlinje",
              "type": "NestedChoice",
              "id": "1180c2c0-2114-4883-92bb-c2e5c45eccbf",
              "choice": {
                "id": "0b73642d-19c4-4502-af8e-28f6267528c5",
                "name": "Legg til sluttlinje",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "bottom",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "**{{time:HH:mm:ss}}:** Observasjon ferdig"
                },
                "insertAfter": {
                  "enabled": false,
                  "after": "",
                  "insertAtEnd": false,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Legg til Tid til",
              "type": "NestedChoice",
              "id": "5e30da54-e780-4f07-b96c-3570ca81f6a8",
              "choice": {
                "id": "4d79c866-0998-4c03-aa3b-509a0995ccc2",
                "name": "Legg til Tid til",
                "type": "Capture",
                "command": false,
                "appendLink": false,
                "captureTo": "",
                "captureToActiveFile": true,
                "captureToCanvasNodeId": "",
                "activeFileWritePosition": "cursor",
                "createFileIfItDoesntExist": {
                  "enabled": false,
                  "createWithTemplate": false,
                  "template": ""
                },
                "format": {
                  "enabled": true,
                  "format": "**Til kl:** {{time}}"
                },
                "insertAfter": {
                  "enabled": true,
                  "after": "# Observasjon",
                  "insertAtEnd": true,
                  "considerSubsections": false,
                  "createIfNotFound": false,
                  "createIfNotFoundLocation": "top",
                  "inline": false,
                  "replaceExisting": false,
                  "blankLineAfterMatchMode": "auto"
                },
                "newLineCapture": {
                  "enabled": false,
                  "direction": "below"
                },
                "prepend": false,
                "task": false,
                "openFile": false,
                "fileOpening": {
                  "location": "tab",
                  "direction": "vertical",
                  "mode": "default",
                  "focus": true
                },
                "templater": {
                  "afterCapture": "none"
                }
              }
            },
            {
              "name": "Regex Pipeline: notatfiks",
              "type": "Obsidian",
              "id": "69f576c3-63a5-4d0e-8723-5905658469c7",
              "commandId": "obsidian-regex-pipeline:ruleset: notatfiks"
            }
          ]
        }
      },
      "pathHint": [
        "Avslutt obs"
      ],
      "parentChoiceId": null
    },
    {
      "choice": {
        "id": "e9aef02d-df10-4191-acd4-3b6cd5b6a6f6",
        "name": "Ny aktivitet (Bunn) ⏭️",
        "type": "Capture",
        "command": true,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "activeFileWritePosition": "bottom",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "\n### {{GLOBAL_VAR:ObsSituasjoner}}; Antall barn: {{value:Antall barn}}; Antall voksne: {{value:Antall ansatte}}; Fra kl: {{TIME:HH:mm}}; Til kl: \n**{{TIME:HH:mm:ss}}:** {{value:Hvem hvor hva (første beskrivelse i ny aktivitet)}} <%tp.file.cursor(2)%>"
        },
        "insertAfter": {
          "enabled": false,
          "after": "### Fysisk utforming",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top"
        },
        "newLineCapture": {
          "enabled": false,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "none"
        }
      },
      "pathHint": [
        "Ny linje",
        "Ny aktivitet (Bunn) ⏭️"
      ],
      "parentChoiceId": "59dadd14-59d6-47cf-9bab-1159b37f766f"
    },
    {
      "choice": {
        "id": "ed1fd49e-1e3b-422c-96eb-a13974f1e620",
        "name": "Ny deskriptiv (Bunn) ⏱️",
        "type": "Capture",
        "command": true,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "**{{TIME:HH:mm:ss}}:** {{value:Beskriv det du ser, og hører}} <%tp.file.cursor(2)%>"
        },
        "insertAfter": {
          "enabled": false,
          "after": "### Fysisk utforming",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top"
        },
        "newLineCapture": {
          "enabled": false,
          "direction": "below"
        },
        "prepend": true,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "none"
        }
      },
      "pathHint": [
        "Ny linje",
        "Ny deskriptiv (Bunn) ⏱️"
      ],
      "parentChoiceId": "59dadd14-59d6-47cf-9bab-1159b37f766f"
    },
    {
      "choice": {
        "id": "da9d1275-7c52-478f-ab41-524743de39f3",
        "name": "Ny Notatmarkør (Bunn) 🗒️",
        "type": "Capture",
        "command": true,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "**{{TIME:HH:mm:ss}}:** ;**{{GLOBAL_VAR:DeskriptivTagg}}:**; {{value:Notat om dette}} <%tp.file.cursor(2)%>"
        },
        "insertAfter": {
          "enabled": false,
          "after": "### Fysisk utforming",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top"
        },
        "newLineCapture": {
          "enabled": false,
          "direction": "below"
        },
        "prepend": true,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "none"
        }
      },
      "pathHint": [
        "Ny linje",
        "Ny Notatmarkør (Bunn) 🗒️"
      ],
      "parentChoiceId": "59dadd14-59d6-47cf-9bab-1159b37f766f"
    },
    {
      "choice": {
        "id": "e43dbaa4-56d3-44e2-a2a3-fb81a0171bb6",
        "name": "Ny aktivitet (under)",
        "type": "Capture",
        "command": true,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "\n### {{GLOBAL_VAR:ObsSituasjoner}}; Antall barn: <%tp.file.cursor(1)%>; Antall ansatte: <%tp.file.cursor(2)%>; Fra kl: {{TIME:HH:mm}}; Til kl: \n**{{TIME:HH:mm:ss}}:** {{value:Hvem hvor hva (første beskrivelse i ny aktivitet)}} <%tp.file.cursor(3)%>"
        },
        "insertAfter": {
          "enabled": false,
          "after": "### Fysisk utforming",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top"
        },
        "newLineCapture": {
          "enabled": true,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "wholeFile"
        }
      },
      "pathHint": [
        "Ny linje",
        "Ny aktivitet (under)"
      ],
      "parentChoiceId": "59dadd14-59d6-47cf-9bab-1159b37f766f"
    },
    {
      "choice": {
        "id": "bedaabd4-fa55-4b86-aac9-49b07d272dde",
        "name": "Ny Notatmarkør (Under) 🗒️",
        "type": "Capture",
        "command": true,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "**{{TIME:HH:mm:ss}}:** ;**{{GLOBAL_VAR:DeskriptivTagg}}:**; "
        },
        "insertAfter": {
          "enabled": false,
          "after": "### Fysisk utforming",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top"
        },
        "newLineCapture": {
          "enabled": true,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "none"
        }
      },
      "pathHint": [
        "Ny linje",
        "Ny Notatmarkør (Under) 🗒️"
      ],
      "parentChoiceId": "59dadd14-59d6-47cf-9bab-1159b37f766f"
    },
    {
      "choice": {
        "id": "8808ecb4-99ad-4c05-9802-bdff581ff9b1",
        "name": "Inline DeskriptivTagg",
        "type": "Capture",
        "command": true,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": " ;**{{GLOBAL_VAR:DeskriptivTagg}}:**; <%tp.file.cursor()%>"
        },
        "insertAfter": {
          "enabled": false,
          "after": "",
          "insertAtEnd": false,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top",
          "inline": false,
          "replaceExisting": false,
          "blankLineAfterMatchMode": "auto"
        },
        "newLineCapture": {
          "enabled": false,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "wholeFile"
        }
      },
      "pathHint": [
        "Ny linje",
        "Inline DeskriptivTagg"
      ],
      "parentChoiceId": "59dadd14-59d6-47cf-9bab-1159b37f766f"
    },
    {
      "choice": {
        "id": "160ecfcd-046b-4ba6-84ba-2e076954bf59",
        "name": "Ny deskriptiv (Under)",
        "type": "Capture",
        "command": true,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "**{{TIME:HH:mm:ss}}:** "
        },
        "insertAfter": {
          "enabled": false,
          "after": "### Fysisk utforming",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top"
        },
        "newLineCapture": {
          "enabled": true,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "wholeFile"
        },
        "isDndShadowItem": true
      },
      "pathHint": [
        "Ny linje",
        "Ny deskriptiv (Under)"
      ],
      "parentChoiceId": "59dadd14-59d6-47cf-9bab-1159b37f766f"
    },
    {
      "choice": {
        "id": "01be70cd-ace7-4dcc-a60f-7876a0642097",
        "name": "Spørsmålformat",
        "type": "Capture",
        "command": false,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "> **{{VALUE:Spørsmål til senere (trenger ikke spm.tegn)}}?**\n> \n"
        },
        "insertAfter": {
          "enabled": true,
          "after": "## Spørsmål",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top",
          "inline": false,
          "replaceExisting": false,
          "blankLineAfterMatchMode": "auto"
        },
        "newLineCapture": {
          "enabled": false,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "none"
        }
      },
      "pathHint": [
        "Div Format",
        "Spørsmålformat"
      ],
      "parentChoiceId": "cff3180e-2e4a-4d1d-83f6-03910b5c2bea"
    },
    {
      "choice": {
        "id": "7c0a8932-eeed-437a-97af-b05834b5e3ae",
        "name": "Info-Format",
        "type": "Capture",
        "command": false,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "> {{VALUE:Ansatte informerer før/under/etter (med klokkeslett)}} ({{TIME}})\n"
        },
        "insertAfter": {
          "enabled": true,
          "after": "## Informasjon fra ansatte",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top",
          "inline": false,
          "replaceExisting": false,
          "blankLineAfterMatchMode": "auto"
        },
        "newLineCapture": {
          "enabled": false,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "none"
        }
      },
      "pathHint": [
        "Div Format",
        "Info-Format"
      ],
      "parentChoiceId": "cff3180e-2e4a-4d1d-83f6-03910b5c2bea"
    },
    {
      "choice": {
        "id": "e77ef54c-726e-4815-9408-89080a981810",
        "name": "Notat-tagg Format",
        "type": "Capture",
        "command": false,
        "appendLink": false,
        "captureTo": "",
        "captureToActiveFile": true,
        "captureToCanvasNodeId": "",
        "activeFileWritePosition": "cursor",
        "createFileIfItDoesntExist": {
          "enabled": false,
          "createWithTemplate": false,
          "template": ""
        },
        "format": {
          "enabled": true,
          "format": "#{{GLOBAL_VAR:NoteTagg}} {{VALUE:Notat:}} ({{time}})\n"
        },
        "insertAfter": {
          "enabled": true,
          "after": "## Mine notater",
          "insertAtEnd": true,
          "considerSubsections": false,
          "createIfNotFound": false,
          "createIfNotFoundLocation": "top",
          "inline": false,
          "replaceExisting": false,
          "blankLineAfterMatchMode": "auto"
        },
        "newLineCapture": {
          "enabled": false,
          "direction": "below"
        },
        "prepend": false,
        "task": false,
        "openFile": false,
        "fileOpening": {
          "location": "tab",
          "direction": "vertical",
          "mode": "default",
          "focus": true
        },
        "templater": {
          "afterCapture": "none"
        }
      },
      "pathHint": [
        "Div Format",
        "Notat-tagg Format"
      ],
      "parentChoiceId": "cff3180e-2e4a-4d1d-83f6-03910b5c2bea"
    }
  ],
  "assets": []
}
```
