# Configurações do VSCode - [Luiz Freitas](https://luiz-freitas.web.app/)

Estas são as configurações que gosto de usar, alguns plugins, fontes...

## Plugins:

`Tabnine`: Autocomplete para diversas linguagens;<br>
`Reactjs code snippets`: Auxiliar autocomplete para React - [Ver exemplos](https://marketplace.visualstudio.com/items?itemName=xabikos.ReactSnippets)<br>
`Color Highlight`: Mostra a cor exata de todos RGB’s ou HEX;<br>
`DotEnv`: Suporte à sintaxe .env;<br>
`Dracula Official`: Tema escuro;<br>
`EditorConfig`: Padronizar quebra de linha, indentação, espaços e tabs entre desenvolvedores de um mesmo projeto;<br>
`ESLint`: Padronizar código;<br>
`Markdown All in One`: Escrever e ler Markdown;<br>
`Material Icon Theme`: Exibir os ícones de acordo com a linguagem utilizada na sidebar


## settings.json:

```
  {
    // Configura tamanho e família da fonte
    "editor.fontSize":16,
    "editor.lineHeight":24,
    "editor.fontFamily":"Fira Code",
    "editor.fontLigatures":true,
    "terminal.integrated.fontFamily":"Droid Sans Mono, monospace, Droid Sans Fallback",
    "terminal.integrated.fontSize":14,
    // Aplica linhas verticais para lembrar de quebrar linha em códigos muito grandes
    "editor.rulers": [
        80,
        120
    ],
    // Aplica um sinal visual na esquerda da linha selecionada
    "editor.renderLineHighlight":"gutter",

    "files.associations": {
        ".env*": "dotenv"
    },
    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope": "keyword.other.dotenv",
                "settings": {
                    "foreground": "#FF000000"
                }
            }
        ]
    },
    // Define o tema do VSCode
    "workbench.colorTheme":"Omni",
    // Define o tema dos ícones na sidebar
    "workbench.iconTheme":"material-icon-theme",
    "tabnine.experimentalAutoImports": true,
    "git.enableSmartCommit": true,
    "git.autofetch": true,
    "git.confirmSync": false,

     //Prettier
     "editor.formatOnSave": true,
     "editor.codeActionsOnSave": {
        "source.fixAll.eslint": "explicit"
     },
     "[typescript]": {
        "editor.defaultFormatter": "vscode.typescript-language-features"
    },
    "typescript.updateImportsOnFileMove.enabled": "always",
    "javascript.updateImportsOnFileMove.enabled": "always"
  }
```
