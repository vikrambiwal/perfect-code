# Change Log

All notable changes to the "perfect-code" extension will be documented in this file.

[![v1.0.1](https://img.shields.io/badge/Latest_release-v1.0.1-green.svg?style=flat)](./changelog/v1_0_1.md)

### Release with following extension:

Extension Name

```js
React Native Tools 0.6.11
```

```
vsmobile.vscode-react-native@0.6.11
```

[![v1.0.0](https://img.shields.io/badge/Release-v1.0.0-green.svg?style=flat)](./changelog/v1_0_0.md)

### Initial release with following extension:

Extension Name

```js
AdonisJS 1.0.2
Atom Keymap 3.0.4
Auto close Tag 0.5.6
Auto Complete Tag 0.0.2
Auto Rename Tag 0.0.15
Babel JavaScript 0.0.17
C/C++ 0.17.5
change-case 1.0.0
Code Runner 0.9.3
Code Spell Checker 1.6.10
Color Highlight 2.3.0
Copy Relative Path 0.0.2
Debugger For Chrome 4.6.0
DotENV 1.0.1
Edge template Support 0.2.0
Git Blame 2.4.2
Material Icon Theme 3.5.0
Node Debug 1.24.2
Path Intellisense 1.4.2
Prettier - Code formatter 1.5.0
Rainbow Brackets 0.0.6
React Native Snippet 0.4.3
Solarized Espresso Soda 3.0.0
TODO Highlight 0.5.12
```

Extension detail: `code --list-extensions --show-versions`

```
2gua.rainbow-brackets@0.0.6
alexdima.copy-relative-path@0.0.2
brofox86.theme-espresso-soda-solarized@3.0.0
christian-kohler.path-intellisense@1.4.2
dbaeumer.vscode-eslint@1.4.12
esbenp.prettier-vscode@1.5.0
formulahendry.auto-close-tag@0.5.6
formulahendry.auto-complete-tag@0.0.2
formulahendry.auto-rename-tag@0.0.15
formulahendry.code-runner@0.9.3
Hridoy.adonisjs-snippets@1.0.2
jundat95.react-native-snippet@0.4.3
luongnd.edge@0.2.0
mgmcdermott.vscode-language-babel@0.0.17
mikestead.dotenv@1.0.1
ms-vscode.atom-keybindings@3.0.4
ms-vscode.cpptools@0.17.5
ms-vscode.node-debug2@1.24.2
msjsdiag.debugger-for-chrome@4.6.0
naumovs.color-highlight@2.3.0
PKief.material-icon-theme@3.5.0
streetsidesoftware.code-spell-checker@1.6.10
waderyan.gitblame@2.4.2
wayou.vscode-todo-highlight@0.5.12
wmaurer.change-case@1.0.0
```

### User Setting (VSCode -> Preferences -> Settings -> User Settings)

```json
{
	"window.zoomLevel": 0,
	"atomKeymap.promptV3Features": true,
	"editor.formatOnPaste": false,
	"editor.formatOnSave": true,
	"prettier.printWidth": 120,
	"prettier.useTabs": true,
	"prettier.singleQuote": true,
	"cSpell.ignoreWords": ["punchh", "reactotron", "proto", "props", "reactnative", "gaurav", "sharma"],
	"editor.renderWhitespace": "boundary",
	"editor.insertSpaces": false,
	"editor.rulers": [120],
	"search.useIgnoreFiles": false,
	"search.quickOpen.includeSymbols": false,
	"search.exclude": {
		"**/node_modules": false,
		"**/bower_components": true
	},
	"workbench.editor.enablePreviewFromQuickOpen": false,
	"explorer.confirmDragAndDrop": false,
	"extensions.ignoreRecommendations": false,
	"explorer.confirmDelete": false,
	"search.location": "sidebar",
	"emmet.includeLanguages": {
		"vue-html": "html",
		"edge": "javascriptreact"
	},
	"workbench.startupEditor": "welcomePage",
	"launch": {
		"version": "0.2.0",
		"configurations": [
			{
				"name": "Debug react native",
				"program": "${workspaceRoot}/.vscode/launchReactNative.js",
				"type": "reactnative",
				"request": "attach",
				"sourceMaps": true,
				"outDir": "${workspaceRoot}/.vscode/.react"
			},
			{
				"type": "node",
				"request": "launch",
				"name": "debug node",
				"program": "${file}"
			}
		]
	},
	"workbench.iconTheme": "material-icon-theme",
	"workbench.colorTheme": "Solarized Espresso Soda"
}
```

### `Keybindings.json` shortcuts (VSCode -> Preferences -> Keyboard Shortcuts -> [edit] Keybindings.json)

```json
[
	{
		"key": "cmd+k",
		"command": "workbench.debug.panel.action.clearReplAction",
		"when": "inDebugRepl"
	},
	{
		"key": "cmd+j",
		"command": "workbench.action.togglePanel"
	},
	{
		"key": "cmd+j",
		"command": "-workbench.action.togglePanel"
	}
]
```

### Code snippets (VSCode -> Preferences -> User Snippets -> New Global Snippets file)

```json
{
	"JSON Print": {
		"prefix": "json",
		"scope": "javascript,typescript",
		"body": "JSON.stringify(${1:object}, null, 2)"
	},
	"Import Print": {
		"prefix": "imt",
		"body": "import ${1:module} from '${1:module}';"
	},
	"Export stmt": {
		"prefix": "mex",
		"body": ["module.exports = {", "${1:export}", "};"]
	}
}
```
