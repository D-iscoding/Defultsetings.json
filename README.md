# Defultsetings.json

{
	// If this setting is false, no telemetry will be sent regardless of the new setting's value. Deprecated due to being combined into the `telemetry.telemetryLevel` setting.
	// Enable crash reports to be collected. This helps us improve stability. 
	// This option requires restart to take effect.
	"telemetry.enableCrashReporter": true,

	// If this setting is false, no telemetry will be sent regardless of the new setting's value. Deprecated in favor of the `telemetry.telemetryLevel` setting.
	// Enable diagnostic data to be collected. This helps us to better understand how Visual Studio Code is performing and where improvements need to be made. [Read more](https://go.microsoft.com/fwlink/?LinkId=521839) about what we collect and our privacy statement.
	"telemetry.enableTelemetry": true,

	// 
	// Controls Visual Studio Code telemetry, first-party extension telemetry, and participating third-party extension telemetry. Some third party extensions might not respect this setting. Consult the specific extension's documentation to be sure. Telemetry helps us better understand how Visual Studio Code is performing, where improvements need to be made, and how features are being used. Read more about the [data we collect](https://aka.ms/vscode-telemetry) and our [privacy statement](https://go.microsoft.com/fwlink/?LinkId=521839). A full restart of the application is necessary for crash reporting changes to take effect.
	// 
	// &nbsp;
	// 
	// The following table outlines the data sent with each setting:
	// 
	// |       | Crash Reports | Error Telemetry | Usage Data |
	// |:------|:---------------------:|:---------------:|:--------------:|
	// | all   |            ✓          |        ✓        |        ✓       |
	// | error |            ✓          |        ✓        |        -       |
	// | crash |            ✓          |        -        |        -       |
	// | off   |            -          |        -        |        -       |
	// 
	// 
	// &nbsp;
	// 
	// ****Note:*** If this setting is 'off', no telemetry will be sent regardless of other telemetry settings. If this setting is set to anything except 'off' and telemetry is disabled with deprecated settings, no telemetry will be sent.*
	// 
	//  - all: Sends usage data, errors, and crash reports.
	//  - error: Sends general error telemetry and crash reports.
	//  - crash: Sends OS level crash reports.
	//  - off: Disables all product telemetry.
	"telemetry.telemetryLevel": "all",

	// Controls whether the editor shows CodeLens.
	"diffEditor.codeLens": false,

	// 
	//  - legacy: Uses the legacy diffing algorithm.
	//  - advanced: Uses the advanced diffing algorithm.
	"diffEditor.diffAlgorithm": "advanced",

	// Controls whether the diff editor shows empty decorations to see where characters got inserted or deleted.
	"diffEditor.experimental.showEmptyDecorations": true,

	// Controls whether the diff editor should show detected code moves.
	"diffEditor.experimental.showMoves": false,

	// If enabled and the editor uses the inline view, word changes are rendered inline.
	"diffEditor.experimental.useTrueInlineView": false,

	// Controls how many lines are used as context when comparing unchanged regions.
	"diffEditor.hideUnchangedRegions.contextLineCount": 3,

	// Controls whether the diff editor shows unchanged regions.
	"diffEditor.hideUnchangedRegions.enabled": false,

	// Controls how many lines are used as a minimum for unchanged regions.
	"diffEditor.hideUnchangedRegions.minimumLineCount": 3,

	// Controls how many lines are used for unchanged regions.
	"diffEditor.hideUnchangedRegions.revealLineCount": 20,

	// When enabled, the diff editor ignores changes in leading or trailing whitespace.
	"diffEditor.ignoreTrimWhitespace": true,

	// Timeout in milliseconds after which diff computation is cancelled. Use 0 for no timeout.
	"diffEditor.maxComputationTime": 5000,

	// Maximum file size in MB for which to compute diffs. Use 0 for no limit.
	"diffEditor.maxFileSize": 50,

	// When enabled, the diff editor shows a special gutter for revert and stage actions.
	"diffEditor.renderGutterMenu": true,

	// Controls whether the diff editor shows +/- indicators for added/removed changes.
	"diffEditor.renderIndicators": true,

	// When enabled, the diff editor shows arrows in its glyph margin to revert changes.
	"diffEditor.renderMarginRevertIcon": true,

	// Controls whether the diff editor shows the diff side by side or inline.
	"diffEditor.renderSideBySide": true,

	// If the diff editor width is smaller than this value, the inline view is used.
	"diffEditor.renderSideBySideInlineBreakpoint": 900,

	// If enabled and the editor width is too small, the inline view is used.
	"diffEditor.useInlineViewWhenSpaceIsLimited": true,

	// 
	//  - off: Lines will never wrap.
	//  - on: Lines will wrap at the viewport width.
	//  - inherit: Lines will wrap according to the `editor.wordWrap` setting.
	"diffEditor.wordWrap": "inherit",

	// Controls whether suggestions should be accepted on commit characters. For example, in JavaScript, the semi-colon (`;`) can be a commit character that accepts a suggestion and types that character.
	"editor.acceptSuggestionOnCommitCharacter": true,

	// Controls whether suggestions should be accepted on `Enter`, in addition to `Tab`. Helps to avoid ambiguity between inserting new lines or accepting suggestions.
	//  - on
	//  - smart: Only accept a suggestion with `Enter` when it makes a textual change.
	//  - off
	"editor.acceptSuggestionOnEnter": "on",

	// Controls the number of lines in the editor that can be read out by a screen reader at once. When we detect a screen reader we automatically set the default to be 500. Warning: this has a performance implication for numbers larger than the default.
	"editor.accessibilityPageSize": 500,

	// Controls if the UI should run in a mode where it is optimized for screen readers.
	//  - auto: Use platform APIs to detect when a Screen Reader is attached.
	//  - on: Optimize for usage with a Screen Reader.
	//  - off: Assume a screen reader is not attached.
	"editor.accessibilitySupport": "auto",

	// Controls whether the editor should automatically close brackets after the user adds an opening bracket.
	//  - always
	//  - languageDefined: Use language configurations to determine when to autoclose brackets.
	//  - beforeWhitespace: Autoclose brackets only when the cursor is to the left of whitespace.
	//  - never
	"editor.autoClosingBrackets": "languageDefined",

	// Controls whether the editor should automatically close comments after the user adds an opening comment.
	//  - always
	//  - languageDefined: Use language configurations to determine when to autoclose comments.
	//  - beforeWhitespace: Autoclose comments only when the cursor is to the left of whitespace.
	//  - never
	"editor.autoClosingComments": "languageDefined",

	// Controls whether the editor should remove adjacent closing quotes or brackets when deleting.
	//  - always
	//  - auto: Remove adjacent closing quotes or brackets only if they were automatically inserted.
	//  - never
	"editor.autoClosingDelete": "auto",

	// Controls whether the editor should type over closing quotes or brackets.
	//  - always
	//  - auto: Type over closing quotes or brackets only if they were automatically inserted.
	//  - never
	"editor.autoClosingOvertype": "auto",

	// Controls whether the editor should automatically close quotes after the user adds an opening quote.
	//  - always
	//  - languageDefined: Use language configurations to determine when to autoclose quotes.
	//  - beforeWhitespace: Autoclose quotes only when the cursor is to the left of whitespace.
	//  - never
	"editor.autoClosingQuotes": "languageDefined",

	// Controls whether the editor should automatically adjust the indentation when users type, paste, move or indent lines.
	//  - none: The editor will not insert indentation automatically.
	//  - keep: The editor will keep the current line's indentation.
	//  - brackets: The editor will keep the current line's indentation and honor language defined brackets.
	//  - advanced: The editor will keep the current line's indentation, honor language defined brackets and invoke special onEnterRules defined by languages.
	//  - full: The editor will keep the current line's indentation, honor language defined brackets, invoke special onEnterRules defined by languages, and honor indentationRules defined by languages.
	"editor.autoIndent": "full",

	// Controls whether the editor should automatically surround selections when typing quotes or brackets.
	//  - languageDefined: Use language configurations to determine when to automatically surround selections.
	//  - quotes: Surround with quotes but not brackets.
	//  - brackets: Surround with brackets but not quotes.
	//  - never
	"editor.autoSurround": "languageDefined",

	// Controls whether bracket pair colorization is enabled or not. Use `workbench.colorCustomizations` to override the bracket highlight colors.
	"editor.bracketPairColorization.enabled": true,

	// Controls whether each bracket type has its own independent color pool.
	"editor.bracketPairColorization.independentColorPoolPerBracketType": false,

	// Enable triggering `editor.codeActionsOnSave#` when `#files.autoSave` is set to `afterDelay`. Code Actions must be set to `always` to be triggered for window and focus changes.
	"editor.codeActions.triggerOnFocusChange": false,

	// Run Code Actions for the editor on save. Code Actions must be specified and the editor must not be shutting down. When `files.autoSave` is set to `afterDelay`, Code Actions will only be run when the file is saved explicitly. Example: `"source.organizeImports": "explicit" `
	"editor.codeActionsOnSave": {},

	// Enable/disable showing nearest Quick Fix within a line when not currently on a diagnostic.
	"editor.codeActionWidget.includeNearbyQuickFixes": true,

	// Enable/disable showing group headers in the Code Action menu.
	"editor.codeActionWidget.showHeaders": true,

	// Controls whether the editor shows CodeLens.
	"editor.codeLens": true,

	// Controls the font family for CodeLens.
	"editor.codeLensFontFamily": "",

	// Controls the font size in pixels for CodeLens. When set to 0, 90% of `editor.fontSize` is used.
	"editor.codeLensFontSize": 0,

	// Controls whether the editor should render the inline color decorators and color picker.
	"editor.colorDecorators": true,

	// Controls the condition to make a color picker appear from a color decorator.
	//  - clickAndHover: Make the color picker appear both on click and hover of the color decorator
	//  - hover: Make the color picker appear on hover of the color decorator
	//  - click: Make the color picker appear on click of the color decorator
	"editor.colorDecoratorsActivatedOn": "clickAndHover",

	// Controls the max number of color decorators that can be rendered in an editor at once.
	"editor.colorDecoratorsLimit": 500,

	// Enable that the selection with the mouse and keys is doing column selection.
	"editor.columnSelection": false,

	// Controls if empty lines should be ignored with toggle, add or remove actions for line comments.
	"editor.comments.ignoreEmptyLines": true,

	// Controls whether a space character is inserted when commenting.
	"editor.comments.insertSpace": true,

	// Controls whether syntax highlighting should be copied into the clipboard.
	"editor.copyWithSyntaxHighlighting": true,

	// Control the cursor animation style.
	"editor.cursorBlinking": "blink",

	// Controls whether the smooth caret animation should be enabled.
	//  - off: Smooth caret animation is disabled.
	//  - explicit: Smooth caret animation is enabled only when the user moves the cursor with an explicit gesture.
	//  - on: Smooth caret animation is always enabled.
	"editor.cursorSmoothCaretAnimation": "off",

	// Controls the cursor style in insert input mode.
	"editor.cursorStyle": "line",

	// Controls the minimal number of visible leading lines (minimum 0) and trailing lines (minimum 1) surrounding the cursor. Known as 'scrollOff' or 'scrollOffset' in some other editors.
	"editor.cursorSurroundingLines": 0,

	// Controls when `editor.cursorSurroundingLines` should be enforced.
	//  - default: `cursorSurroundingLines` is enforced only when triggered via the keyboard or API.
	//  - all: `cursorSurroundingLines` is enforced always.
	"editor.cursorSurroundingLinesStyle": "default",

	// Controls the width of the cursor when `editor.cursorStyle` is set to `line`.
	"editor.cursorWidth": 0,

	// Controls whether inline color decorations should be shown using the default document color provider.
	//  - auto: Show default color decorators only when no extension provides colors decorators.
	//  - always: Always show default color decorators.
	//  - never: Never show default color decorators.
	"editor.defaultColorDecorators": "auto",

	// Defines a default folding range provider that takes precedence over all other folding range providers. Must be the identifier of an extension contributing a folding range provider.
	//  - null: All active folding range providers
	//  - formulahendry.auto-rename-tag: Auto rename paired HTML/XML tag
	//  - formulahendry.code-runner: Run C, C++, Java, JS, PHP, Python, Perl, Ruby, Go, Lua, Groovy, PowerShell, CMD, BASH, F#, C#, VBScript, TypeScript, CoffeeScript, Scala, Swift, Julia, Crystal, OCaml, R, AppleScript, Elixir, VB.NET, Clojure, Haxe, Obj-C, Rust, Racket, Scheme, AutoHotkey, AutoIt, Kotlin, Dart, Pascal, Haskell, Nim, D, Lisp, Kit, V, SCSS, Sass, CUDA, Less, Fortran, Ring, Standard ML, Zig, Mojo, Erlang, SPWN, Pkl, Gleam
	//  - vscode.css-language-features: Provides rich language support for CSS, LESS and SCSS files.
	//  - vscode.html-language-features: Provides rich language support for HTML and Handlebar files
	//  - solnurkarim.html-to-css-autocompletion: Provides completion suggestions for classes and ids from markup documents to stylesheets.
	//  - vscode.json-language-features: Provides rich language support for JSON files.
	//  - vscode.markdown-language-features: Provides rich language support for Markdown.
	//  - vscode.markdown-math: Adds math support to Markdown in notebooks.
	//  - vscode.php-language-features: Provides rich language support for PHP files.
	//  - ms-python.python: Python language support with extension access points for IntelliSense (Pylance), Debugging (Python Debugger), linting, formatting, refactoring, unit tests, and more.
	//  - vscode.typescript-language-features: Provides rich language support for JavaScript and TypeScript.
	//  - ecmel.vscode-html-css: CSS Intellisense for HTML
	//  - ms-python.vscode-pylance: A performant, feature-rich language server for Python in VS Code
	//  - BracketPairColorDLW.bracket-pair-color-dlw: Quickly 'Bracket Pair Color DLW' setting with a simple command
	//  - vscode.configuration-editing: Provides capabilities (advanced IntelliSense, auto-fixing) in configuration files like settings, launch, and extension recommendation files.
	//  - Wscats.cors-browser: 🚀Preview file in your default browser
	//  - vscode.debug-auto-launch: Helper for auto-attach feature when node-debug extensions are not active.
	//  - vscode.debug-server-ready: Open URI in browser if server under debugging is ready.
	//  - ms-python.debugpy: Python Debugger extension using debugpy.
	//  - atariq11700.debugpy-old: Python Debugger extension using `debugpy` for python <= 3.6.
	//  - vscode.emmet: Emmet support for VS Code
	//  - vscode.extension-editing: Provides linting capabilities for authoring extensions.
	//  - vscode.git: Git SCM Integration
	//  - vscode.git-base: Git static contributions and pickers.
	//  - vscode.github: GitHub features for VS Code
	//  - vscode.github-authentication: GitHub Authentication Provider
	//  - vscode.grunt: Extension to add Grunt capabilities to VS Code.
	//  - vscode.gulp: Extension to add Gulp capabilities to VSCode.
	//  - bianxianyang.htmlplay: html/js/css playground
	//  - vscode.ipynb: Provides basic support for opening and reading Jupyter's .ipynb notebook files
	//  - vscode.jake: Extension to add Jake capabilities to VS Code.
	//  - ms-vscode.js-debug: An extension for debugging Node.js programs and Chrome.
	//  - ms-vscode.js-debug-companion: Companion extension to js-debug that provides capability for remote debugging
	//  - ms-vscode.js-debug-nightly: An extension for debugging Node.js programs and Chrome.
	//  - ritwickdey.LiveServer: Launch a development local Server with live reload feature for static & dynamic pages
	//  - vscode.media-preview: Provides VS Code's built-in previews for images, audio, and video
	//  - vscode.merge-conflict: Highlighting and commands for inline merge conflicts.
	//  - vscode.microsoft-authentication: Microsoft authentication provider
	//  - vscode.npm: Extension to add task support for npm scripts.
	//  - christian-kohler.npm-intellisense: Visual Studio Code plugin that autocompletes npm modules in import statements
	//  - techer.open-in-browser: This allows you to open the current file in your default browser or application.
	//  - esbenp.prettier-vscode: Code formatter using prettier
	//  - vscode.references-view: Reference Search results as separate, stable view in the sidebar
	//  - vscode.search-result: Provides syntax highlighting and language features for tabbed search results.
	//  - vscode.simple-browser: A very basic built-in webview for displaying web content.
	//  - vscode.terminal-suggest: Extension to add terminal completions for zsh, bash, and fish terminals.
	//  - vscode.tunnel-forwarding: Allows forwarding local ports to be accessible over the internet.
	//  - ms-vscode.vscode-js-profile-table: Text visualizer for profiles taken from the JavaScript debugger
	//  - GitHub.vscode-pull-request-github: Pull Request and Issue Provider for GitHub
	//  - standard.vscode-standard: Visual Studio Code extension for JavaScript Standard Style with automatic fixing.
	//  - vitaliymaz.vscode-svg-previewer: Show SVG preview to the side panel
	"editor.defaultFoldingRangeProvider": null,

	// Defines a default formatter which takes precedence over all other formatter settings. Must be the identifier of an extension contributing a formatter.
	//  - null: None
	//  - formulahendry.auto-rename-tag: Auto rename paired HTML/XML tag
	//  - formulahendry.code-runner: Run C, C++, Java, JS, PHP, Python, Perl, Ruby, Go, Lua, Groovy, PowerShell, CMD, BASH, F#, C#, VBScript, TypeScript, CoffeeScript, Scala, Swift, Julia, Crystal, OCaml, R, AppleScript, Elixir, VB.NET, Clojure, Haxe, Obj-C, Rust, Racket, Scheme, AutoHotkey, AutoIt, Kotlin, Dart, Pascal, Haskell, Nim, D, Lisp, Kit, V, SCSS, Sass, CUDA, Less, Fortran, Ring, Standard ML, Zig, Mojo, Erlang, SPWN, Pkl, Gleam
	//  - vscode.css-language-features: Provides rich language support for CSS, LESS and SCSS files.
	//  - vscode.html-language-features: Provides rich language support for HTML and Handlebar files
	//  - solnurkarim.html-to-css-autocompletion: Provides completion suggestions for classes and ids from markup documents to stylesheets.
	//  - vscode.json-language-features: Provides rich language support for JSON files.
	//  - vscode.markdown-language-features: Provides rich language support for Markdown.
	//  - vscode.markdown-math: Adds math support to Markdown in notebooks.
	//  - vscode.php-language-features: Provides rich language support for PHP files.
	//  - esbenp.prettier-vscode: Code formatter using prettier
	//  - ms-python.python: Python language support with extension access points for IntelliSense (Pylance), Debugging (Python Debugger), linting, formatting, refactoring, unit tests, and more.
	//  - vscode.typescript-language-features: Provides rich language support for JavaScript and TypeScript.
	//  - ecmel.vscode-html-css: CSS Intellisense for HTML
	//  - ms-python.vscode-pylance: A performant, feature-rich language server for Python in VS Code
	//  - standard.vscode-standard: Visual Studio Code extension for JavaScript Standard Style with automatic fixing.
	//  - BracketPairColorDLW.bracket-pair-color-dlw: Quickly 'Bracket Pair Color DLW' setting with a simple command
	//  - vscode.configuration-editing: Provides capabilities (advanced IntelliSense, auto-fixing) in configuration files like settings, launch, and extension recommendation files.
	//  - Wscats.cors-browser: 🚀Preview file in your default browser
	//  - vscode.debug-auto-launch: Helper for auto-attach feature when node-debug extensions are not active.
	//  - vscode.debug-server-ready: Open URI in browser if server under debugging is ready.
	//  - ms-python.debugpy: Python Debugger extension using debugpy.
	//  - atariq11700.debugpy-old: Python Debugger extension using `debugpy` for python <= 3.6.
	//  - vscode.emmet: Emmet support for VS Code
	//  - vscode.extension-editing: Provides linting capabilities for authoring extensions.
	//  - vscode.git: Git SCM Integration
	//  - vscode.git-base: Git static contributions and pickers.
	//  - vscode.github: GitHub features for VS Code
	//  - vscode.github-authentication: GitHub Authentication Provider
	//  - vscode.grunt: Extension to add Grunt capabilities to VS Code.
	//  - vscode.gulp: Extension to add Gulp capabilities to VSCode.
	//  - bianxianyang.htmlplay: html/js/css playground
	//  - vscode.ipynb: Provides basic support for opening and reading Jupyter's .ipynb notebook files
	//  - vscode.jake: Extension to add Jake capabilities to VS Code.
	//  - ms-vscode.js-debug: An extension for debugging Node.js programs and Chrome.
	//  - ms-vscode.js-debug-companion: Companion extension to js-debug that provides capability for remote debugging
	//  - ms-vscode.js-debug-nightly: An extension for debugging Node.js programs and Chrome.
	//  - ritwickdey.LiveServer: Launch a development local Server with live reload feature for static & dynamic pages
	//  - vscode.media-preview: Provides VS Code's built-in previews for images, audio, and video
	//  - vscode.merge-conflict: Highlighting and commands for inline merge conflicts.
	//  - vscode.microsoft-authentication: Microsoft authentication provider
	//  - vscode.npm: Extension to add task support for npm scripts.
	//  - christian-kohler.npm-intellisense: Visual Studio Code plugin that autocompletes npm modules in import statements
	//  - techer.open-in-browser: This allows you to open the current file in your default browser or application.
	//  - vscode.references-view: Reference Search results as separate, stable view in the sidebar
	//  - vscode.search-result: Provides syntax highlighting and language features for tabbed search results.
	//  - vscode.simple-browser: A very basic built-in webview for displaying web content.
	//  - vscode.terminal-suggest: Extension to add terminal completions for zsh, bash, and fish terminals.
	//  - vscode.tunnel-forwarding: Allows forwarding local ports to be accessible over the internet.
	//  - ms-vscode.vscode-js-profile-table: Text visualizer for profiles taken from the JavaScript debugger
	//  - GitHub.vscode-pull-request-github: Pull Request and Issue Provider for GitHub
	//  - vitaliymaz.vscode-svg-previewer: Show SVG preview to the side panel
	"editor.defaultFormatter": null,

	// Controls whether the Go to Definition mouse gesture always opens the peek widget.
	"editor.definitionLinkOpensInPeek": false,

	// Controls whether `editor.tabSize#` and `#editor.insertSpaces` will be automatically detected when a file is opened based on the file contents.
	"editor.detectIndentation": true,

	// Controls whether the editor should allow moving selections via drag and drop.
	"editor.dragAndDrop": true,

	// Controls whether you can drag and drop a file into a text editor by holding down the `Shift` key (instead of opening the file in an editor).
	"editor.dropIntoEditor.enabled": true,

	// Configures the preferred type of edit to use when dropping content.
	// 
	// This is an ordered list of edit kinds. The first available edit of a preferred kind will be used.
	"editor.dropIntoEditor.preferences": [],

	// Controls if a widget is shown when dropping files into the editor. This widget lets you control how the file is dropped.
	//  - afterDrop: Show the drop selector widget after a file is dropped into the editor.
	//  - never: Never show the drop selector widget. Instead the default drop provider is always used.
	"editor.dropIntoEditor.showDropSelector": "afterDrop",

	// Controls whether copying without a selection copies the current line.
	"editor.emptySelectionClipboard": true,

	// Controls whether the tokenization should happen asynchronously on a web worker.
	"editor.experimental.asyncTokenization": true,

	// Controls whether async tokenization should be logged. For debugging only.
	"editor.experimental.asyncTokenizationLogging": false,

	// Controls whether async tokenization should be verified against legacy background tokenization. Might slow down tokenization. For debugging only.
	"editor.experimental.asyncTokenizationVerification": false,

	// Controls whether tree sitter parsing should be turned on for specific languages. This will take precedence over `editor.experimental.treeSitterTelemetry` for the specified languages.
	"editor.experimental.preferTreeSitter": [],

	// Controls whether tree sitter parsing should be turned on and telemetry collected. Setting `editor.experimental.preferTreeSitter` for specific languages will take precedence.
	"editor.experimental.treeSitterTelemetry": false,

	// Sets whether the new experimental edit context should be used instead of the text area.
	"editor.experimentalEditContextEnabled": false,

	// Controls whether to use the experimental GPU acceleration to render the editor.
	//  - off: Use regular DOM-based rendering.
	//  - on: Use GPU acceleration.
	"editor.experimentalGpuAcceleration": "off",

	// Controls whether whitespace is rendered with a new, experimental method.
	//  - svg: Use a new rendering method with svgs.
	//  - font: Use a new rendering method with font characters.
	//  - off: Use the stable rendering method.
	"editor.experimentalWhitespaceRendering": "svg",

	// Scrolling speed multiplier when pressing `Alt`.
	"editor.fastScrollSensitivity": 5,

	// Controls whether the Find Widget should add extra lines on top of the editor. When true, you can scroll beyond the first line when the Find Widget is visible.
	"editor.find.addExtraSpaceOnTop": true,

	// Controls the condition for turning on Find in Selection automatically.
	//  - never: Never turn on Find in Selection automatically (default).
	//  - always: Always turn on Find in Selection automatically.
	//  - multiline: Turn on Find in Selection automatically when multiple lines of content are selected.
	"editor.find.autoFindInSelection": "never",

	// Controls whether the cursor should jump to find matches while typing.
	"editor.find.cursorMoveOnType": true,

	// Controls how the find widget history should be stored
	//  - never: Do not store search history from the find widget.
	//  - workspace: Store search history across the active workspace
	"editor.find.history": "workspace",

	// Controls whether the search automatically restarts from the beginning (or the end) when no further matches can be found.
	"editor.find.loop": true,

	// Controls how the replace widget history should be stored
	//  - never: Do not store history from the replace widget.
	//  - workspace: Store replace history across the active workspace
	"editor.find.replaceHistory": "workspace",

	// Controls whether the search string in the Find Widget is seeded from the editor selection.
	//  - never: Never seed search string from the editor selection.
	//  - always: Always seed search string from the editor selection, including word at cursor position.
	//  - selection: Only seed search string from the editor selection.
	"editor.find.seedSearchStringFromSelection": "always",

	// Controls whether the editor has code folding enabled.
	"editor.folding": true,

	// Controls whether the editor should highlight folded ranges.
	"editor.foldingHighlight": true,

	// Controls whether the editor automatically collapses import ranges.
	"editor.foldingImportsByDefault": false,

	// The maximum number of foldable regions. Increasing this value may result in the editor becoming less responsive when the current source has a large number of foldable regions.
	"editor.foldingMaximumRegions": 5000,

	// Controls the strategy for computing folding ranges.
	//  - auto: Use a language-specific folding strategy if available, else the indentation-based one.
	//  - indentation: Use the indentation-based folding strategy.
	"editor.foldingStrategy": "auto",

	// Controls the font family.
	"editor.fontFamily": "Consolas, 'Courier New', monospace",

	// Configures font ligatures or font features. Can be either a boolean to enable/disable ligatures or a string for the value of the CSS 'font-feature-settings' property.
	"editor.fontLigatures": false,

	// Controls the font size in pixels.
	"editor.fontSize": 14,

	// Configures font variations. Can be either a boolean to enable/disable the translation from font-weight to font-variation-settings or a string for the value of the CSS 'font-variation-settings' property.
	"editor.fontVariations": false,

	// Controls the font weight. Accepts "normal" and "bold" keywords or numbers between 1 and 1000.
	"editor.fontWeight": "normal",

	// Controls whether the editor should automatically format the pasted content. A formatter must be available and the formatter should be able to format a range in a document.
	"editor.formatOnPaste": false,

	// Format a file on save. A formatter must be available and the editor must not be shutting down. When `files.autoSave` is set to `afterDelay`, the file will only be formatted when saved explicitly.
	"editor.formatOnSave": false,

	// Controls if format on save formats the whole file or only modifications. Only applies when `editor.formatOnSave` is enabled.
	//  - file: Format the whole file.
	//  - modifications: Format modifications (requires source control).
	//  - modificationsIfAvailable: Will attempt to format modifications only (requires source control). If source control can't be used, then the whole file will be formatted.
	"editor.formatOnSaveMode": "file",

	// Controls whether the editor should automatically format the line after typing.
	"editor.formatOnType": false,

	// Controls whether the editor should render the vertical glyph margin. Glyph margin is mostly used for debugging.
	"editor.glyphMargin": true,

	// Alternative command id that is being executed when the result of 'Go to Declaration' is the current location.
	"editor.gotoLocation.alternativeDeclarationCommand": "editor.action.goToReferences",

	// Alternative command id that is being executed when the result of 'Go to Definition' is the current location.
	"editor.gotoLocation.alternativeDefinitionCommand": "editor.action.goToReferences",

	// Alternative command id that is being executed when the result of 'Go to Implementation' is the current location.
	"editor.gotoLocation.alternativeImplementationCommand": "",

	// Alternative command id that is being executed when the result of 'Go to Reference' is the current location.
	"editor.gotoLocation.alternativeReferenceCommand": "",

	// Alternative command id that is being executed when the result of 'Go to Type Definition' is the current location.
	"editor.gotoLocation.alternativeTypeDefinitionCommand": "editor.action.goToReferences",

	// This setting is deprecated, please use separate settings like 'editor.editor.gotoLocation.multipleDefinitions' or 'editor.editor.gotoLocation.multipleImplementations' instead.
	// 
	"editor.gotoLocation.multiple": null,

	// Controls the behavior the 'Go to Declaration'-command when multiple target locations exist.
	//  - peek: Show Peek view of the results (default)
	//  - gotoAndPeek: Go to the primary result and show a Peek view
	//  - goto: Go to the primary result and enable Peek-less navigation to others
	"editor.gotoLocation.multipleDeclarations": "peek",

	// Controls the behavior the 'Go to Definition'-command when multiple target locations exist.
	//  - peek: Show Peek view of the results (default)
	//  - gotoAndPeek: Go to the primary result and show a Peek view
	//  - goto: Go to the primary result and enable Peek-less navigation to others
	"editor.gotoLocation.multipleDefinitions": "peek",

	// Controls the behavior the 'Go to Implementations'-command when multiple target locations exist.
	//  - peek: Show Peek view of the results (default)
	//  - gotoAndPeek: Go to the primary result and show a Peek view
	//  - goto: Go to the primary result and enable Peek-less navigation to others
	"editor.gotoLocation.multipleImplementations": "peek",

	// Controls the behavior the 'Go to References'-command when multiple target locations exist.
	//  - peek: Show Peek view of the results (default)
	//  - gotoAndPeek: Go to the primary result and show a Peek view
	//  - goto: Go to the primary result and enable Peek-less navigation to others
	"editor.gotoLocation.multipleReferences": "peek",

	// Controls the behavior the 'Go to Type Definition'-command when multiple target locations exist.
	//  - peek: Show Peek view of the results (default)
	//  - gotoAndPeek: Go to the primary result and show a Peek view
	//  - goto: Go to the primary result and enable Peek-less navigation to others
	"editor.gotoLocation.multipleTypeDefinitions": "peek",

	// Controls whether bracket pair guides are enabled or not.
	//  - true: Enables bracket pair guides.
	//  - active: Enables bracket pair guides only for the active bracket pair.
	//  - false: Disables bracket pair guides.
	"editor.guides.bracketPairs": false,

	// Controls whether horizontal bracket pair guides are enabled or not.
	//  - true: Enables horizontal guides as addition to vertical bracket pair guides.
	//  - active: Enables horizontal guides only for the active bracket pair.
	//  - false: Disables horizontal bracket pair guides.
	"editor.guides.bracketPairsHorizontal": "active",

	// Controls whether the editor should highlight the active bracket pair.
	"editor.guides.highlightActiveBracketPair": true,

	// Controls whether the editor should highlight the active indent guide.
	//  - true: Highlights the active indent guide.
	//  - always: Highlights the active indent guide even if bracket guides are highlighted.
	//  - false: Do not highlight the active indent guide.
	"editor.guides.highlightActiveIndentation": true,

	// Controls whether the editor should render indent guides.
	"editor.guides.indentation": true,

	// Controls whether the cursor should be hidden in the overview ruler.
	"editor.hideCursorInOverviewRuler": false,

	// Prefer showing hovers above the line, if there's space.
	"editor.hover.above": true,

	// Controls the delay in milliseconds after which the hover is shown.
	"editor.hover.delay": 300,

	// Controls whether the hover is shown.
	"editor.hover.enabled": true,

	// Controls the delay in milliseconds after which the hover is hidden. Requires `editor.hover.sticky` to be enabled.
	"editor.hover.hidingDelay": 300,

	// Controls whether the hover should remain visible when mouse is moved over it.
	"editor.hover.sticky": true,

	// The number of spaces used for indentation or `"tabSize"` to use the value from `editor.tabSize#`. This setting is overridden based on the file contents when `#editor.detectIndentation` is on.
	"editor.indentSize": "tabSize",

	// Enables the inlay hints in the editor.
	//  - on: Inlay hints are enabled
	//  - onUnlessPressed: Inlay hints are showing by default and hide when holding Ctrl+Alt
	//  - offUnlessPressed: Inlay hints are hidden by default and show when holding Ctrl+Alt
	//  - off: Inlay hints are disabled
	"editor.inlayHints.enabled": "on",

	// Controls font family of inlay hints in the editor. When set to empty, the `editor.fontFamily` is used.
	"editor.inlayHints.fontFamily": "",

	// Controls font size of inlay hints in the editor. As default the `editor.fontSize` is used when the configured value is less than `5` or greater than the editor font size.
	"editor.inlayHints.fontSize": 0,

	// Maximum overall length of inlay hints, for a single line, before they get truncated by the editor. Set to `0` to never truncate
	"editor.inlayHints.maximumLength": 43,

	// Enables the padding around the inlay hints in the editor.
	"editor.inlayHints.padding": false,

	// Controls whether the accessibility hint should be provided to screen reader users when an inline completion is shown.
	"editor.inlineCompletionsAccessibilityVerbose": false,

	// Controls whether showing a suggestion will shift the code to make space for the suggestion inline.
	"editor.inlineSuggest.edits.codeShifting": true,

	// Controls whether larger suggestions can be shown side by side.
	//  - auto: Larger suggestions will show side by side if there is enough space, otherwise they will be shown bellow.
	//  - never: Larger suggestions are never shown side by side and will always be shown bellow.
	"editor.inlineSuggest.edits.renderSideBySide": "auto",

	// Controls whether to automatically show inline suggestions in the editor.
	"editor.inlineSuggest.enabled": true,

	// Controls the font family of the inline suggestions.
	"editor.inlineSuggest.fontFamily": "default",

	// Controls when to show the inline suggestion toolbar.
	//  - always: Show the inline suggestion toolbar whenever an inline suggestion is shown.
	//  - onHover: Show the inline suggestion toolbar when hovering over an inline suggestion.
	//  - never: Never show the inline suggestion toolbar.
	"editor.inlineSuggest.showToolbar": "onHover",

	// Controls how inline suggestions interact with the suggest widget. If enabled, the suggest widget is not shown automatically when inline suggestions are available.
	"editor.inlineSuggest.suppressSuggestions": false,

	// Controls whether to show syntax highlighting for inline suggestions in the editor.
	"editor.inlineSuggest.syntaxHighlightingEnabled": false,

	// Insert spaces when pressing `Tab`. This setting is overridden based on the file contents when `editor.detectIndentation` is on.
	"editor.insertSpaces": true,

	// Defines the bracket symbols that increase or decrease the indentation.
	"editor.language.brackets": null,

	// Defines the bracket pairs that are colorized by their nesting level if bracket pair colorization is enabled.
	"editor.language.colorizedBracketPairs": null,

	// Special handling for large files to disable certain memory intensive features.
	"editor.largeFileOptimizations": true,

	// Controls the letter spacing in pixels.
	"editor.letterSpacing": 0,

	// Enables the Code Action lightbulb in the editor.
	//  - off: Disable the code action menu.
	//  - onCode: Show the code action menu when the cursor is on lines with code.
	//  - on: Show the code action menu when the cursor is on lines with code or on empty lines.
	"editor.lightbulb.enabled": "onCode",

	// Controls the line height. 
	//  - Use 0 to automatically compute the line height from the font size.
	//  - Values between 0 and 8 will be used as a multiplier with the font size.
	//  - Values greater than or equal to 8 will be used as effective values.
	"editor.lineHeight": 0,

	// Controls the display of line numbers.
	//  - off: Line numbers are not rendered.
	//  - on: Line numbers are rendered as absolute number.
	//  - relative: Line numbers are rendered as distance in lines to cursor position.
	//  - interval: Line numbers are rendered every 10 lines.
	"editor.lineNumbers": "on",

	// Controls whether the editor has linked editing enabled. Depending on the language, related symbols such as HTML tags, are updated while editing.
	"editor.linkedEditing": false,

	// Controls whether the editor should detect links and make them clickable.
	"editor.links": true,

	// Highlight matching brackets.
	"editor.matchBrackets": "always",

	// Lines above this length will not be tokenized for performance reasons
	"editor.maxTokenizationLineLength": 20000,

	// Controls whether the minimap is hidden automatically.
	"editor.minimap.autohide": false,

	// Controls whether the minimap is shown.
	"editor.minimap.enabled": true,

	// Limit the width of the minimap to render at most a certain number of columns.
	"editor.minimap.maxColumn": 120,

	// Render the actual characters on a line as opposed to color blocks.
	"editor.minimap.renderCharacters": true,

	// Scale of content drawn in the minimap: 1, 2 or 3.
	"editor.minimap.scale": 1,

	// Controls the font size of section headers in the minimap.
	"editor.minimap.sectionHeaderFontSize": 9,

	// Controls the amount of space (in pixels) between characters of section header. This helps the readability of the header in small font sizes.
	"editor.minimap.sectionHeaderLetterSpacing": 1,

	// Controls whether MARK: comments are shown as section headers in the minimap.
	"editor.minimap.showMarkSectionHeaders": true,

	// Controls whether named regions are shown as section headers in the minimap.
	"editor.minimap.showRegionSectionHeaders": true,

	// Controls when the minimap slider is shown.
	"editor.minimap.showSlider": "mouseover",

	// Controls the side where to render the minimap.
	"editor.minimap.side": "right",

	// Controls the size of the minimap.
	//  - proportional: The minimap has the same size as the editor contents (and might scroll).
	//  - fill: The minimap will stretch or shrink as necessary to fill the height of the editor (no scrolling).
	//  - fit: The minimap will shrink as necessary to never be larger than the editor (no scrolling).
	"editor.minimap.size": "proportional",

	// A multiplier to be used on the `deltaX` and `deltaY` of mouse wheel scroll events.
	"editor.mouseWheelScrollSensitivity": 1,

	// Zoom the font of the editor when using mouse wheel and holding `Ctrl`.
	"editor.mouseWheelZoom": false,

	// Controls the max number of cursors that can be in an active editor at once.
	"editor.multiCursorLimit": 10000,

	// Merge multiple cursors when they are overlapping.
	"editor.multiCursorMergeOverlapping": true,

	// The modifier to be used to add multiple cursors with the mouse. The Go to Definition and Open Link mouse gestures will adapt such that they do not conflict with the [multicursor modifier](https://code.visualstudio.com/docs/editor/codebasics#_multicursor-modifier).
	//  - ctrlCmd: Maps to `Control` on Windows and Linux and to `Command` on macOS.
	//  - alt: Maps to `Alt` on Windows and Linux and to `Option` on macOS.
	"editor.multiCursorModifier": "alt",

	// Controls pasting when the line count of the pasted text matches the cursor count.
	//  - spread: Each cursor pastes a single line of the text.
	//  - full: Each cursor pastes the full text.
	"editor.multiCursorPaste": "spread",

	// Controls whether occurrences should be highlighted across open files.
	//  - off: Does not highlight occurrences.
	//  - singleFile: Highlights occurrences only in the current file.
	//  - multiFile: Experimental: Highlights occurrences across all valid open files.
	"editor.occurrencesHighlight": "singleFile",

	// Controls the delay in milliseconds after which occurrences are highlighted.
	"editor.occurrencesHighlightDelay": 250,

	// Controls the cursor style in overtype input mode.
	"editor.overtypeCursorStyle": "block",

	// Controls whether pasting should overtype.
	"editor.overtypeOnPaste": true,

	// Controls whether a border should be drawn around the overview ruler.
	"editor.overviewRulerBorder": true,

	// Controls the amount of space between the bottom edge of the editor and the last line.
	"editor.padding.bottom": 0,

	// Controls the amount of space between the top edge of the editor and the first line.
	"editor.padding.top": 0,

	// Controls whether the parameter hints menu cycles or closes when reaching the end of the list.
	"editor.parameterHints.cycle": true,

	// Enables a pop-up that shows parameter documentation and type information as you type.
	"editor.parameterHints.enabled": true,

	// Controls whether you can paste content in different ways.
	"editor.pasteAs.enabled": true,

	// Configures the preferred type of edit to use when pasting content.
	// 
	// This is an ordered list of edit kinds. The first available edit of a preferred kind will be used.
	"editor.pasteAs.preferences": [],

	// Controls if a widget is shown when pasting content in to the editor. This widget lets you control how the file is pasted.
	//  - afterPaste: Show the paste selector widget after content is pasted into the editor.
	//  - never: Never show the paste selector widget. Instead the default pasting behavior is always used.
	"editor.pasteAs.showPasteSelector": "afterPaste",

	// Controls whether to focus the inline editor or the tree in the peek widget.
	//  - tree: Focus the tree when opening peek
	//  - editor: Focus the editor when opening peek
	"editor.peekWidgetDefaultFocus": "tree",

	// Controls whether suggestions should automatically show up while typing. This can be controlled for typing in comments, strings, and other code. Quick suggestion can be configured to show as ghost text or with the suggest widget. Also be aware of the `editor.suggestOnTriggerCharacters`-setting which controls if suggestions are triggered by special characters.
	"editor.quickSuggestions": {
		"other": "on",
		"comments": "off",
		"strings": "off"
	},

	// Controls the delay in milliseconds after which quick suggestions will show up.
	"editor.quickSuggestionsDelay": 10,

	// Enable/disable the ability to preview changes before renaming
	"editor.rename.enablePreview": true,

	// Deprecated, use `editor.linkedEditing` instead.
	// Controls whether the editor auto renames on type.
	"editor.renameOnType": false,

	// Controls whether the editor should render control characters.
	"editor.renderControlCharacters": true,

	// Render last line number when the file ends with a newline.
	"editor.renderFinalNewline": "on",

	// Controls how the editor should render the current line highlight.
	//  - none
	//  - gutter
	//  - line
	//  - all: Highlights both the gutter and the current line.
	"editor.renderLineHighlight": "line",

	// Controls if the editor should render the current line highlight only when the editor is focused.
	"editor.renderLineHighlightOnlyWhenFocus": false,

	// Controls how the editor should render whitespace characters.
	//  - none
	//  - boundary: Render whitespace characters except for single spaces between words.
	//  - selection: Render whitespace characters only on selected text.
	//  - trailing: Render only trailing whitespace characters.
	//  - all
	"editor.renderWhitespace": "selection",

	// Controls whether selections should have rounded corners.
	"editor.roundedSelection": true,

	// Render vertical rulers after a certain number of monospace characters. Use multiple values for multiple rulers. No rulers are drawn if array is empty.
	"editor.rulers": [],

	// Control whether inline suggestions are announced by a screen reader.
	"editor.screenReaderAnnounceInlineSuggestion": true,

	// Controls the visibility of the horizontal scrollbar.
	//  - auto: The horizontal scrollbar will be visible only when necessary.
	//  - visible: The horizontal scrollbar will always be visible.
	//  - hidden: The horizontal scrollbar will always be hidden.
	"editor.scrollbar.horizontal": "auto",

	// The height of the horizontal scrollbar.
	"editor.scrollbar.horizontalScrollbarSize": 12,

	// When set, the horizontal scrollbar will not increase the size of the editor's content.
	"editor.scrollbar.ignoreHorizontalScrollbarInContentHeight": false,

	// Controls whether clicks scroll by page or jump to click position.
	"editor.scrollbar.scrollByPage": false,

	// Controls the visibility of the vertical scrollbar.
	//  - auto: The vertical scrollbar will be visible only when necessary.
	//  - visible: The vertical scrollbar will always be visible.
	//  - hidden: The vertical scrollbar will always be hidden.
	"editor.scrollbar.vertical": "auto",

	// The width of the vertical scrollbar.
	"editor.scrollbar.verticalScrollbarSize": 14,

	// Controls the number of extra characters beyond which the editor will scroll horizontally.
	"editor.scrollBeyondLastColumn": 4,

	// Controls whether the editor will scroll beyond the last line.
	"editor.scrollBeyondLastLine": true,

	// Scroll only along the predominant axis when scrolling both vertically and horizontally at the same time. Prevents horizontal drift when scrolling vertically on a trackpad.
	"editor.scrollPredominantAxis": true,

	// Controls whether the editor should highlight matches similar to the selection.
	"editor.selectionHighlight": true,

	// Controls whether the semanticHighlighting is shown for the languages that support it.
	//  - true: Semantic highlighting enabled for all color themes.
	//  - false: Semantic highlighting disabled for all color themes.
	//  - configuredByTheme: Semantic highlighting is configured by the current color theme's `semanticHighlighting` setting.
	"editor.semanticHighlighting.enabled": "configuredByTheme",

	// Overrides editor semantic token color and styles from the currently selected color theme.
	"editor.semanticTokenColorCustomizations": {},

	// Controls strikethrough deprecated variables.
	"editor.showDeprecated": true,

	// Controls when the folding controls on the gutter are shown.
	//  - always: Always show the folding controls.
	//  - never: Never show the folding controls and reduce the gutter size.
	//  - mouseover: Only show the folding controls when the mouse is over the gutter.
	"editor.showFoldingControls": "mouseover",

	// Controls fading out of unused code.
	"editor.showUnused": true,

	// Whether leading and trailing whitespace should always be selected.
	"editor.smartSelect.selectLeadingAndTrailingWhitespace": true,

	// Whether subwords (like 'foo' in 'fooBar' or 'foo_bar') should be selected.
	"editor.smartSelect.selectSubwords": true,

	// Controls whether the editor will scroll using an animation.
	"editor.smoothScrolling": false,

	// Controls if surround-with-snippets or file template snippets show as Code Actions.
	"editor.snippets.codeActions.enabled": true,

	// Controls whether snippets are shown with other suggestions and how they are sorted.
	//  - top: Show snippet suggestions on top of other suggestions.
	//  - bottom: Show snippet suggestions below other suggestions.
	//  - inline: Show snippets suggestions with other suggestions.
	//  - none: Do not show snippet suggestions.
	"editor.snippetSuggestions": "inline",

	// Keep peek editors open even when double-clicking their content or when hitting `Escape`.
	"editor.stablePeek": false,

	// Defines the model to use for determining which lines to stick. If the outline model does not exist, it will fall back on the folding provider model which falls back on the indentation model. This order is respected in all three cases.
	"editor.stickyScroll.defaultModel": "outlineModel",

	// Shows the nested current scopes during the scroll at the top of the editor.
	"editor.stickyScroll.enabled": true,

	// Defines the maximum number of sticky lines to show.
	"editor.stickyScroll.maxLineCount": 5,

	// Enable scrolling of Sticky Scroll with the editor's horizontal scrollbar.
	"editor.stickyScroll.scrollWithEditor": true,

	// Emulate selection behavior of tab characters when using spaces for indentation. Selection will stick to tab stops.
	"editor.stickyTabStops": false,

	// This setting is deprecated, please use separate settings like 'editor.suggest.showKeywords' or 'editor.suggest.showSnippets' instead.
	// 
	"editor.suggest.filteredTypes": {},

	// Controls whether filtering and sorting suggestions accounts for small typos.
	"editor.suggest.filterGraceful": true,

	// Controls whether words are overwritten when accepting completions. Note that this depends on extensions opting into this feature.
	//  - insert: Insert suggestion without overwriting text right of the cursor.
	//  - replace: Insert suggestion and overwrite text right of the cursor.
	"editor.suggest.insertMode": "insert",

	// Controls whether sorting favors words that appear close to the cursor.
	"editor.suggest.localityBonus": false,

	// When enabled IntelliSense filtering requires that the first character matches on a word start. For example, `c` on `Console` or `WebContext` but _not_ on `description`. When disabled IntelliSense will show more results but still sorts them by match quality.
	"editor.suggest.matchOnWordStartOnly": true,

	// This setting is deprecated. The suggest widget can now be resized.
	// 
	"editor.suggest.maxVisibleSuggestions": 0,

	// Controls whether to preview the suggestion outcome in the editor.
	"editor.suggest.preview": false,

	// Controls whether a suggestion is selected when the widget shows. Note that this only applies to automatically triggered suggestions (`editor.quickSuggestions#` and `#editor.suggestOnTriggerCharacters`) and that a suggestion is always selected when explicitly invoked, e.g via `Ctrl+Space`.
	//  - always: Always select a suggestion when automatically triggering IntelliSense.
	//  - never: Never select a suggestion when automatically triggering IntelliSense.
	//  - whenTriggerCharacter: Select a suggestion only when triggering IntelliSense from a trigger character.
	//  - whenQuickSuggestion: Select a suggestion only when triggering IntelliSense as you type.
	"editor.suggest.selectionMode": "always",

	// Controls whether remembered suggestion selections are shared between multiple workspaces and windows (needs `editor.suggestSelection`).
	"editor.suggest.shareSuggestSelections": false,

	// When enabled IntelliSense shows `class`-suggestions.
	"editor.suggest.showClasses": true,

	// When enabled IntelliSense shows `color`-suggestions.
	"editor.suggest.showColors": true,

	// When enabled IntelliSense shows `constant`-suggestions.
	"editor.suggest.showConstants": true,

	// When enabled IntelliSense shows `constructor`-suggestions.
	"editor.suggest.showConstructors": true,

	// When enabled IntelliSense shows `customcolor`-suggestions.
	"editor.suggest.showCustomcolors": true,

	// When enabled IntelliSense shows `deprecated`-suggestions.
	"editor.suggest.showDeprecated": true,

	// When enabled IntelliSense shows `enumMember`-suggestions.
	"editor.suggest.showEnumMembers": true,

	// When enabled IntelliSense shows `enum`-suggestions.
	"editor.suggest.showEnums": true,

	// When enabled IntelliSense shows `event`-suggestions.
	"editor.suggest.showEvents": true,

	// When enabled IntelliSense shows `field`-suggestions.
	"editor.suggest.showFields": true,

	// When enabled IntelliSense shows `file`-suggestions.
	"editor.suggest.showFiles": true,

	// When enabled IntelliSense shows `folder`-suggestions.
	"editor.suggest.showFolders": true,

	// When enabled IntelliSense shows `function`-suggestions.
	"editor.suggest.showFunctions": true,

	// Controls whether to show or hide icons in suggestions.
	"editor.suggest.showIcons": true,

	// Controls whether suggest details show inline with the label or only in the details widget.
	"editor.suggest.showInlineDetails": true,

	// When enabled IntelliSense shows `interface`-suggestions.
	"editor.suggest.showInterfaces": true,

	// When enabled IntelliSense shows `issues`-suggestions.
	"editor.suggest.showIssues": true,

	// When enabled IntelliSense shows `keyword`-suggestions.
	"editor.suggest.showKeywords": true,

	// When enabled IntelliSense shows `method`-suggestions.
	"editor.suggest.showMethods": true,

	// When enabled IntelliSense shows `module`-suggestions.
	"editor.suggest.showModules": true,

	// When enabled IntelliSense shows `operator`-suggestions.
	"editor.suggest.showOperators": true,

	// When enabled IntelliSense shows `property`-suggestions.
	"editor.suggest.showProperties": true,

	// When enabled IntelliSense shows `reference`-suggestions.
	"editor.suggest.showReferences": true,

	// When enabled IntelliSense shows `snippet`-suggestions.
	"editor.suggest.showSnippets": true,

	// Controls the visibility of the status bar at the bottom of the suggest widget.
	"editor.suggest.showStatusBar": false,

	// When enabled IntelliSense shows `struct`-suggestions.
	"editor.suggest.showStructs": true,

	// When enabled IntelliSense shows `typeParameter`-suggestions.
	"editor.suggest.showTypeParameters": true,

	// When enabled IntelliSense shows `unit`-suggestions.
	"editor.suggest.showUnits": true,

	// When enabled IntelliSense shows `user`-suggestions.
	"editor.suggest.showUsers": true,

	// When enabled IntelliSense shows `value`-suggestions.
	"editor.suggest.showValues": true,

	// When enabled IntelliSense shows `variable`-suggestions.
	"editor.suggest.showVariables": true,

	// When enabled IntelliSense shows `text`-suggestions.
	"editor.suggest.showWords": true,

	// Controls whether an active snippet prevents quick suggestions.
	"editor.suggest.snippetsPreventQuickSuggestions": false,

	// Font size for the suggest widget. When set to `0`, the value of `editor.fontSize` is used.
	"editor.suggestFontSize": 0,

	// Line height for the suggest widget. When set to `0`, the value of `editor.lineHeight` is used. The minimum value is 8.
	"editor.suggestLineHeight": 0,

	// Controls whether suggestions should automatically show up when typing trigger characters.
	"editor.suggestOnTriggerCharacters": true,

	// Controls how suggestions are pre-selected when showing the suggest list.
	//  - first: Always select the first suggestion.
	//  - recentlyUsed: Select recent suggestions unless further typing selects one, e.g. `console.| -> console.log` because `log` has been completed recently.
	//  - recentlyUsedByPrefix: Select suggestions based on previous prefixes that have completed those suggestions, e.g. `co -> console` and `con -> const`.
	"editor.suggestSelection": "first",

	// Enables tab completions.
	//  - on: Tab complete will insert the best matching suggestion when pressing tab.
	//  - off: Disable tab completions.
	//  - onlySnippets: Tab complete snippets when their prefix match. Works best when 'quickSuggestions' aren't enabled.
	"editor.tabCompletion": "off",

	// Controls whether the editor receives tabs or defers them to the workbench for navigation.
	"editor.tabFocusMode": false,

	// The number of spaces a tab is equal to. This setting is overridden based on the file contents when `editor.detectIndentation` is on.
	"editor.tabSize": 4,

	// Overrides editor syntax colors and font style from the currently selected color theme.
	"editor.tokenColorCustomizations": {},

	// Remove trailing auto inserted whitespace.
	"editor.trimAutoWhitespace": true,

	// Controls whether clicking on the empty content after a folded line will unfold the line.
	"editor.unfoldOnClickAfterEndOfLine": false,

	// Defines allowed characters that are not being highlighted.
	"editor.unicodeHighlight.allowedCharacters": {},

	// Unicode characters that are common in allowed locales are not being highlighted.
	"editor.unicodeHighlight.allowedLocales": {
		"_os": true,
		"_vscode": true
	},

	// Controls whether characters are highlighted that can be confused with basic ASCII characters, except those that are common in the current user locale.
	"editor.unicodeHighlight.ambiguousCharacters": true,

	// Controls whether characters in comments should also be subject to Unicode highlighting.
	"editor.unicodeHighlight.includeComments": "inUntrustedWorkspace",

	// Controls whether characters in strings should also be subject to Unicode highlighting.
	"editor.unicodeHighlight.includeStrings": true,

	// Controls whether characters that just reserve space or have no width at all are highlighted.
	"editor.unicodeHighlight.invisibleCharacters": true,

	// Controls whether all non-basic ASCII characters are highlighted. Only characters between U+0020 and U+007E, tab, line-feed and carriage-return are considered basic ASCII.
	"editor.unicodeHighlight.nonBasicASCII": "inUntrustedWorkspace",

	// Remove unusual line terminators that might cause problems.
	//  - auto: Unusual line terminators are automatically removed.
	//  - off: Unusual line terminators are ignored.
	//  - prompt: Unusual line terminators prompt to be removed.
	"editor.unusualLineTerminators": "prompt",

	// Spaces and tabs are inserted and deleted in alignment with tab stops.
	"editor.useTabStops": true,

	// Controls whether completions should be computed based on words in the document and from which documents they are computed.
	//  - off: Turn off Word Based Suggestions.
	//  - currentDocument: Only suggest words from the active document.
	//  - matchingDocuments: Suggest words from all open documents of the same language.
	//  - allDocuments: Suggest words from all open documents.
	"editor.wordBasedSuggestions": "matchingDocuments",

	// Controls the word break rules used for Chinese/Japanese/Korean (CJK) text.
	//  - normal: Use the default line break rule.
	//  - keepAll: Word breaks should not be used for Chinese/Japanese/Korean (CJK) text. Non-CJK text behavior is the same as for normal.
	"editor.wordBreak": "normal",

	// 
	"editor.wordSegmenterLocales": null,

	// Characters that will be used as word separators when doing word related navigations or operations.
	"editor.wordSeparators": "`~!@#$%^&*()-=+[{]}\\|;:'\",.<>/?",

	// Controls how lines should wrap.
	//  - off: Lines will never wrap.
	//  - on: Lines will wrap at the viewport width.
	//  - wordWrapColumn: Lines will wrap at `editor.wordWrapColumn`.
	//  - bounded: Lines will wrap at the minimum of viewport and `editor.wordWrapColumn`.
	"editor.wordWrap": "off",

	// Controls the wrapping column of the editor when `editor.wordWrap` is `wordWrapColumn` or `bounded`.
	"editor.wordWrapColumn": 80,

	// Controls the indentation of wrapped lines.
	//  - none: No indentation. Wrapped lines begin at column 1.
	//  - same: Wrapped lines get the same indentation as the parent.
	//  - indent: Wrapped lines get +1 indentation toward the parent.
	//  - deepIndent: Wrapped lines get +2 indentation toward the parent.
	"editor.wrappingIndent": "same",

	// Controls the algorithm that computes wrapping points. Note that when in accessibility mode, advanced will be used for the best experience.
	//  - simple: Assumes that all characters are of the same width. This is a fast algorithm that works correctly for monospace fonts and certain scripts (like Latin characters) where glyphs are of equal width.
	//  - advanced: Delegates wrapping points computation to the browser. This is a slow algorithm, that might cause freezes for large files, but it works correctly in all cases.
	"editor.wrappingStrategy": "simple",

	// Whether the inline chat also renders an accessible diff viewer for its changes.
	//  - auto: The accessible diff viewer is based on screen reader mode being enabled.
	//  - on: The accessible diff viewer is always enabled.
	//  - off: The accessible diff viewer is never enabled.
	"inlineChat.accessibleDiffView": "auto",

	// Whether to finish an inline chat session when typing outside of changed regions.
	"inlineChat.finishOnType": false,

	// Whether holding the inline chat keybinding will automatically enable speech recognition.
	"inlineChat.holdToSpeech": true,

	// Whether empty lines show a hint to generate code with inline chat.
	"inlineChat.lineEmptyHint": false,

	// Whether lines that are dominated by natural language or pseudo code show a hint to continue with inline chat. For instance, `class Person with name and hobbies` would show a hint to continue with chat.
	"inlineChat.lineNaturalLanguageHint": true,

	// Run a series of Code Actions for a notebook on save. Code Actions must be specified and the editor must not be shutting down. When `files.autoSave` is set to `afterDelay`, Code Actions will only be run when the file is saved explicitly. Example: `"notebook.source.organizeImports": "explicit"`
	"notebook.codeActionsOnSave": {},

	// Controls whether inline actions are always visible in the Source Control view.
	"scm.alwaysShowActions": false,

	// Controls whether repositories should always be visible in the Source Control view.
	"scm.alwaysShowRepositories": false,

	// Controls whether the Source Control view should automatically reveal and select files when opening them.
	"scm.autoReveal": true,

	// Controls whether the Source Control view should render folders in a compact form. In such a form, single child folders will be compressed in a combined tree element.
	"scm.compactFolders": true,

	// Controls the count badge on the Source Control icon on the Activity Bar.
	//  - all: Show the sum of all Source Control Provider count badges.
	//  - focused: Show the count badge of the focused Source Control Provider.
	//  - off: Disable the Source Control count badge.
	"scm.countBadge": "all",

	// Controls the default Source Control repository view mode.
	//  - tree: Show the repository changes as a tree.
	//  - list: Show the repository changes as a list.
	"scm.defaultViewMode": "list",

	// Controls the default Source Control repository changes sort order when viewed as a list.
	//  - name: Sort the repository changes by file name.
	//  - path: Sort the repository changes by path.
	//  - status: Sort the repository changes by Source Control status.
	"scm.defaultViewSortKey": "path",

	// Controls diff decorations in the editor.
	//  - all: Show the diff decorations in all available locations.
	//  - gutter: Show the diff decorations only in the editor gutter.
	//  - overview: Show the diff decorations only in the overview ruler.
	//  - minimap: Show the diff decorations only in the minimap.
	//  - none: Do not show the diff decorations.
	"scm.diffDecorations": "all",

	// Controls the behavior of Source Control diff gutter decorations.
	//  - diff: Show the inline diff Peek view on click.
	//  - none: Do nothing.
	"scm.diffDecorationsGutterAction": "diff",

	// Controls whether a pattern is used for the diff decorations in gutter.
	"scm.diffDecorationsGutterPattern": {
		"added": false,
		"modified": true
	},

	// Controls the visibility of the Source Control diff decorator in the gutter.
	//  - always: Show the diff decorator in the gutter at all times.
	//  - hover: Show the diff decorator in the gutter only on hover.
	"scm.diffDecorationsGutterVisibility": "always",

	// Controls the width(px) of diff decorations in gutter (added & modified).
	"scm.diffDecorationsGutterWidth": 3,

	// Controls whether leading and trailing whitespace is ignored in Source Control diff gutter decorations.
	//  - true: Ignore leading and trailing whitespace.
	//  - false: Do not ignore leading and trailing whitespace.
	//  - inherit: Inherit from `diffEditor.ignoreTrimWhitespace`.
	"scm.diffDecorationsIgnoreTrimWhitespace": "false",

	// Controls which badges are shown in the Source Control Graph view. The badges are shown on the right side of the graph indicating the names of history item groups.
	//  - all: Show badges of all history item groups in the Source Control Graph view.
	//  - filter: Show only the badges of history item groups used as a filter in the Source Control Graph view.
	"scm.graph.badges": "filter",

	// Controls whether the Source Control Graph view will load the next page of items when you scroll to the end of the list.
	"scm.graph.pageOnScroll": true,

	// The number of items to show in the Source Control Graph view by default and when loading more items.
	"scm.graph.pageSize": 50,

	// Controls the font for the input message. Use `default` for the workbench user interface font family, `editor` for the `editor.fontFamily`'s value, or a custom font family.
	"scm.inputFontFamily": "default",

	// Controls the font size for the input message in pixels.
	"scm.inputFontSize": 13,

	// Controls the maximum number of lines that the input will auto-grow to.
	"scm.inputMaxLineCount": 10,

	// Controls the minimum number of lines that the input will auto-grow from.
	"scm.inputMinLineCount": 1,

	// Controls the count badges on Source Control Provider headers. These headers appear in the Source Control view when there is more than one provider or when the `scm.alwaysShowRepositories` setting is enabled, and in the Source Control Repositories view.
	//  - hidden: Hide Source Control Provider count badges.
	//  - auto: Only show count badge for Source Control Provider when non-zero.
	//  - visible: Show Source Control Provider count badges.
	"scm.providerCountBadge": "hidden",

	// Controls the sort order of the repositories in the source control repositories view.
	//  - discovery time: Repositories in the Source Control Repositories view are sorted by discovery time. Repositories in the Source Control view are sorted in the order that they were selected.
	//  - name: Repositories in the Source Control Repositories and Source Control views are sorted by repository name.
	//  - path: Repositories in the Source Control Repositories and Source Control views are sorted by repository path.
	"scm.repositories.sortOrder": "discovery time",

	// Controls how many repositories are visible in the Source Control Repositories section. Set to 0, to be able to manually resize the view.
	"scm.repositories.visible": 10,

	// Controls whether an action button can be shown in the Source Control view.
	"scm.showActionButton": true,

	// Controls whether an action button can be shown in the Source Control input.
	"scm.showInputActionButton": true,

	// Controls the default working set to use when switching to a source control history item group that does not have a working set.
	//  - empty: Use an empty working set when switching to a source control history item group that does not have a working set.
	//  - current: Use the current working set when switching to a source control history item group that does not have a working set.
	"scm.workingSets.default": "current",

	// Controls whether to store editor working sets when switching between source control history item groups.
	"scm.workingSets.enabled": false,

	// A set of UNC host names (without leading or trailing backslash, for example `192.168.0.1` or `my-server`) to allow without user confirmation. If a UNC host is being accessed that is not allowed via this setting or has not been acknowledged via user confirmation, an error will occur and the operation stopped. A restart is required when changing this setting. Find out more about this setting at https://aka.ms/vscode-windows-unc.
	"security.allowedUNCHosts": [],

	// If enabled, a dialog will ask for confirmation whenever a local file or workspace is about to open through a protocol handler.
	"security.promptForLocalFileProtocolHandling": true,

	// If enabled, a dialog will ask for confirmation whenever a remote file or workspace is about to open through a protocol handler.
	"security.promptForRemoteFileProtocolHandling": true,

	// If enabled, only allows access to UNC host names that are allowed by the `security.allowedUNCHosts` setting or after user confirmation. Find out more about this setting at https://aka.ms/vscode-windows-unc.
	"security.restrictUNCAccess": true,

	// Controls when the restricted mode banner is shown.
	//  - always: Show the banner every time an untrusted workspace is open.
	//  - untilDismissed: Show the banner when an untrusted workspace is opened until dismissed.
	//  - never: Do not show the banner when an untrusted workspace is open.
	"security.workspace.trust.banner": "untilDismissed",

	// Controls whether or not the empty window is trusted by default within VS Code. When used with `security.workspace.trust.untrustedFiles`, you can enable the full functionality of VS Code without prompting in an empty window.
	"security.workspace.trust.emptyWindow": true,

	// Controls whether or not Workspace Trust is enabled within VS Code.
	"security.workspace.trust.enabled": true,

	// Controls when the startup prompt to trust a workspace is shown.
	//  - always: Ask for trust every time an untrusted workspace is opened.
	//  - once: Ask for trust the first time an untrusted workspace is opened.
	//  - never: Do not ask for trust when an untrusted workspace is opened.
	"security.workspace.trust.startupPrompt": "once",

	// Controls how to handle opening untrusted files in a trusted workspace. This setting also applies to opening files in an empty window which is trusted via `security.workspace.trust.emptyWindow`.
	//  - prompt: Ask how to handle untrusted files for each workspace. Once untrusted files are introduced to a trusted workspace, you will not be prompted again.
	//  - open: Always allow untrusted files to be introduced to a trusted workspace without prompting.
	//  - newWindow: Always open untrusted files in a separate window in restricted mode without prompting.
	"security.workspace.trust.untrustedFiles": "prompt",

	// Whether to dim unfocused editors and terminals, which makes it more clear where typed input will go to. This works with the majority of editors with the notable exceptions of those that utilize iframes like notebooks and extension webview editors.
	"accessibility.dimUnfocused.enabled": false,

	// The opacity fraction (0.2 to 1.0) to use for unfocused editors and terminals. This will only take effect when `accessibility.dimUnfocused.enabled` is enabled.
	"accessibility.dimUnfocused.opacity": 0.75,

	// Controls whether the Accessible View is hidden.
	"accessibility.hideAccessibleView": false,

	// Controls the height of editor tabs. Also applies to the title control bar when `workbench.editor.showTabs` is not set to `multiple`.
	"window.density.editorTabHeight": "default",

	// Controls the behavior of clicking an Activity Bar icon in the workbench. This value is ignored when `workbench.activityBar.location` is not set to `default`.
	//  - toggle: Hide the Primary Side Bar if the clicked item is already visible.
	//  - focus: Focus the Primary Side Bar if the clicked item is already visible.
	"workbench.activityBar.iconClickBehavior": "toggle",

	// Controls the location of the Activity Bar relative to the Primary and Secondary Side Bars.
	//  - default: Show the Activity Bar on the side of the Primary Side Bar and on top of the Secondary Side Bar.
	//  - top: Show the Activity Bar on top of the Primary and Secondary Side Bars.
	//  - bottom: Show the Activity Bar at the bottom of the Primary and Secondary Side Bars.
	//  - hidden: Hide the Activity Bar in the Primary and Secondary Side Bars.
	"workbench.activityBar.location": "default",

	// Controls whether to automatically resume available working changes stored in the cloud for the current workspace.
	//  - onReload: Automatically resume available working changes from the cloud on window reload.
	//  - off: Never attempt to resume working changes from the cloud.
	"workbench.cloudChanges.autoResume": "onReload",

	// Controls whether to prompt the user to store working changes in the cloud when using Continue Working On.
	//  - prompt: Prompt the user to sign in to store working changes in the cloud with Continue Working On.
	//  - off: Do not store working changes in the cloud with Continue Working On unless the user has already turned on Cloud Changes.
	"workbench.cloudChanges.continueOn": "prompt",

	// Overrides colors from the currently selected color theme.
	"workbench.colorCustomizations": {},

	// Specifies the color theme used in the workbench when `window.autoDetectColorScheme` is not enabled.
	"workbench.colorTheme": "Default Dark Modern",

	// Controls where the command palette should ask chat questions.
	//  - chatView: Ask chat questions in the Chat view.
	//  - quickChat: Ask chat questions in Quick Chat.
	"workbench.commandPalette.experimental.askChatLocation": "chatView",

	// Controls whether the command palette should include similar commands. You must have an extension installed that provides Natural Language support.
	"workbench.commandPalette.experimental.enableNaturalLanguageSearch": true,

	// Controls whether the command palette should have a list of commonly used commands.
	"workbench.commandPalette.experimental.suggestCommands": false,

	// Controls the number of recently used commands to keep in history for the command palette. Set to 0 to disable command history.
	"workbench.commandPalette.history": 50,

	// Controls whether the last typed input to the command palette should be restored when opening it the next time.
	"workbench.commandPalette.preserveInput": false,

	// Controls whether to always show the editor actions, even when the editor group is not active.
	"workbench.editor.alwaysShowEditorActions": false,

	// If an editor matching one of the listed types is opened as the first in an editor group and more than one group is open, the group is automatically locked. Locked groups will only be used for opening editors when explicitly chosen by a user gesture (for example drag and drop), but not by default. Consequently, the active editor in a locked group is less likely to be replaced accidentally with a different editor.
	"workbench.editor.autoLockGroups": {
		"default": false,
		"workbench.editor.chatSession": false,
		"workbench.editorinputs.searchEditorInput": false,
		"repl": false,
		"workbench.editors.gettingStartedInput": false,
		"terminalEditor": true,
		"jupyter-notebook": false,
		"imagePreview.previewEditor": false,
		"vscode.audioPreview": false,
		"vscode.videoPreview": false,
		"jsProfileVisualizer.cpuprofile.table": false,
		"jsProfileVisualizer.heapprofile.table": false,
		"jsProfileVisualizer.heapsnapshot.table": false,
		"svgPreviewer.customEditor": false,
		"workbench.input.interactive": false,
		"mainThreadWebview-markdown.preview": false,
		"mainThreadWebview-simpleBrowser.view": true,
		"mainThreadWebview-browserPreview": true
	},

	// Controls if the centered layout should automatically resize to maximum width when more than one group is open. Once only one group is open it will resize back to the original centered width.
	"workbench.editor.centeredLayoutAutoResize": true,

	// Controls whether the centered layout tries to maintain constant width when the window is resized.
	"workbench.editor.centeredLayoutFixedWidth": false,

	// Controls the behavior of empty editor groups when the last tab in the group is closed. When enabled, empty groups will automatically close. When disabled, empty groups will remain part of the grid.
	"workbench.editor.closeEmptyGroups": true,

	// Controls whether editors showing a file that was opened during the session should close automatically when getting deleted or renamed by some other process. Disabling this will keep the editor open  on such an event. Note that deleting from within the application will always close the editor and that editors with unsaved changes will never close to preserve your data.
	"workbench.editor.closeOnFileDelete": false,

	// Controls whether the custom workbench editor labels should be applied.
	"workbench.editor.customLabels.enabled": true,

	// Controls the rendering of the editor label. Each __Item__ is a pattern that matches a file path. Both relative and absolute file paths are supported. The relative path must include the WORKSPACE_FOLDER (e.g `WORKSPACE_FOLDER/src/**.tsx` or `*/src/**.tsx`). Absolute patterns must start with a `/`. In case multiple patterns match, the longest matching path will be picked. Each __Value__ is the template for the rendered editor when the __Item__ matches. Variables are substituted based on the context:
	// - `${dirname}`: name of the folder in which the file is located (e.g. `WORKSPACE_FOLDER/folder/file.txt -> folder`).
	// - `${dirname(N)}`: name of the nth parent folder in which the file is located (e.g. `N=2: WORKSPACE_FOLDER/static/folder/file.txt -> WORKSPACE_FOLDER`). Folders can be picked from the start of the path by using negative numbers (e.g. `N=-1: WORKSPACE_FOLDER/folder/file.txt -> WORKSPACE_FOLDER`). If the __Item__ is an absolute pattern path, the first folder (`N=-1`) refers to the first folder in the absolute path, otherwise it corresponds to the workspace folder.
	// - `${filename}`: name of the file without the file extension (e.g. `WORKSPACE_FOLDER/folder/file.txt -> file`).
	// - `${extname}`: the file extension (e.g. `WORKSPACE_FOLDER/folder/file.txt -> txt`).
	// - `${extname(N)}`: the nth extension of the file separated by '.' (e.g. `N=2: WORKSPACE_FOLDER/folder/file.ext1.ext2.ext3 -> ext1`). Extension can be picked from the start of the extension by using negative numbers (e.g. `N=-1: WORKSPACE_FOLDER/folder/file.ext1.ext2.ext3 -> ext2`).
	// 
	// Example: `"**/static/**/*.html": "${filename} - ${dirname} (${extname})"` will render a file `WORKSPACE_FOLDER/static/folder/file.html` as `file - folder (html)`.
	"workbench.editor.customLabels.patterns": {},

	// Controls whether editor file decorations should use badges.
	"workbench.editor.decorations.badges": true,

	// Controls whether editor file decorations should use colors.
	"workbench.editor.decorations.colors": true,

	// The default editor for files detected as binary. If undefined, the user will be presented with a picker.
	"workbench.editor.defaultBinaryEditor": "",

	// Controls how the editor group is resized when double clicking on a tab. This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	//  - maximize: All other editor groups are hidden and the current editor group is maximized to take up the entire editor area.
	//  - expand: The editor group takes as much space as possible by making all other editor groups as small as possible.
	//  - off: No editor group is resized when double clicking on a tab.
	"workbench.editor.doubleClickTabToToggleEditorGroupSizes": "expand",

	// Controls if editors can be dragged out of the window to open them in a new window. Press and hold the `Alt` key while dragging to toggle this dynamically.
	"workbench.editor.dragToOpenWindow": true,

	// Controls where the editor actions are shown.
	//  - default: Show editor actions in the window title bar when `workbench.editor.showTabs` is set to `none`. Otherwise, editor actions are shown in the editor tab bar.
	//  - titleBar: Show editor actions in the window title bar. If `window.customTitleBarVisibility` is set to `never`, editor actions are hidden.
	//  - hidden: Editor actions are not shown.
	"workbench.editor.editorActionsLocation": "default",

	// Controls if the empty editor text hint should be visible in the editor.
	"workbench.editor.empty.hint": "text",

	// Controls whether preview mode is used when editors open. There is a maximum of one preview mode editor per editor group. This editor displays its filename in italics on its tab or title label and in the Open Editors view. Its contents will be replaced by the next editor opened in preview mode. Making a change in a preview mode editor will persist it, as will a double-click on its label, or the 'Keep Open' option in its label context menu. Opening a file from Explorer with a double-click persists its editor immediately.
	"workbench.editor.enablePreview": true,

	// Controls whether editors remain in preview when a code navigation is started from them. Preview editors do not stay open, and are reused until explicitly set to be kept open (via double-click or editing). This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	"workbench.editor.enablePreviewFromCodeNavigation": false,

	// Controls whether editors opened from Quick Open show as preview editors. Preview editors do not stay open, and are reused until explicitly set to be kept open (via double-click or editing). When enabled, hold Ctrl before selection to open an editor as a non-preview. This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	"workbench.editor.enablePreviewFromQuickOpen": false,

	// Controls whether editors are closed in most recently used order or from left to right.
	"workbench.editor.focusRecentEditorAfterClose": true,

	// Controls whether a top border is drawn on tabs for editors that have unsaved changes. This value is ignored when `workbench.editor.showTabs` is not set to multiple.
	"workbench.editor.highlightModifiedTabs": false,

	// Enables use of editor history in language detection. This causes automatic language detection to favor languages that have been recently opened and allows for automatic language detection to operate with smaller inputs.
	"workbench.editor.historyBasedLanguageDetection": true,

	// Controls the format of the label for an editor.
	//  - default: Show the name of the file. When tabs are enabled and two files have the same name in one group the distinguishing sections of each file's path are added. When tabs are disabled, the path relative to the workspace folder is shown if the editor is active.
	//  - short: Show the name of the file followed by its directory name.
	//  - medium: Show the name of the file followed by its path relative to the workspace folder.
	//  - long: Show the name of the file followed by its absolute path.
	"workbench.editor.labelFormat": "default",

	// Controls whether the language in a text editor is automatically detected unless the language has been explicitly set by the language picker. This can also be scoped by language so you can specify which languages you do not want to be switched off of. This is useful for languages like Markdown that often contain other languages that might trick language detection into thinking it's the embedded language and not Markdown.
	"workbench.editor.languageDetection": true,

	// When enabled, shows a Status bar Quick Fix when the editor language doesn't match detected content language.
	"workbench.editor.languageDetectionHints": {
		"untitledEditors": true,
		"notebookEditors": true
	},

	// Controls if the number of opened editors should be limited or not. When enabled, less recently used editors will close to make space for newly opening editors.
	"workbench.editor.limit.enabled": false,

	// Controls if the maximum number of opened editors should exclude dirty editors for counting towards the configured limit.
	"workbench.editor.limit.excludeDirty": false,

	// Controls if the limit of maximum opened editors should apply per editor group or across all editor groups.
	"workbench.editor.limit.perEditorGroup": false,

	// Controls the maximum number of opened editors. Use the `workbench.editor.limit.perEditorGroup` setting to control this limit per editor group or across all groups.
	"workbench.editor.limit.value": 10,

	// Enables the use of mouse buttons four and five for commands 'Go Back' and 'Go Forward'.
	"workbench.editor.mouseBackForwardToNavigate": true,

	// Controls the scope of history navigation in editors for commands such as 'Go Back' and 'Go Forward'.
	//  - default: Navigate across all opened editors and editor groups.
	//  - editorGroup: Navigate only in editors of the active editor group.
	//  - editor: Navigate only in the active editor.
	"workbench.editor.navigationScope": "default",

	// Controls where editors open. Select `left` or `right` to open editors to the left or right of the currently active one. Select `first` or `last` to open editors independently from the currently active one.
	"workbench.editor.openPositioning": "right",

	// Controls the default direction of editors that are opened side by side (for example, from the Explorer). By default, editors will open on the right hand side of the currently active one. If changed to `down`, the editors will open below the currently active one.
	"workbench.editor.openSideBySideDirection": "right",

	// Controls the size of pinned editor tabs. Pinned tabs are sorted to the beginning of all opened tabs and typically do not close until unpinned. This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	//  - normal: A pinned tab inherits the look of non pinned tabs.
	//  - compact: A pinned tab will show in a compact form with only icon or first letter of the editor name.
	//  - shrink: A pinned tab shrinks to a compact fixed size showing parts of the editor name.
	"workbench.editor.pinnedTabSizing": "normal",

	// When enabled, displays pinned tabs in a separate row above all other tabs. This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	"workbench.editor.pinnedTabsOnSeparateRow": false,

	// When enabled, a language detection model that takes into account editor history will be given higher precedence.
	"workbench.editor.preferHistoryBasedLanguageDetection": false,

	// Controls whether pinned editors should close when keyboard or middle mouse click is used for closing.
	//  - keyboardAndMouse: Always prevent closing the pinned editor when using mouse middle click or keyboard.
	//  - keyboard: Prevent closing the pinned editor when using the keyboard.
	//  - mouse: Prevent closing the pinned editor when using mouse middle click.
	//  - never: Never prevent closing a pinned editor.
	"workbench.editor.preventPinnedEditorClose": "keyboardAndMouse",

	// Restores the last editor view state (such as scroll position) when re-opening editors after they have been closed. Editor view state is stored per editor group and discarded when a group closes. Use the `workbench.editor.sharedViewState` setting to use the last known view state across all editor groups in case no previous view state was found for a editor group.
	"workbench.editor.restoreViewState": true,

	// Controls whether an editor is revealed in any of the visible groups if opened. If disabled, an editor will prefer to open in the currently active editor group. If enabled, an already opened editor will be revealed instead of opened again in the currently active editor group. Note that there are some cases where this setting is ignored, such as when forcing an editor to open in a specific group or to the side of the currently active group.
	"workbench.editor.revealIfOpen": false,

	// Controls whether scrolling over tabs will open them or not. By default tabs will only reveal upon scrolling, but not open. You can press and hold the Shift-key while scrolling to change this behavior for that duration. This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	"workbench.editor.scrollToSwitchTabs": false,

	// Preserves the most recent editor view state (such as scroll position) across all editor groups and restores that if no specific editor view state is found for the editor group.
	"workbench.editor.sharedViewState": false,

	// Controls whether opened editors should show with an icon or not. This requires a file icon theme to be enabled as well.
	"workbench.editor.showIcons": true,

	// Controls whether opened editors should show as individual tabs, one single large tab or if the title area should not be shown.
	//  - multiple: Each editor is displayed as a tab in the editor title area.
	//  - single: The active editor is displayed as a single large tab in the editor title area.
	//  - none: The editor title area is not displayed.
	"workbench.editor.showTabs": "multiple",

	// Controls the layout for when an editor is split in an editor group to be either vertical or horizontal.
	//  - vertical: Editors are positioned from top to bottom.
	//  - horizontal: Editors are positioned from left to right.
	"workbench.editor.splitInGroupLayout": "horizontal",

	// Controls if editor groups can be split from drag and drop operations by dropping an editor or file on the edges of the editor area.
	"workbench.editor.splitOnDragAndDrop": true,

	// Controls the size of editor groups when splitting them.
	//  - auto: Splits the active editor group to equal parts, unless all editor groups are already in equal parts. In that case, splits all the editor groups to equal parts.
	//  - distribute: Splits all the editor groups to equal parts.
	//  - split: Splits the active editor group to equal parts.
	"workbench.editor.splitSizing": "auto",

	// Controls the visibility of the tab close action button.
	"workbench.editor.tabActionCloseVisibility": true,

	// Controls the position of the editor's tabs action buttons (close, unpin). This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	"workbench.editor.tabActionLocation": "right",

	// Controls the visibility of the tab unpin action button.
	"workbench.editor.tabActionUnpinVisibility": true,

	// Controls the size of editor tabs. This value is ignored when `workbench.editor.showTabs` is not set to `multiple`.
	//  - fit: Always keep tabs large enough to show the full editor label.
	//  - shrink: Allow tabs to get smaller when the available space is not enough to show all tabs at once.
	//  - fixed: Make all tabs the same size, while allowing them to get smaller when the available space is not enough to show all tabs at once.
	"workbench.editor.tabSizing": "fit",

	// Controls the maximum width of tabs when `workbench.editor.tabSizing` size is set to `fixed`.
	"workbench.editor.tabSizingFixedMaxWidth": 160,

	// Controls the minimum width of tabs when `workbench.editor.tabSizing` size is set to `fixed`.
	"workbench.editor.tabSizingFixedMinWidth": 50,

	// Controls the height of the scrollbars used for tabs and breadcrumbs in the editor title area.
	//  - default: The default size.
	//  - large: Increases the size, so it can be grabbed more easily with the mouse.
	"workbench.editor.titleScrollbarSizing": "default",

	// Controls the format of the label for an untitled editor.
	//  - content: The name of the untitled file is derived from the contents of its first line unless it has an associated file path. It will fallback to the name in case the line is empty or contains no word characters.
	//  - name: The name of the untitled file is not derived from the contents of the file.
	"workbench.editor.untitled.labelFormat": "content",

	// Controls whether tabs should be wrapped over multiple lines when exceeding available space or whether a scrollbar should appear instead. This value is ignored when `workbench.editor.showTabs` is not set to '`multiple`'.
	"workbench.editor.wrapTabs": false,

	// Configure [glob patterns](https://aka.ms/vscode-glob-patterns) to editors (for example `"*.hex": "hexEditor.hexedit"`). These have precedence over the default behavior.
	"workbench.editorAssociations": {},

	// Controls the minimum size of a file in MB before asking for confirmation when opening in the editor. Note that this setting may not apply to all editor types and environments.
	"workbench.editorLargeFileConfirmation": 1024,

	// Fetches experiments to run from a Microsoft online service.
	"workbench.enableExperiments": true,

	// Controls whether to automatically store available working changes in the cloud for the current workspace. This setting has no effect in the web.
	//  - onShutdown: Automatically store current working changes in the cloud on window close.
	//  - off: Never attempt to automatically store working changes in the cloud.
	"workbench.experimental.cloudChanges.autoStore": "off",

	// Controls whether to surface cloud changes which partially match the current session.
	"workbench.experimental.cloudChanges.partialMatches.enabled": false,

	// Controls whether to render the Share action next to the command center when `window.commandCenter` is `true`.
	"workbench.experimental.share.enabled": false,

	// Configure the browser to use for opening http or https links externally. This can either be the name of the browser (`edge`, `chrome`, `firefox`) or an absolute path to the browser's executable. Will use the system default if not set.
	"workbench.externalBrowser": "",

	// Configure the opener to use for external URIs (http, https).
	"workbench.externalUriOpeners": {},

	// Controls the delay in milliseconds after which the hover is shown for workbench items (ex. some extension provided tree view items). Already visible items may require a refresh before reflecting this setting change.
	"workbench.hover.delay": 500,

	// Specifies the file icon theme used in the workbench or 'null' to not show any file icons.
	//  - null: No file icons
	//  - vs-minimal
	//  - vs-seti
	"workbench.iconTheme": "vs-seti",

	// Controls whether the layout control is shown in the custom title bar. This setting only has an effect when `window.customTitleBarVisibility` is not set to `never`.
	"workbench.layoutControl.enabled": true,

	// Controls whether the layout control in the custom title bar is displayed as a single menu button or with multiple UI toggles.
	//  - menu: Shows a single button with a dropdown of layout options.
	//  - toggles: Shows several buttons for toggling the visibility of the panels and side bar.
	//  - both: Shows both the dropdown and toggle buttons.
	"workbench.layoutControl.type": "both",

	// Controls the type of matching used when searching lists and trees in the workbench.
	//  - fuzzy: Use fuzzy matching when searching.
	//  - contiguous: Use contiguous matching when searching.
	"workbench.list.defaultFindMatchType": "fuzzy",

	// Controls the default find mode for lists and trees in the workbench.
	//  - highlight: Highlight elements when searching. Further up and down navigation will traverse only the highlighted elements.
	//  - filter: Filter elements when searching.
	"workbench.list.defaultFindMode": "highlight",

	// Scrolling speed multiplier when pressing `Alt`.
	"workbench.list.fastScrollSensitivity": 5,

	// Controls whether lists and trees support horizontal scrolling in the workbench. Warning: turning on this setting has a performance implication.
	"workbench.list.horizontalScrolling": false,

	// Please use 'workbench.list.defaultFindMode' and	'workbench.list.typeNavigationMode' instead.
	// Controls the keyboard navigation style for lists and trees in the workbench. Can be simple, highlight and filter.
	//  - simple: Simple keyboard navigation focuses elements which match the keyboard input. Matching is done only on prefixes.
	//  - highlight: Highlight keyboard navigation highlights elements which match the keyboard input. Further up and down navigation will traverse only the highlighted elements.
	//  - filter: Filter keyboard navigation will filter out and hide all the elements which do not match the keyboard input.
	"workbench.list.keyboardNavigation": "highlight",

	// A multiplier to be used on the `deltaX` and `deltaY` of mouse wheel scroll events.
	"workbench.list.mouseWheelScrollSensitivity": 1,

	// The modifier to be used to add an item in trees and lists to a multi-selection with the mouse (for example in the explorer, open editors and scm view). The 'Open to Side' mouse gestures - if supported - will adapt such that they do not conflict with the multiselect modifier.
	//  - ctrlCmd: Maps to `Control` on Windows and Linux and to `Command` on macOS.
	//  - alt: Maps to `Alt` on Windows and Linux and to `Option` on macOS.
	"workbench.list.multiSelectModifier": "ctrlCmd",

	// Controls how to open items in trees and lists using the mouse (if supported). Note that some trees and lists might choose to ignore this setting if it is not applicable.
	"workbench.list.openMode": "singleClick",

	// Controls whether clicks in the scrollbar scroll page by page.
	"workbench.list.scrollByPage": false,

	// Controls whether lists and trees have smooth scrolling.
	"workbench.list.smoothScrolling": false,

	// Controls how type navigation works in lists and trees in the workbench. When set to `trigger`, type navigation begins once the `list.triggerTypeNavigation` command is run.
	"workbench.list.typeNavigationMode": "automatic",

	// Controls whether local file history is enabled. When enabled, the file contents of an editor that is saved will be stored to a backup location to be able to restore or review the contents later. Changing this setting has no effect on existing local file history entries.
	"workbench.localHistory.enabled": true,

	// Configure paths or [glob patterns](https://aka.ms/vscode-glob-patterns) for excluding files from the local file history. Glob patterns are always evaluated relative to the path of the workspace folder unless they are absolute paths. Changing this setting has no effect on existing local file history entries.
	"workbench.localHistory.exclude": {},

	// Controls the maximum number of local file history entries per file. When the number of local file history entries exceeds this number for a file, the oldest entries will be discarded.
	"workbench.localHistory.maxFileEntries": 50,

	// Controls the maximum size of a file (in KB) to be considered for local file history. Files that are larger will not be added to the local file history. Changing this setting has no effect on existing local file history entries.
	"workbench.localHistory.maxFileSize": 256,

	// Configure an interval in seconds during which the last entry in local file history is replaced with the entry that is being added. This helps reduce the overall number of entries that are added, for example when auto save is enabled. This setting is only applied to entries that have the same source of origin. Changing this setting has no effect on existing local file history entries.
	"workbench.localHistory.mergeWindow": 10,

	// Controls whether the navigation control is shown in the custom title bar. This setting only has an effect when `window.customTitleBarVisibility` is not set to `never`.
	"workbench.navigationControl.enabled": true,

	// Controls the default location of the panel (Terminal, Debug Console, Output, Problems) in a new workspace. It can either show at the bottom, top, right, or left of the editor area.
	"workbench.panel.defaultLocation": "bottom",

	// Controls whether the panel opens maximized. It can either always open maximized, never open maximized, or open to the last state it was in before being closed.
	//  - always: Always maximize the panel when opening it.
	//  - never: Never maximize the panel when opening it. The panel will open un-maximized.
	//  - preserve: Open the panel to the state that it was in, before it was closed.
	"workbench.panel.opensMaximized": "preserve",

	// Controls whether activity items in the panel title are shown as label or icon.
	"workbench.panel.showLabels": true,

	// Specifies the color theme when system color mode is dark and `window.autoDetectColorScheme` is enabled.
	"workbench.preferredDarkColorTheme": "Default Dark Modern",

	// Specifies the color theme when in high contrast dark mode and `window.autoDetectHighContrast` is enabled.
	"workbench.preferredHighContrastColorTheme": "Default High Contrast",

	// Specifies the color theme when in high contrast light mode and `window.autoDetectHighContrast` is enabled.
	"workbench.preferredHighContrastLightColorTheme": "Default High Contrast Light",

	// Specifies the color theme when system color mode is light and `window.autoDetectColorScheme` is enabled.
	"workbench.preferredLightColorTheme": "Default Light Modern",

	// Specifies the product icon theme used.
	//  - Default: Default
	"workbench.productIconTheme": "Default",

	// Controls whether Quick Open should close automatically once it loses focus.
	"workbench.quickOpen.closeOnFocusLost": true,

	// Controls whether the last typed input to Quick Open should be restored when opening it the next time.
	"workbench.quickOpen.preserveInput": false,

	// Controls whether the workbench should render with fewer animations.
	//  - on: Always render with reduced motion.
	//  - off: Do not render with reduced motion
	//  - auto: Render with reduced motion based on OS configuration.
	"workbench.reduceMotion": "auto",

	// When enabled, remote extensions recommendations will be shown in the Remote Indicator menu.
	"workbench.remoteIndicator.showExtensionRecommendations": true,

	// Controls the hover feedback delay in milliseconds of the dragging area in between views/editors.
	"workbench.sash.hoverDelay": 300,

	// Controls the feedback area size in pixels of the dragging area in between views/editors. Set it to a larger value if you feel it's hard to resize views using the mouse.
	"workbench.sash.size": 4,

	// Configure settings to be applied for all profiles.
	"workbench.settings.applyToAllProfiles": [],

	// Determines which settings editor to use by default.
	//  - ui: Use the settings UI editor.
	//  - json: Use the JSON file editor.
	"workbench.settings.editor": "ui",

	// Controls whether to enable the natural language search mode for settings. The natural language search is provided by a Microsoft online service.
	"workbench.settings.enableNaturalLanguageSearch": true,

	// Controls whether opening keybinding settings also opens an editor showing all default keybindings.
	"workbench.settings.openDefaultKeybindings": false,

	// Controls whether opening settings also opens an editor showing all default settings.
	"workbench.settings.openDefaultSettings": false,

	// Controls the behavior of the Settings editor Table of Contents while searching. If this setting is being changed in the Settings editor, the setting will take effect after the search query is modified.
	//  - hide: Hide the Table of Contents while searching.
	//  - filter: Filter the Table of Contents to just categories that have matching settings. Clicking on a category will filter the results to that category.
	"workbench.settings.settingsSearchTocBehavior": "filter",

	// Controls whether to use the split JSON editor when editing settings as JSON.
	"workbench.settings.useSplitJSON": false,

	// Controls whether to use an experimental ranking algorithm for search results in the Settings editor. The newer algorithm is still in development and aims to show fewer and more relevant results.
	"workbench.settings.useWeightedKeySearch": false,

	// Controls the location of the primary side bar and activity bar. They can either show on the left or right of the workbench. The secondary side bar will show on the opposite side of the workbench.
	"workbench.sideBar.location": "left",

	// Controls which editor is shown at startup, if none are restored from the previous session.
	//  - none: Start without an editor.
	//  - welcomePage: Open the Welcome page, with content to aid in getting started with VS Code and extensions.
	//  - readme: Open the README when opening a folder that contains one, fallback to 'welcomePage' otherwise. Note: This is only observed as a global configuration, it will be ignored if set in a workspace or folder configuration.
	//  - newUntitledFile: Open a new untitled text file (only applies when opening an empty window).
	//  - welcomePageInEmptyWorkbench: Open the Welcome page when opening an empty workbench.
	//  - terminal: Open a new terminal in the editor area.
	"workbench.startupEditor": "welcomePage",

	// Controls the visibility of the status bar at the bottom of the workbench.
	"workbench.statusBar.visible": true,

	// When enabled, will show the watermark tips when no editor is open.
	"workbench.tips.enabled": true,

	// Controls whether sticky scrolling is enabled in trees.
	"workbench.tree.enableStickyScroll": true,

	// Controls how tree folders are expanded when clicking the folder names. Note that some trees and lists might choose to ignore this setting if it is not applicable.
	"workbench.tree.expandMode": "singleClick",

	// Controls tree indentation in pixels.
	"workbench.tree.indent": 8,

	// Controls whether the tree should render indent guides.
	"workbench.tree.renderIndentGuides": "onHover",

	// Controls the number of sticky elements displayed in the tree when `workbench.tree.enableStickyScroll` is enabled.
	"workbench.tree.stickyScrollMaxItemCount": 7,

	// When enabled, trusted domain prompts will appear when opening links in trusted workspaces.
	"workbench.trustedDomains.promptInTrustedWorkspace": false,

	// Controls the visibility of view header actions. View header actions may either be always visible, or only visible when that view is focused or hovered over.
	"workbench.view.alwaysShowHeaderActions": false,

	// If an extension requests a hidden view to be shown, display a clickable status bar indicator instead.
	"workbench.view.showQuietly": {},

	// Deprecated, use the global `workbench.reduceMotion`.
	// When enabled, reduce motion in welcome page.
	"workbench.welcomePage.preferReducedMotion": false,

	// When enabled, an extension's walkthrough will open upon install of the extension.
	"workbench.welcomePage.walkthroughs.openOnInstall": true,

	// If enabled, will automatically select a color theme based on the system color mode. If the system color mode is dark, `workbench.preferredDarkColorTheme#` is used, else `#workbench.preferredLightColorTheme`.
	"window.autoDetectColorScheme": false,

	// If enabled, will automatically change to high contrast theme if the OS is using a high contrast theme. The high contrast theme to use is specified by `workbench.preferredHighContrastColorTheme#` and `#workbench.preferredHighContrastLightColorTheme`.
	"window.autoDetectHighContrast": true,

	// Controls whether closing the last editor should also close the window. This setting only applies for windows that do not show folders.
	"window.closeWhenEmpty": false,

	// Show command launcher together with the window title. This setting only has an effect when `window.customTitleBarVisibility` is not set to `never`.
	"window.commandCenter": true,

	// Controls whether to show a confirmation dialog before closing a window or quitting the application.
	//  - always: Always ask for confirmation.
	//  - keyboardOnly: Only ask for confirmation if a keybinding was used.
	//  - never: Never explicitly ask for confirmation.
	"window.confirmBeforeClose": "never",

	// Controls whether a confirmation dialog shows asking to save or discard an opened untitled workspace in the window when switching to another workspace. Disabling the confirmation dialog will always discard the untitled workspace.
	"window.confirmSaveUntitledWorkspace": true,

	// Controls whether the menu bar will be focused by pressing the Alt-key. This setting has no effect on toggling the menu bar with the Alt-key.
	"window.customMenuBarAltFocus": true,

	// Adjust when the custom title bar should be shown. The custom title bar can be hidden when in full screen mode with `windowed`. The custom title bar can only be hidden in non full screen mode with `never` when `window.titleBarStyle` is set to `native`.
	//  - auto: Automatically changes custom title bar visibility.
	//  - windowed: Hide custom titlebar in full screen. When not in full screen, automatically change custom title bar visibility.
	//  - never: Hide custom titlebar when `window.titleBarStyle` is set to `native`.
	"window.customTitleBarVisibility": "auto",

	// Adjust the appearance of dialog windows.
	"window.dialogStyle": "native",

	// If enabled, this setting will close the window when the application icon in the title bar is double-clicked. The window will not be able to be dragged by the icon. This setting is effective only if `window.titleBarStyle` is set to `custom`.
	"window.doubleClickIconToClose": false,

	// Controls whether the main menus can be opened via Alt-key shortcuts. Disabling mnemonics allows to bind these Alt-key shortcuts to editor commands instead.
	"window.enableMenuBarMnemonics": true,

	// Control the visibility of the menu bar. A setting of 'toggle' means that the menu bar is hidden and a single press of the Alt key will show it. A setting of 'compact' will move the menu into the side bar.
	//  - classic: Menu is displayed at the top of the window and only hidden in full screen mode.
	//  - visible: Menu is always visible at the top of the window even in full screen mode.
	//  - toggle: Menu is hidden but can be displayed at the top of the window via the Alt key.
	//  - hidden: Menu is always hidden.
	//  - compact: Menu is displayed as a compact button in the side bar. This value is ignored when `window.titleBarStyle` is `native`.
	"window.menuBarVisibility": "classic",

	// Controls the dimensions of opening a new window when at least one window is already opened. Note that this setting does not have an impact on the first window that is opened. The first window will always restore the size and location as you left it before closing.
	//  - default: Open new windows in the center of the screen.
	//  - inherit: Open new windows with same dimension as last active one.
	//  - offset: Open new windows with same dimension as last active one with an offset position.
	//  - maximized: Open new windows maximized.
	//  - fullscreen: Open new windows in full screen mode.
	"window.newWindowDimensions": "default",

	// Specifies the profile to use when opening a new window. If a profile name is provided, the new window will use that profile. If no profile name is provided, the new window will use the profile of the active window or the Default profile if no active window exists.
	"window.newWindowProfile": null,

	// Controls whether files should open in a new window when using a command line or file dialog.
	// Note that there can still be cases where this setting is ignored (e.g. when using the `--new-window` or `--reuse-window` command line option).
	//  - on: Files will open in a new window.
	//  - off: Files will open in the window with the files' folder open or the last active window.
	//  - default: Files will open in a new window unless picked from within the application (e.g. via the File menu).
	"window.openFilesInNewWindow": "off",

	// Controls whether folders should open in a new window or replace the last active window.
	// Note that there can still be cases where this setting is ignored (e.g. when using the `--new-window` or `--reuse-window` command line option).
	//  - on: Folders will open in a new window.
	//  - off: Folders will replace the last active window.
	//  - default: Folders will open in a new window unless a folder is picked from within the application (e.g. via the File menu).
	"window.openFoldersInNewWindow": "default",

	// Controls whether a new empty window should open when starting a second instance without arguments or if the last running instance should get focus.
	// Note that there can still be cases where this setting is ignored (e.g. when using the `--new-window` or `--reuse-window` command line option).
	//  - on: Open a new empty window.
	//  - off: Focus the last active running instance.
	"window.openWithoutArgumentsInNewWindow": "on",

	// Controls whether a window should restore to full screen mode if it was exited in full screen mode.
	"window.restoreFullscreen": false,

	// Controls how windows and editors within are being restored when opening.
	//  - preserve: Always reopen all windows. If a folder or workspace is opened (e.g. from the command line) it opens as a new window unless it was opened before. If files are opened they will open in one of the restored windows together with editors that were previously opened.
	//  - all: Reopen all windows unless a folder, workspace or file is opened (e.g. from the command line). If a file is opened, it will replace any of the editors that were previously opened in a window.
	//  - folders: Reopen all windows that had folders or workspaces opened unless a folder, workspace or file is opened (e.g. from the command line). If a file is opened, it will replace any of the editors that were previously opened in a window.
	//  - one: Reopen the last active window unless a folder, workspace or file is opened (e.g. from the command line). If a file is opened, it will replace any of the editors that were previously opened in a window.
	//  - none: Never reopen a window. Unless a folder or workspace is opened (e.g. from the command line), an empty window will appear.
	"window.restoreWindows": "all",

	// Controls the window title based on the current context such as the opened workspace or active editor. Variables are substituted based on the context:
	// - `${activeEditorShort}`: the file name (e.g. myFile.txt).
	// - `${activeEditorMedium}`: the path of the file relative to the workspace folder (e.g. myFolder/myFileFolder/myFile.txt).
	// - `${activeEditorLong}`: the full path of the file (e.g. /Users/Development/myFolder/myFileFolder/myFile.txt).
	// - `${activeFolderShort}`: the name of the folder the file is contained in (e.g. myFileFolder).
	// - `${activeFolderMedium}`: the path of the folder the file is contained in, relative to the workspace folder (e.g. myFolder/myFileFolder).
	// - `${activeFolderLong}`: the full path of the folder the file is contained in (e.g. /Users/Development/myFolder/myFileFolder).
	// - `${folderName}`: name of the workspace folder the file is contained in (e.g. myFolder).
	// - `${folderPath}`: file path of the workspace folder the file is contained in (e.g. /Users/Development/myFolder).
	// - `${rootName}`: name of the workspace with optional remote name and workspace indicator if applicable (e.g. myFolder, myRemoteFolder [SSH] or myWorkspace (Workspace)).
	// - `${rootNameShort}`: shortened name of the workspace without suffixes (e.g. myFolder, myRemoteFolder or myWorkspace).
	// - `${rootPath}`: file path of the opened workspace or folder (e.g. /Users/Development/myWorkspace).
	// - `${profileName}`: name of the profile in which the workspace is opened (e.g. Data Science (Profile)). Ignored if default profile is used.
	// - `${appName}`: e.g. VS Code.
	// - `${remoteName}`: e.g. SSH
	// - `${dirty}`: an indicator for when the active editor has unsaved changes.
	// - `${focusedView}`: the name of the view that is currently focused.
	// - `${activeRepositoryName}`: the name of the active repository (e.g. vscode).
	// - `${activeRepositoryBranchName}`: the name of the active branch in the active repository (e.g. main).
	// - `${separator}`: a conditional separator (" - ") that only shows when surrounded by variables with values or static text.
	"window.title": "${dirty}${activeEditorShort}${separator}${rootName}${separator}${profileName}${separator}${appName}",

	// Adjust the appearance of the window title bar to be native by the OS or custom. On Linux and Windows, this setting also affects the application and context menu appearances. Changes require a full restart to apply.
	"window.titleBarStyle": "custom",

	// Separator used by `window.title`.
	"window.titleSeparator": " - ",

	// Adjust the default zoom level for all windows. Each increment above `0` (e.g. `1`) or below (e.g. `-1`) represents zooming `20%` larger or smaller. You can also enter decimals to adjust the zoom level with a finer granularity. See `window.zoomPerWindow` for configuring if the 'Zoom In' and 'Zoom Out' commands apply the zoom level to all windows or only the active window.
	"window.zoomLevel": 0,

	// Controls if the 'Zoom In' and 'Zoom Out' commands apply the zoom level to all windows or only the active window. See `window.zoomLevel` for configuring a default zoom level for all windows.
	"window.zoomPerWindow": true,

	// Configure [glob patterns](https://aka.ms/vscode-glob-patterns) of file associations to languages (for example `"*.extension": "html"`). Patterns will match on the absolute path of a file if they contain a path separator and will match on the name of the file otherwise. These have precedence over the default associations of the languages installed.
	"files.associations": {},

	// When enabled, the editor will attempt to guess the character set encoding when opening files. This setting can also be configured per language. Note, this setting is not respected by text search. Only `files.encoding` is respected.
	"files.autoGuessEncoding": false,

	// Controls [auto save](https://code.visualstudio.com/docs/editor/codebasics#_save-auto-save) of editors that have unsaved changes.
	//  - off: An editor with changes is never automatically saved.
	//  - afterDelay: An editor with changes is automatically saved after the configured `files.autoSaveDelay`.
	//  - onFocusChange: An editor with changes is automatically saved when the editor loses focus.
	//  - onWindowChange: An editor with changes is automatically saved when the window loses focus.
	"files.autoSave": "off",

	// Controls the delay in milliseconds after which an editor with unsaved changes is saved automatically. Only applies when `files.autoSave` is set to `afterDelay`.
	"files.autoSaveDelay": 1000,

	// When enabled, will limit [auto save](https://code.visualstudio.com/docs/editor/codebasics#_save-auto-save) of editors to files that have no errors reported in them at the time the auto save is triggered. Only applies when `files.autoSave` is enabled.
	"files.autoSaveWhenNoErrors": false,

	// When enabled, will limit [auto save](https://code.visualstudio.com/docs/editor/codebasics#_save-auto-save) of editors to files that are inside the opened workspace. Only applies when `files.autoSave` is enabled.
	"files.autoSaveWorkspaceFilesOnly": false,

	// List of character set encodings that the editor should attempt to guess in the order they are listed. In case it cannot be determined, `files.encoding` is respected
	//  - utf8: UTF-8
	//  - utf16le: UTF-16 LE
	//  - utf16be: UTF-16 BE
	//  - windows1252: Western (Windows 1252)
	//  - windows1250: Central European (Windows 1250)
	//  - iso88592: Central European (ISO 8859-2)
	//  - windows1251: Cyrillic (Windows 1251)
	//  - cp866: Cyrillic (CP 866)
	//  - cp1125: Cyrillic (CP 1125)
	//  - iso88595: Cyrillic (ISO 8859-5)
	//  - koi8r: Cyrillic (KOI8-R)
	//  - windows1253: Greek (Windows 1253)
	//  - iso88597: Greek (ISO 8859-7)
	//  - windows1255: Hebrew (Windows 1255)
	//  - iso88598: Hebrew (ISO 8859-8)
	//  - cp950: Traditional Chinese (Big5)
	//  - shiftjis: Japanese (Shift JIS)
	//  - eucjp: Japanese (EUC-JP)
	//  - euckr: Korean (EUC-KR)
	//  - gb2312: Simplified Chinese (GB 2312)
	"files.candidateGuessEncodings": [],

	// The default language identifier that is assigned to new files. If configured to `${activeEditorLanguage}`, will use the language identifier of the currently active text editor if any.
	"files.defaultLanguage": "",

	// Default path for file dialogs, overriding user's home path. Only used in the absence of a context-specific path, such as most recently opened file or folder.
	"files.dialog.defaultPath": "",

	// Moves files/folders to the OS trash (recycle bin on Windows) when deleting. Disabling this will delete files/folders permanently.
	"files.enableTrash": true,

	// The default character set encoding to use when reading and writing files. This setting can also be configured per language.
	//  - utf8: UTF-8
	//  - utf8bom: UTF-8 with BOM
	//  - utf16le: UTF-16 LE
	//  - utf16be: UTF-16 BE
	//  - windows1252: Western (Windows 1252)
	//  - iso88591: Western (ISO 8859-1)
	//  - iso88593: Western (ISO 8859-3)
	//  - iso885915: Western (ISO 8859-15)
	//  - macroman: Western (Mac Roman)
	//  - cp437: DOS (CP 437)
	//  - windows1256: Arabic (Windows 1256)
	//  - iso88596: Arabic (ISO 8859-6)
	//  - windows1257: Baltic (Windows 1257)
	//  - iso88594: Baltic (ISO 8859-4)
	//  - iso885914: Celtic (ISO 8859-14)
	//  - windows1250: Central European (Windows 1250)
	//  - iso88592: Central European (ISO 8859-2)
	//  - cp852: Central European (CP 852)
	//  - windows1251: Cyrillic (Windows 1251)
	//  - cp866: Cyrillic (CP 866)
	//  - cp1125: Cyrillic (CP 1125)
	//  - iso88595: Cyrillic (ISO 8859-5)
	//  - koi8r: Cyrillic (KOI8-R)
	//  - koi8u: Cyrillic (KOI8-U)
	//  - iso885913: Estonian (ISO 8859-13)
	//  - windows1253: Greek (Windows 1253)
	//  - iso88597: Greek (ISO 8859-7)
	//  - windows1255: Hebrew (Windows 1255)
	//  - iso88598: Hebrew (ISO 8859-8)
	//  - iso885910: Nordic (ISO 8859-10)
	//  - iso885916: Romanian (ISO 8859-16)
	//  - windows1254: Turkish (Windows 1254)
	//  - iso88599: Turkish (ISO 8859-9)
	//  - windows1258: Vietnamese (Windows 1258)
	//  - gbk: Simplified Chinese (GBK)
	//  - gb18030: Simplified Chinese (GB18030)
	//  - cp950: Traditional Chinese (Big5)
	//  - big5hkscs: Traditional Chinese (Big5-HKSCS)
	//  - shiftjis: Japanese (Shift JIS)
	//  - eucjp: Japanese (EUC-JP)
	//  - euckr: Korean (EUC-KR)
	//  - windows874: Thai (Windows 874)
	//  - iso885911: Latin/Thai (ISO 8859-11)
	//  - koi8ru: Cyrillic (KOI8-RU)
	//  - koi8t: Tajik (KOI8-T)
	//  - gb2312: Simplified Chinese (GB 2312)
	//  - cp865: Nordic DOS (CP 865)
	//  - cp850: Western European DOS (CP 850)
	"files.encoding": "utf8",

	// The default end of line character.
	//  - \n: LF
	//  - \r\n: CRLF
	//  - auto: Uses operating system specific end of line character.
	"files.eol": "auto",

	// Configure [glob patterns](https://aka.ms/vscode-glob-patterns) for excluding files and folders. For example, the File Explorer decides which files and folders to show or hide based on this setting. Refer to the `search.exclude#` setting to define search-specific excludes. Refer to the `#explorer.excludeGitIgnore` setting for ignoring files based on your `.gitignore`.
	"files.exclude": {
		"**/.git": true,
		"**/.svn": true,
		"**/.hg": true,
		"**/CVS": true,
		"**/.DS_Store": true,
		"**/Thumbs.db": true
	},

	// [Hot Exit](https://aka.ms/vscode-hot-exit) controls whether unsaved files are remembered between sessions, allowing the save prompt when exiting the editor to be skipped.
	//  - off: Disable hot exit. A prompt will show when attempting to close a window with editors that have unsaved changes.
	//  - onExit: Hot exit will be triggered when the last window is closed on Windows/Linux or when the `workbench.action.quit` command is triggered (command palette, keybinding, menu). All windows without folders opened will be restored upon next launch. A list of previously opened windows with unsaved files can be accessed via `File > Open Recent > More...`
	//  - onExitAndWindowClose: Hot exit will be triggered when the last window is closed on Windows/Linux or when the `workbench.action.quit` command is triggered (command palette, keybinding, menu), and also for any window with a folder opened regardless of whether it's the last window. All windows without folders opened will be restored upon next launch. A list of previously opened windows with unsaved files can be accessed via `File > Open Recent > More...`
	"files.hotExit": "onExit",

	// When enabled, insert a final new line at the end of the file when saving it.
	"files.insertFinalNewline": false,

	// Timeout in milliseconds after which file participants for create, rename, and delete are cancelled. Use `0` to disable participants.
	"files.participants.timeout": 60000,

	// Configure paths or [glob patterns](https://aka.ms/vscode-glob-patterns) to exclude from being marked as read-only if they match as a result of the `files.readonlyInclude` setting. Glob patterns are always evaluated relative to the path of the workspace folder unless they are absolute paths. Files from readonly file system providers will always be read-only independent of this setting.
	"files.readonlyExclude": {},

	// Marks files as read-only when their file permissions indicate as such. This can be overridden via `files.readonlyInclude#` and `#files.readonlyExclude` settings.
	"files.readonlyFromPermissions": false,

	// Configure paths or [glob patterns](https://aka.ms/vscode-glob-patterns) to mark as read-only. Glob patterns are always evaluated relative to the path of the workspace folder unless they are absolute paths. You can exclude matching paths via the `files.readonlyExclude` setting. Files from readonly file system providers will always be read-only independent of this setting.
	"files.readonlyInclude": {},

	// Controls if files that were part of a refactoring are saved automatically
	"files.refactoring.autoSave": true,

	// Restore the undo stack when a file is reopened.
	"files.restoreUndoStack": true,

	// A save conflict can occur when a file is saved to disk that was changed by another program in the meantime. To prevent data loss, the user is asked to compare the changes in the editor with the version on disk. This setting should only be changed if you frequently encounter save conflict errors and may result in data loss if used without caution.
	//  - askUser: Will refuse to save and ask for resolving the save conflict manually.
	//  - overwriteFileOnDisk: Will resolve the save conflict by overwriting the file on disk with the changes in the editor.
	"files.saveConflictResolution": "askUser",

	// Enables the simple file dialog for opening and saving files and folders. The simple file dialog replaces the system file dialog when enabled.
	"files.simpleDialog.enable": false,

	// When enabled, will trim all new lines after the final new line at the end of the file when saving it.
	"files.trimFinalNewlines": false,

	// When enabled, will trim trailing whitespace when saving a file.
	"files.trimTrailingWhitespace": false,

	// When enabled, trailing whitespace will be removed from multiline strings and regexes will be removed on save or when executing 'editor.action.trimTrailingWhitespace'. This can cause whitespace to not be trimmed from lines when there isn't up-to-date token information.
	"files.trimTrailingWhitespaceInRegexAndStrings": true,

	// Configure paths or [glob patterns](https://aka.ms/vscode-glob-patterns) to exclude from file watching. Paths can either be relative to the watched folder or absolute. Glob patterns are matched relative from the watched folder. When you experience the file watcher process consuming a lot of CPU, make sure to exclude large folders that are of less interest (such as build output folders).
	"files.watcherExclude": {
		"**/.git/objects/**": true,
		"**/.git/subtree-cache/**": true,
		"**/.hg/store/**": true
	},

	// Configure extra paths to watch for changes inside the workspace. By default, all workspace folders will be watched recursively, except for folders that are symbolic links. You can explicitly add absolute or relative paths to support watching folders that are symbolic links. Relative paths will be resolved to an absolute path using the currently opened workspace.
	"files.watcherInclude": [],

	// Controls the font size (in pixels) of the screencast mode keyboard.
	"screencastMode.fontSize": 56,

	// Options for customizing the keyboard overlay in screencast mode.
	"screencastMode.keyboardOptions": {
		"showKeys": true,
		"showKeybindings": true,
		"showCommands": true,
		"showCommandGroups": false,
		"showSingleEditorCursorMoves": true
	},

	// Controls how long (in milliseconds) the keyboard overlay is shown in screencast mode.
	"screencastMode.keyboardOverlayTimeout": 800,

	// Controls the color in hex (#RGB, #RGBA, #RRGGBB or #RRGGBBAA) of the mouse indicator in screencast mode.
	"screencastMode.mouseIndicatorColor": "#FF0000",

	// Controls the size (in pixels) of the mouse indicator in screencast mode.
	"screencastMode.mouseIndicatorSize": 20,

	// Controls the vertical offset of the screencast mode overlay from the bottom as a percentage of the workbench height.
	"screencastMode.verticalOffset": 20,

	// Controls whether turning on Zen Mode also centers the layout.
	"zenMode.centerLayout": true,

	// Controls whether turning on Zen Mode also puts the workbench into full screen mode.
	"zenMode.fullScreen": true,

	// Controls whether turning on Zen Mode also hides the activity bar either at the left or right of the workbench.
	"zenMode.hideActivityBar": true,

	// Controls whether turning on Zen Mode also hides the editor line numbers.
	"zenMode.hideLineNumbers": true,

	// Controls whether turning on Zen Mode also hides the status bar at the bottom of the workbench.
	"zenMode.hideStatusBar": true,

	// Controls whether a window should restore to Zen Mode if it was exited in Zen Mode.
	"zenMode.restore": true,

	// Controls whether turning on Zen Mode should show multiple editor tabs, a single editor tab, or hide the editor title area completely.
	//  - multiple: Each editor is displayed as a tab in the editor title area.
	//  - single: The active editor is displayed as a single large tab in the editor title area.
	//  - none: The editor title area is not displayed.
	"zenMode.showTabs": "multiple",

	// Controls whether notifications do not disturb mode should be enabled while in Zen Mode. If true, only error notifications will pop out.
	"zenMode.silentNotifications": true,

	// Controls whether the Explorer should automatically open a file when it is dropped into the explorer
	"explorer.autoOpenDroppedFile": true,

	// Controls whether the Explorer should automatically reveal and select files when opening them.
	//  - true: Files will be revealed and selected.
	//  - false: Files will not be revealed and selected.
	//  - focusNoScroll: Files will not be scrolled into view, but will still be focused.
	"explorer.autoReveal": true,

	// Configure paths or [glob patterns](https://aka.ms/vscode-glob-patterns) for excluding files and folders from being revealed and selected in the Explorer when they are opened. Glob patterns are always evaluated relative to the path of the workspace folder unless they are absolute paths.
	"explorer.autoRevealExclude": {
		"**/node_modules": true,
		"**/bower_components": true
	},

	// Controls whether the Explorer should render folders in a compact form. In such a form, single child folders will be compressed in a combined tree element. Useful for Java package structures, for example.
	"explorer.compactFolders": true,

	// Controls whether the Explorer should ask for confirmation when deleting a file via the trash.
	"explorer.confirmDelete": true,

	// Controls whether the Explorer should ask for confirmation to move files and folders via drag and drop.
	"explorer.confirmDragAndDrop": true,

	// Controls whether the Explorer should ask for confirmation when pasting native files and folders.
	"explorer.confirmPasteNative": true,

	// Controls whether the Explorer should ask for confirmation when undoing.
	//  - verbose: Explorer will prompt before all undo operations.
	//  - default: Explorer will prompt before destructive undo operations.
	//  - light: Explorer will not prompt before undo operations when focused.
	"explorer.confirmUndo": "default",

	// The path separation character used when copying relative file paths.
	//  - /: Use slash as path separation character.
	//  - \: Use backslash as path separation character.
	//  - auto: Uses operating system specific path separation character.
	"explorer.copyRelativePathSeparator": "auto",

	// Controls whether file decorations should use badges.
	"explorer.decorations.badges": true,

	// Controls whether file decorations should use colors.
	"explorer.decorations.colors": true,

	// Controls whether the Explorer should allow to move files and folders via drag and drop. This setting only effects drag and drop from inside the Explorer.
	"explorer.enableDragAndDrop": true,

	// Controls whether the Explorer should support undoing file and folder operations.
	"explorer.enableUndo": true,

	// Controls whether entries in .gitignore should be parsed and excluded from the Explorer. Similar to `files.exclude`.
	"explorer.excludeGitIgnore": false,

	// Controls whether the Explorer should expand multi-root workspaces containing only one folder during initialization
	"explorer.expandSingleFolderWorkspaces": true,

	// Controls whether file nesting is enabled in the Explorer. File nesting allows for related files in a directory to be visually grouped together under a single parent file.
	"explorer.fileNesting.enabled": false,

	// Controls whether file nests are automatically expanded. `explorer.fileNesting.enabled` must be set for this to take effect.
	"explorer.fileNesting.expand": true,

	// Controls nesting of files in the Explorer. `explorer.fileNesting.enabled` must be set for this to take effect. Each __Item__ represents a parent pattern and may contain a single `*` character that matches any string. Each __Value__ represents a comma separated list of the child patterns that should be shown nested under a given parent. Child patterns may contain several special tokens:
	// - `${capture}`: Matches the resolved value of the `*` from the parent pattern
	// - `${basename}`: Matches the parent file's basename, the `file` in `file.ts`
	// - `${extname}`: Matches the parent file's extension, the `ts` in `file.ts`
	// - `${dirname}`: Matches the parent file's directory name, the `src` in `src/file.ts`
	// - `*`:  Matches any string, may only be used once per child pattern
	"explorer.fileNesting.patterns": {
		"*.ts": "${capture}.js",
		"*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts",
		"*.jsx": "${capture}.js",
		"*.tsx": "${capture}.ts",
		"tsconfig.json": "tsconfig.*.json",
		"package.json": "package-lock.json, yarn.lock, pnpm-lock.yaml, bun.lockb, bun.lock"
	},

	// Controls which naming strategy to use when giving a new name to a duplicated Explorer item on paste.
	//  - simple: Appends the word "copy" at the end of the duplicated name potentially followed by a number.
	//  - smart: Adds a number at the end of the duplicated name. If some number is already part of the name, tries to increase that number.
	//  - disabled: Disables incremental naming. If two files with the same name exist you will be prompted to overwrite the existing file.
	"explorer.incrementalNaming": "simple",

	// The minimum number of editor slots pre-allocated in the Open Editors pane. If set to 0 the Open Editors pane will dynamically resize based on the number of editors.
	"explorer.openEditors.minVisible": 0,

	// Controls the sorting order of editors in the Open Editors pane.
	//  - editorOrder: Editors are ordered in the same order editor tabs are shown.
	//  - alphabetical: Editors are ordered alphabetically by tab name inside each editor group.
	//  - fullPath: Editors are ordered alphabetically by full path inside each editor group.
	"explorer.openEditors.sortOrder": "editorOrder",

	// The initial maximum number of editors shown in the Open Editors pane. Exceeding this limit will show a scroll bar and allow resizing the pane to display more items.
	"explorer.openEditors.visible": 9,

	// Controls the property-based sorting of files and folders in the Explorer. When `explorer.fileNesting.enabled` is enabled, also controls sorting of nested files.
	//  - default: Files and folders are sorted by their names. Folders are displayed before files.
	//  - mixed: Files and folders are sorted by their names. Files are interwoven with folders.
	//  - filesFirst: Files and folders are sorted by their names. Files are displayed before folders.
	//  - type: Files and folders are grouped by extension type then sorted by their names. Folders are displayed before files.
	//  - modified: Files and folders are sorted by last modified date in descending order. Folders are displayed before files.
	//  - foldersNestsFiles: Files and folders are sorted by their names. Folders are displayed before files. Files with nested children are displayed before other files.
	"explorer.sortOrder": "default",

	// Controls the lexicographic sorting of file and folder names in the Explorer.
	//  - default: Uppercase and lowercase names are mixed together.
	//  - upper: Uppercase names are grouped together before lowercase names.
	//  - lower: Lowercase names are grouped together before uppercase names.
	//  - unicode: Names are sorted in Unicode order.
	"explorer.sortOrderLexicographicOptions": "default",

	// Controls whether the file and folder sort order, should be reversed.
	"explorer.sortOrderReverse": false,

	// Controls the positioning of the actionbar on rows in the search view.
	//  - auto: Position the actionbar to the right when the search view is narrow, and immediately after the content when the search view is wide.
	//  - right: Always position the actionbar to the right.
	"search.actionsPosition": "right",

	// Controls whether the search results will be collapsed or expanded.
	//  - auto: Files with less than 10 results are expanded. Others are collapsed.
	//  - alwaysCollapse
	//  - alwaysExpand
	"search.collapseResults": "alwaysExpand",

	// Controls whether search file decorations should use badges.
	"search.decorations.badges": true,

	// Controls whether search file decorations should use colors.
	"search.decorations.colors": true,

	// Controls the default search result view mode.
	//  - tree: Shows search results as a tree.
	//  - list: Shows search results as a list.
	"search.defaultViewMode": "list",

	// Configure [glob patterns](https://code.visualstudio.com/docs/editor/codebasics#_advanced-search-options) for excluding files and folders in fulltext searches and file search in quick open. To exclude files from the recently opened list in quick open, patterns must be absolute (for example `**/node_modules/**`). Inherits all glob patterns from the `files.exclude` setting.
	"search.exclude": {
		"**/node_modules": true,
		"**/bower_components": true,
		"**/*.code-search": true
	},

	// Show notebook editor rich content results for closed notebooks. Please refresh your search results after changing this setting.
	"search.experimental.closedNotebookRichContentResults": false,

	// Controls whether to follow symlinks while searching.
	"search.followSymlinks": true,

	// This setting is deprecated. You can drag the search icon to a new location instead.
	// Controls whether the search will be shown as a view in the sidebar or as a panel in the panel area for more horizontal space.
	"search.location": "sidebar",

	// The search cache is kept in the extension host which never shuts down, so this setting is no longer needed.
	// When enabled, the searchService process will be kept alive instead of being shut down after an hour of inactivity. This will keep the file search cache in memory.
	"search.maintainFileSearchCache": false,

	// Controls the maximum number of search results, this can be set to `null` (empty) to return unlimited results.
	"search.maxResults": 20000,

	// Controls where new `Search: Find in Files` and `Find in Folder` operations occur: either in the search view, or in a search editor.
	//  - view: Search in the search view, either in the panel or side bars.
	//  - reuseEditor: Search in an existing search editor if present, otherwise in a new search editor.
	//  - newEditor: Search in a new search editor.
	"search.mode": "view",

	// Controls whether the last typed input to Quick Search should be restored when opening it the next time.
	"search.quickAccess.preserveInput": false,

	// Controls sorting order of editor history in quick open when filtering.
	//  - default: History entries are sorted by relevance based on the filter value used. More relevant entries appear first.
	//  - recency: History entries are sorted by recency. More recently opened entries appear first.
	"search.quickOpen.history.filterSortOrder": "default",

	// Whether to include results from recently opened files in the file results for Quick Open.
	"search.quickOpen.includeHistory": true,

	// Whether to include results from a global symbol search in the file results for Quick Open.
	"search.quickOpen.includeSymbols": false,

	// Number of threads to use for searching. When set to 0, the engine automatically determines this value.
	"search.ripgrep.maxThreads": 0,

	// The default number of surrounding context lines to use when creating new Search Editors. If using `search.searchEditor.reusePriorSearchConfiguration`, this can be set to `null` (empty) to use the prior Search Editor's configuration.
	"search.searchEditor.defaultNumberOfContextLines": 1,

	// Configure effect of double-clicking a result in a search editor.
	//  - selectWord: Double-clicking selects the word under the cursor.
	//  - goToLocation: Double-clicking opens the result in the active editor group.
	//  - openLocationToSide: Double-clicking opens the result in the editor group to the side, creating one if it does not yet exist.
	"search.searchEditor.doubleClickBehaviour": "goToLocation",

	// When a search is triggered, focus the Search Editor results instead of the Search Editor input.
	"search.searchEditor.focusResultsOnSearch": false,

	// When enabled, new Search Editors will reuse the includes, excludes, and flags of the previously opened Search Editor.
	"search.searchEditor.reusePriorSearchConfiguration": false,

	// Configure effect of single-clicking a result in a search editor.
	//  - default: Single-clicking does nothing.
	//  - peekDefinition: Single-clicking opens a Peek Definition window.
	"search.searchEditor.singleClickBehaviour": "default",

	// Search all files as you type.
	"search.searchOnType": true,

	// When `search.searchOnType#` is enabled, controls the timeout in milliseconds between a character being typed and the search starting. Has no effect when `#search.searchOnType` is disabled.
	"search.searchOnTypeDebouncePeriod": 300,

	// Update the search query to the editor's selected text when focusing the search view. This happens either on click or when triggering the `workbench.views.search.focus` command.
	"search.seedOnFocus": false,

	// Enable seeding search from the word nearest the cursor when the active editor has no selection.
	"search.seedWithNearestWord": false,

	// Controls whether to show line numbers for search results.
	"search.showLineNumbers": false,

	// Search case-insensitively if the pattern is all lowercase, otherwise, search case-sensitively.
	"search.smartCase": false,

	// Controls sorting order of search results.
	//  - default: Results are sorted by folder and file names, in alphabetical order.
	//  - fileNames: Results are sorted by file names ignoring folder order, in alphabetical order.
	//  - type: Results are sorted by file extensions, in alphabetical order.
	//  - modified: Results are sorted by file last modified date, in descending order.
	//  - countDescending: Results are sorted by count per file, in descending order.
	//  - countAscending: Results are sorted by count per file, in ascending order.
	"search.sortOrder": "default",

	// Controls whether to use your global gitignore file (for example, from `$HOME/.config/git/ignore`) when searching for files. Requires `search.useIgnoreFiles` to be enabled.
	"search.useGlobalIgnoreFiles": false,

	// Controls whether to use `.gitignore` and `.ignore` files when searching for files.
	"search.useIgnoreFiles": true,

	// Controls whether to use `.gitignore` and `.ignore` files in parent directories when searching for files. Requires `search.useIgnoreFiles` to be enabled.
	"search.useParentIgnoreFiles": false,

	// Deprecated. PCRE2 will be used automatically when using regex features that are only supported by PCRE2.
	// Whether to use the PCRE2 regex engine in text search. This enables using some advanced regex features like lookahead and backreferences. However, not all PCRE2 features are supported - only features that are also supported by JavaScript.
	"search.usePCRE2": false,

	// Controls whether to open Replace Preview when selecting or replacing a match.
	"search.useReplacePreview": true,

	// Deprecated. Consider "search.usePCRE2" for advanced regex feature support.
	// This setting is deprecated and now falls back on "search.usePCRE2".
	"search.useRipgrep": true,

	// Controls whether use of Electron's fetch implementation instead of Node.js' should be enabled. All local extensions will get Electron's fetch implementation for the global fetch API.
	"http.electronFetch": false,

	// Controls whether experimental loading of CA certificates from the OS should be enabled. This uses a more general approach than the default implementation. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.experimental.systemCertificatesV2": false,

	// Controls whether Node.js' fetch implementation should be extended with additional support. Currently proxy support (`http.proxySupport#`) and system certificates (`#http.systemCertificates#`) are added when the corresponding settings are enabled. When during [remote development](https://aka.ms/vscode-remote) the `#http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.fetchAdditionalSupport": true,

	// Specifies domain names for which proxy settings should be ignored for HTTP/HTTPS requests. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.noProxy": [],

	// The proxy setting to use. If not set, will be inherited from the `http_proxy` and `https_proxy` environment variables. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.proxy": "",

	// The value to send as the `Proxy-Authorization` header for every network request. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.proxyAuthorization": null,

	// Overrides the principal service name for Kerberos authentication with the HTTP proxy. A default based on the proxy hostname is used when this is not set. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.proxyKerberosServicePrincipal": "",

	// Controls whether the proxy server certificate should be verified against the list of supplied CAs. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.proxyStrictSSL": true,

	// Use the proxy support for extensions. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	//  - off: Disable proxy support for extensions.
	//  - on: Enable proxy support for extensions.
	//  - fallback: Enable proxy support for extensions, fall back to request options, when no proxy found.
	//  - override: Enable proxy support for extensions, override request options.
	"http.proxySupport": "override",

	// Controls whether CA certificates should be loaded from the OS. On Windows and macOS, a reload of the window is required after turning this off. When during [remote development](https://aka.ms/vscode-remote) the `http.useLocalProxyConfiguration` setting is disabled this setting can be configured in the local and the remote settings separately.
	"http.systemCertificates": true,

	// Controls whether in the remote extension host the local proxy configuration should be used. This setting only applies as a remote setting during [remote development](https://aka.ms/vscode-remote).
	"http.useLocalProxyConfiguration": true,

	// Controls if the AltGraph+ modifier should be treated as Ctrl+Alt+.
	"keyboard.mapAltGrToCtrlAlt": false,

	// This setting is deprecated, please use 'update.mode' instead.
	// Configure whether you receive automatic updates. Requires a restart after change. The updates are fetched from a Microsoft online service.
	"update.channel": "default",

	// Enable to download and install new VS Code versions in the background on Windows.
	"update.enableWindowsBackgroundUpdates": true,

	// Configure whether you receive automatic updates. Requires a restart after change. The updates are fetched from a Microsoft online service.
	//  - none: Disable updates.
	//  - manual: Disable automatic background update checks. Updates will be available if you manually check for updates.
	//  - start: Check for updates only on startup. Disable automatic background update checks.
	//  - default: Enable automatic update checks. Code will check for updates automatically and periodically.
	"update.mode": "default",

	// Show Release Notes after an update. The Release Notes are fetched from a Microsoft online service.
	"update.showReleaseNotes": true,

	// Controls whether the comment thread should collapse when the thread is resolved.
	"comments.collapseOnResolve": true,

	// Controls whether the comments widget scrolls or expands.
	"comments.maxHeight": true,

	// This setting is deprecated in favor of `comments.openView`.
	// Controls when the comments panel should open.
	"comments.openPanel": "openOnSessionStartWithComments",

	// Controls when the comments view should open.
	//  - never: The comments view will never be opened.
	//  - file: The comments view will open when a file with comments is active.
	//  - firstFile: If the comments view has not been opened yet during this session it will open the first time during a session that a file with comments is active.
	//  - firstFileUnresolved: If the comments view has not been opened yet during this session and the comment is not resolved, it will open the first time during a session that a file with comments is active.
	"comments.openView": "firstFile",

	// Controls whether a confirmation dialog is shown when collapsing a comment thread.
	//  - whenHasUnsubmittedComments: Show a confirmation dialog when collapsing a comment thread with unsubmitted comments.
	//  - never: Never show a confirmation dialog when collapsing a comment thread.
	"comments.thread.confirmOnCollapse": "whenHasUnsubmittedComments",

	// Determines if relative time will be used in comment timestamps (ex. '1 day ago').
	"comments.useRelativeTime": true,

	// Controls the visibility of the comments bar and comment threads in editors that have commenting ranges and comments. Comments are still accessible via the Comments view and will cause commenting to be toggled on in the same way running the command "Comments: Toggle Editor Commenting" toggles comments.
	"comments.visible": true,

	// Allow setting breakpoints in any file.
	"debug.allowBreakpointsEverywhere": false,

	// Controls whether variables that are lazily resolved, such as getters, are automatically resolved and expanded by the debugger.
	//  - auto: When in screen reader optimized mode, automatically expand lazy variables.
	//  - on: Always automatically expand lazy variables.
	//  - off: Never automatically expand lazy variables.
	"debug.autoExpandLazyVariables": "auto",

	// At the end of a debug session, all the read-only tabs associated with that session will be closed
	"debug.closeReadonlyTabsOnEnd": false,

	// Controls whether to confirm when the window closes if there are active debug sessions.
	//  - never: Never confirm.
	//  - always: Always confirm if there are debug sessions.
	"debug.confirmOnExit": "never",

	// Controls whether suggestions should be accepted on Enter in the Debug Console. Enter is also used to evaluate whatever is typed in the Debug Console.
	"debug.console.acceptSuggestionOnEnter": "off",

	// Controls if the Debug Console should be automatically closed when the debug session ends.
	"debug.console.closeOnEnd": false,

	// Controls if the Debug Console should collapse identical lines and show a number of occurrences with a badge.
	"debug.console.collapseIdenticalLines": true,

	// Controls the font family in the Debug Console.
	"debug.console.fontFamily": "default",

	// Controls the font size in pixels in the Debug Console.
	"debug.console.fontSize": 14,

	// Controls if the Debug Console should suggest previously typed input.
	"debug.console.historySuggestions": true,

	// Controls the line height in pixels in the Debug Console. Use 0 to compute the line height from the font size.
	"debug.console.lineHeight": 0,

	// Controls if the lines should wrap in the Debug Console.
	"debug.console.wordWrap": true,

	// Show Source Code in Disassembly View.
	"debug.disassemblyView.showSourceCode": true,

	// Color of the Status bar when debugger is active.
	"debug.enableStatusBarColor": true,

	// Controls whether the editor should be focused when the debugger breaks.
	"debug.focusEditorOnBreak": true,

	// Controls whether the workbench window should be focused when the debugger breaks.
	"debug.focusWindowOnBreak": true,

	// Controls the action to perform when clicking the editor gutter with the middle mouse button.
	//  - logpoint: Add Logpoint.
	//  - conditionalBreakpoint: Add Conditional Breakpoint.
	//  - triggeredBreakpoint: Add Triggered Breakpoint.
	//  - none: Don't perform any action.
	"debug.gutterMiddleClickAction": "logpoint",

	// Hide 'Start Debugging' control in title bar of 'Run and Debug' view while debugging is active. Only relevant when `debug.toolBarLocation` is not `docked`.
	"debug.hideLauncherWhileDebugging": false,

	// Hide the warning shown when a `preLaunchTask` has been running for a while.
	"debug.hideSlowPreLaunchWarning": false,

	// Show variable values inline in editor while debugging.
	//  - on: Always show variable values inline in editor while debugging.
	//  - off: Never show variable values inline in editor while debugging.
	//  - auto: Show variable values inline in editor while debugging when the language supports inline value locations.
	"debug.inlineValues": "auto",

	// Controls when the internal Debug Console should open.
	"debug.internalConsoleOptions": "openOnFirstSessionStart",

	// Controls what to do when errors are encountered after running a preLaunchTask.
	//  - debugAnyway: Ignore task errors and start debugging.
	//  - showErrors: Show the Problems view and do not start debugging.
	//  - prompt: Prompt user.
	//  - abort: Cancel debugging.
	"debug.onTaskErrors": "prompt",

	// Controls when the debug view should open.
	"debug.openDebug": "openOnDebugBreak",

	// Automatically open the explorer view at the end of a debug session.
	"debug.openExplorerOnEnd": false,

	// Controls what editors to save before starting a debug session.
	//  - allEditorsInActiveGroup: Save all editors in the active group before starting a debug session.
	//  - nonUntitledEditorsInActiveGroup: Save all editors in the active group except untitled ones before starting a debug session.
	//  - none: Don't save any editors before starting a debug session.
	"debug.saveBeforeStart": "allEditorsInActiveGroup",

	// Controls whether breakpoints should be shown in the overview ruler.
	"debug.showBreakpointsInOverviewRuler": false,

	// Controls whether inline breakpoints candidate decorations should be shown in the editor while debugging.
	"debug.showInlineBreakpointCandidates": true,

	// Controls when the debug Status bar should be visible.
	//  - never: Never show debug in Status bar
	//  - always: Always show debug in Status bar
	//  - onFirstSessionStart: Show debug in Status bar only after debug was started for the first time
	"debug.showInStatusBar": "onFirstSessionStart",

	// Controls whether the debug sub-sessions are shown in the debug tool bar. When this setting is false the stop command on a sub-session will also stop the parent session.
	"debug.showSubSessionsInToolBar": false,

	// Show variable type in variable pane during debug session
	"debug.showVariableTypes": false,

	// Before starting a new debug session in an integrated or external terminal, clear the terminal.
	"debug.terminal.clearBeforeReusing": false,

	// Controls the location of the debug toolbar. Either `floating` in all views, `docked` in the debug view, `commandCenter` (requires `window.commandCenter`), or `hidden`.
	//  - floating: Show debug toolbar in all views.
	//  - docked: Show debug toolbar only in debug views.
	//  - commandCenter: `(Experimental)` Show debug toolbar in the command center.
	//  - hidden: Do not show debug toolbar.
	"debug.toolBarLocation": "floating",

	// Global debug launch configuration. Should be used as an alternative to 'launch.json' that is shared across workspaces.
	"launch": {
		"configurations": [],
		"compounds": []
	},

	// Enable/disable autoclosing of HTML tags.
	"html.autoClosingTags": true,

	// Enable/disable auto creation of quotes for HTML attribute assignment. The type of quotes can be configured by `html.completion.attributeDefaultValue`.
	"html.autoCreateQuotes": true,

	// Controls the default value for attributes when completion is accepted.
	//  - doublequotes: Attribute value is set to "".
	//  - singlequotes: Attribute value is set to ''.
	//  - empty: Attribute value is not set.
	"html.completion.attributeDefaultValue": "doublequotes",

	// A list of relative file paths pointing to JSON files following the [custom data format](https://github.com/microsoft/vscode-html-languageservice/blob/master/docs/customData.md).
	// 
	// VS Code loads custom data on startup to enhance its HTML support for the custom HTML tags, attributes and attribute values you specify in the JSON files.
	// 
	// The file paths are relative to workspace and only workspace folder settings are considered.
	"html.customData": [],

	// List of tags, comma separated, where the content shouldn't be reformatted. `null` defaults to the `pre` tag.
	"html.format.contentUnformatted": "pre,code,textarea",

	// Enable/disable default HTML formatter.
	"html.format.enable": true,

	// List of tags, comma separated, that should have an extra newline before them. `null` defaults to `"head, body, /html"`.
	"html.format.extraLiners": "head, body, /html",

	// Format and indent `{{#foo}}` and `{{/foo}}`.
	"html.format.indentHandlebars": false,

	// Indent `<head>` and `<body>` sections.
	"html.format.indentInnerHtml": false,

	// Maximum number of line breaks to be preserved in one chunk. Use `null` for unlimited.
	"html.format.maxPreserveNewLines": null,

	// Controls whether existing line breaks before elements should be preserved. Only works before elements, not inside tags or for text.
	"html.format.preserveNewLines": true,

	// Honor django, erb, handlebars and php templating language tags.
	"html.format.templating": false,

	// List of tags, comma separated, that shouldn't be reformatted. `null` defaults to all tags listed at https://www.w3.org/TR/html5/dom.html#phrasing-content.
	"html.format.unformatted": "wbr",

	// Keep text content together between this string.
	"html.format.unformattedContentDelimiter": "",

	// Wrap attributes.
	//  - auto: Wrap attributes only when line length is exceeded.
	//  - force: Wrap each attribute except first.
	//  - force-aligned: Wrap each attribute except first and keep aligned.
	//  - force-expand-multiline: Wrap each attribute.
	//  - aligned-multiple: Wrap when line length is exceeded, align attributes vertically.
	//  - preserve: Preserve wrapping of attributes.
	//  - preserve-aligned: Preserve wrapping of attributes but align.
	"html.format.wrapAttributes": "auto",

	// Indent wrapped attributes to after N characters. Use `null` to use the default indent size. Ignored if `html.format.wrapAttributes` is set to `aligned`.
	"html.format.wrapAttributesIndentSize": null,

	// Maximum amount of characters per line (0 = disable).
	"html.format.wrapLineLength": 120,

	// Show tag and attribute documentation in hover.
	"html.hover.documentation": true,

	// Show references to MDN in hover.
	"html.hover.references": true,

	// Deprecated in favor of `editor.linkedEditing`
	// Enable/disable mirroring cursor on matching HTML tag.
	"html.mirrorCursorOnMatchingTag": false,

	// Controls whether the built-in HTML language support suggests HTML5 tags, properties and values.
	"html.suggest.html5": true,

	// Traces the communication between VS Code and the HTML language server.
	"html.trace.server": "off",

	// Controls whether the built-in HTML language support validates embedded scripts.
	"html.validate.scripts": true,

	// Controls whether the built-in HTML language support validates embedded styles.
	"html.validate.styles": true,

	// The setting `json.colorDecorators.enable` has been deprecated in favor of `editor.colorDecorators`.
	// Enables or disables color decorators
	"json.colorDecorators.enable": true,

	// Enable/disable default JSON formatter
	"json.format.enable": true,

	// Keep all existing new lines when formatting.
	"json.format.keepLines": false,

	// The maximum number of outline symbols and folding regions computed (limited for performance reasons).
	"json.maxItemsComputed": 5000,

	// When enabled, JSON schemas can be fetched from http and https locations.
	"json.schemaDownload.enable": true,

	// Associate schemas to JSON files in the current project.
	"json.schemas": [],

	// Traces the communication between VS Code and the JSON language server.
	"json.trace.server": "off",

	// Enable/disable JSON validation.
	"json.validate.enable": true,

	// Configures the path and file name of files created by copy/paste or drag and drop. This is a map of globs that match against a Markdown document path to the destination path where the new file should be created.
	// 
	// The destination path may use the following variables:
	// 
	// - `${documentDirName}` — Absolute parent directory path of the Markdown document, e.g. `/Users/me/myProject/docs`.
	// - `${documentRelativeDirName}` — Relative parent directory path of the Markdown document, e.g. `docs`. This is the same as `${documentDirName}` if the file is not part of a workspace.
	// - `${documentFileName}` — The full filename of the Markdown document, e.g. `README.md`.
	// - `${documentBaseName}` — The basename of the Markdown document, e.g. `README`.
	// - `${documentExtName}` — The extension of the Markdown document, e.g. `md`.
	// - `${documentFilePath}` — Absolute path of the Markdown document, e.g. `/Users/me/myProject/docs/README.md`.
	// - `${documentRelativeFilePath}` — Relative path of the Markdown document, e.g. `docs/README.md`. This is the same as `${documentFilePath}` if the file is not part of a workspace.
	// - `${documentWorkspaceFolder}` — The workspace folder for the Markdown document, e.g. `/Users/me/myProject`. This is the same as `${documentDirName}` if the file is not part of a workspace.
	// - `${fileName}` — The file name of the dropped file, e.g. `image.png`.
	// - `${fileExtName}` — The extension of the dropped file, e.g. `png`.
	// - `${unixTime}` — The current Unix timestamp in milliseconds.
	"markdown.copyFiles.destination": {},

	// Controls if files created by drop or paste should overwrite existing files.
	//  - nameIncrementally: If a file with the same name already exists, append a number to the file name, for example: `image.png` becomes `image-1.png`.
	//  - overwrite: If a file with the same name already exists, overwrite it.
	"markdown.copyFiles.overwriteBehavior": "nameIncrementally",

	// Controls if files outside of the workspace that are dropped into a Markdown editor should be copied into the workspace.
	// 
	// Use `markdown.copyFiles.destination` to configure where copied dropped files should be created
	//  - mediaFiles: Try to copy external image and video files into the workspace.
	//  - never: Do not copy external files into the workspace.
	"markdown.editor.drop.copyIntoWorkspace": "mediaFiles",

	// Enable dropping files into a Markdown editor while holding Shift. Requires enabling `editor.dropIntoEditor.enabled`.
	//  - always: Always insert Markdown links.
	//  - smart: Smartly create Markdown links by default when not dropping into a code block or other special element. Use the drop widget to switch between pasting as plain text or as Markdown links.
	//  - never: Never create Markdown links.
	"markdown.editor.drop.enabled": "smart",

	// Snippet used when adding audio to Markdown. This snippet can use the following variables:
	// - `${src}` — The resolved path of the audio  file.
	// - `${title}` — The title used for the audio. A snippet placeholder will automatically be created for this variable.
	"markdown.editor.filePaste.audioSnippet": "<audio controls src=\"${src}\" title=\"${title}\"></audio>",

	// Controls if files outside of the workspace that are pasted into a Markdown editor should be copied into the workspace.
	// 
	// Use `markdown.copyFiles.destination` to configure where copied files should be created.
	//  - mediaFiles: Try to copy external image and video files into the workspace.
	//  - never: Do not copy external files into the workspace.
	"markdown.editor.filePaste.copyIntoWorkspace": "mediaFiles",

	// Enable pasting files into a Markdown editor to create Markdown links. Requires enabling `editor.pasteAs.enabled`.
	//  - always: Always insert Markdown links.
	//  - smart: Smartly create Markdown links by default when not pasting into a code block or other special element. Use the paste widget to switch between pasting as plain text or as Markdown links.
	//  - never: Never create Markdown links.
	"markdown.editor.filePaste.enabled": "smart",

	// Snippet used when adding videos to Markdown. This snippet can use the following variables:
	// - `${src}` — The resolved path of the video file.
	// - `${title}` — The title used for the video. A snippet placeholder will automatically be created for this variable.
	"markdown.editor.filePaste.videoSnippet": "<video controls src=\"${src}\" title=\"${title}\"></video>",

	// Controls if Markdown links are created when URLs are pasted into a Markdown editor. Requires enabling `editor.pasteAs.enabled`.
	//  - always: Always insert Markdown links.
	//  - smart: Smartly create Markdown links by default when not pasting into a code block or other special element. Use the paste widget to switch between pasting as plain text or as Markdown links.
	//  - smartWithSelection: Smartly create Markdown links by default when you have selected text and are not pasting into a code block or other special element. Use the paste widget to switch between pasting as plain text or as Markdown links.
	//  - never: Never create Markdown links.
	"markdown.editor.pasteUrlAsFormattedLink.enabled": "smartWithSelection",

	// Enable/disable a paste option that updates links and reference in text that is copied and pasted between Markdown editors.
	// 
	// To use this feature, after pasting text that contains updatable links, just click on the Paste Widget and select `Paste and update pasted links`.
	"markdown.editor.updateLinksOnPaste.enabled": true,

	// Controls where links in Markdown files should be opened.
	//  - currentGroup: Open links in the active editor group.
	//  - beside: Open links beside the active editor.
	"markdown.links.openLocation": "currentGroup",

	// Enable highlighting link occurrences in the current document.
	"markdown.occurrencesHighlight.enabled": false,

	// Controls if file extensions (for example `.md`) are added or not for links to Markdown files. This setting is used when file paths are added by tooling such as path completions or file renames.
	//  - auto: For existing paths, try to maintain the file extension style. For new paths, add file extensions.
	//  - includeExtension: Prefer including the file extension. For example, path completions to a file named `file.md` will insert `file.md`.
	//  - removeExtension: Prefer removing the file extension. For example, path completions to a file named `file.md` will insert `file` without the `.md`.
	"markdown.preferredMdPathExtensionStyle": "auto",

	// Sets how line-breaks are rendered in the Markdown preview. Setting it to `true` creates a `<br>` for newlines inside paragraphs.
	"markdown.preview.breaks": false,

	// Double-click in the Markdown preview to switch to the editor.
	"markdown.preview.doubleClickToSwitchToEditor": true,

	// Controls the font family used in the Markdown preview.
	"markdown.preview.fontFamily": "-apple-system, BlinkMacSystemFont, 'Segoe WPC', 'Segoe UI', system-ui, 'Ubuntu', 'Droid Sans', sans-serif",

	// Controls the font size in pixels used in the Markdown preview.
	"markdown.preview.fontSize": 14,

	// Controls the line height used in the Markdown preview. This number is relative to the font size.
	"markdown.preview.lineHeight": 1.6,

	// Convert URL-like text to links in the Markdown preview.
	"markdown.preview.linkify": true,

	// Mark the current editor selection in the Markdown preview.
	"markdown.preview.markEditorSelection": true,

	// Controls how links to other Markdown files in the Markdown preview should be opened.
	//  - inPreview: Try to open links in the Markdown preview.
	//  - inEditor: Try to open links in the editor.
	"markdown.preview.openMarkdownLinks": "inPreview",

	// When a Markdown preview is scrolled, update the view of the editor.
	"markdown.preview.scrollEditorWithPreview": true,

	// When a Markdown editor is scrolled, update the view of the preview.
	"markdown.preview.scrollPreviewWithEditor": true,

	// Enable some language-neutral replacement and quotes beautification in the Markdown preview.
	"markdown.preview.typographer": false,

	// Controls the logging level of the Markdown language server.
	"markdown.server.log": "off",

	// A list of URLs or local paths to CSS style sheets to use from the Markdown preview. Relative paths are interpreted relative to the folder open in the Explorer. If there is no open folder, they are interpreted relative to the location of the Markdown file. All '\' need to be written as '\\'.
	"markdown.styles": [],

	// Enable path suggestions while writing links in Markdown files.
	"markdown.suggest.paths.enabled": true,

	// Enable suggestions for headers in other Markdown files in the current workspace. Accepting one of these suggestions inserts the full path to header in that file, for example: `[link text](/path/to/file.md#header)`.
	//  - never: Disable workspace header suggestions.
	//  - onDoubleHash: Enable workspace header suggestions after typing `#` in a path, for example: `[link text](#`.
	//  - onSingleOrDoubleHash: Enable workspace header suggestions after typing either `#` or `#` in a path, for example: `[link text](#` or `[link text](#`.
	"markdown.suggest.paths.includeWorkspaceHeaderCompletions": "onDoubleHash",

	// Enable debug logging for the Markdown extension.
	"markdown.trace.extension": "off",

	// Traces the communication between VS Code and the Markdown language server.
	"markdown.trace.server": "off",

	// Try to update links in Markdown files when a file is renamed/moved in the workspace. Use `markdown.updateLinksOnFileMove.include` to configure which files trigger link updates.
	//  - prompt: Prompt on each file move.
	//  - always: Always update links automatically.
	//  - never: Never try to update link and don't prompt.
	"markdown.updateLinksOnFileMove.enabled": "never",

	// Enable updating links when a directory is moved or renamed in the workspace.
	"markdown.updateLinksOnFileMove.enableForDirectories": true,

	// Glob patterns that specifies files that trigger automatic link updates. See `markdown.updateLinksOnFileMove.enabled` for details about this feature.
	"markdown.updateLinksOnFileMove.include": [
		"**/*.{md,mkd,mdwn,mdown,markdown,markdn,mdtxt,mdtext,workbook}",
		"**/*.{jpg,jpe,jpeg,png,bmp,gif,ico,webp,avif,tiff,svg,mp4}"
	],

	// Validate duplicated definitions in the current file.
	"markdown.validate.duplicateLinkDefinitions.enabled": "warning",

	// Enable all error reporting in Markdown files.
	"markdown.validate.enabled": false,

	// Validate links to other files in Markdown files, for example `[link](/path/to/file.md)`. This checks that the target files exists. Requires enabling `markdown.validate.enabled`.
	"markdown.validate.fileLinks.enabled": "warning",

	// Validate the fragment part of links to headers in other files in Markdown files, for example: `[link](/path/to/file.md#header)`. Inherits the setting value from `markdown.validate.fragmentLinks.enabled` by default.
	"markdown.validate.fileLinks.markdownFragmentLinks": "inherit",

	// Validate fragment links to headers in the current Markdown file, for example: `[link](#header)`. Requires enabling `markdown.validate.enabled`.
	"markdown.validate.fragmentLinks.enabled": "warning",

	// Configure links that should not be validated. For example adding `/about` would not validate the link `[about](/about)`, while the glob `/assets/**/*.svg` would let you skip validation for any link to `.svg` files under the `assets` directory.
	"markdown.validate.ignoredLinks": [],

	// Validate reference links in Markdown files, for example: `[link][ref]`. Requires enabling `markdown.validate.enabled`.
	"markdown.validate.referenceLinks.enabled": "warning",

	// Validate link definitions that are unused in the current file.
	"markdown.validate.unusedLinkDefinitions.enabled": "hint",

	// Controls whether the built-in PHP language suggestions are enabled. The support suggests PHP globals and variables.
	"php.suggest.basic": true,

	// Enable/disable built-in PHP validation.
	"php.validate.enable": true,

	// Points to the PHP executable.
	"php.validate.executablePath": null,

	// Whether the linter is run on save or on type.
	"php.validate.run": "onSave",

	// Enable/disable automatic closing of JSX tags.
	"javascript.autoClosingTags": true,

	// Enable/disable default JavaScript formatter.
	"javascript.format.enable": true,

	// Indent case clauses in switch statements. Requires using TypeScript 5.1+ in the workspace.
	"javascript.format.indentSwitchCase": true,

	// Defines space handling after a comma delimiter.
	"javascript.format.insertSpaceAfterCommaDelimiter": true,

	// Defines space handling after the constructor keyword.
	"javascript.format.insertSpaceAfterConstructor": false,

	// Defines space handling after function keyword for anonymous functions.
	"javascript.format.insertSpaceAfterFunctionKeywordForAnonymousFunctions": true,

	// Defines space handling after keywords in a control flow statement.
	"javascript.format.insertSpaceAfterKeywordsInControlFlowStatements": true,

	// Defines space handling after opening and before closing empty braces.
	"javascript.format.insertSpaceAfterOpeningAndBeforeClosingEmptyBraces": true,

	// Defines space handling after opening and before closing JSX expression braces.
	"javascript.format.insertSpaceAfterOpeningAndBeforeClosingJsxExpressionBraces": false,

	// Defines space handling after opening and before closing non-empty braces.
	"javascript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBraces": true,

	// Defines space handling after opening and before closing non-empty brackets.
	"javascript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBrackets": false,

	// Defines space handling after opening and before closing non-empty parenthesis.
	"javascript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyParenthesis": false,

	// Defines space handling after opening and before closing template string braces.
	"javascript.format.insertSpaceAfterOpeningAndBeforeClosingTemplateStringBraces": false,

	// Defines space handling after a semicolon in a for statement.
	"javascript.format.insertSpaceAfterSemicolonInForStatements": true,

	// Defines space handling after a binary operator.
	"javascript.format.insertSpaceBeforeAndAfterBinaryOperators": true,

	// Defines space handling before function argument parentheses.
	"javascript.format.insertSpaceBeforeFunctionParenthesis": false,

	// Defines whether an open brace is put onto a new line for control blocks or not.
	"javascript.format.placeOpenBraceOnNewLineForControlBlocks": false,

	// Defines whether an open brace is put onto a new line for functions or not.
	"javascript.format.placeOpenBraceOnNewLineForFunctions": false,

	// Defines handling of optional semicolons.
	//  - ignore: Don't insert or remove any semicolons.
	//  - insert: Insert semicolons at statement ends.
	//  - remove: Remove unnecessary semicolons.
	"javascript.format.semicolons": "ignore",

	// This setting has been deprecated in favor of `js/ts.implicitProjectConfig.checkJs`.
	// Enable/disable semantic checking of JavaScript files. Existing `jsconfig.json` or `tsconfig.json` files override this setting.
	"javascript.implicitProjectConfig.checkJs": false,

	// This setting has been deprecated in favor of `js/ts.implicitProjectConfig.experimentalDecorators`.
	// Enable/disable `experimentalDecorators` in JavaScript files that are not part of a project. Existing `jsconfig.json` or `tsconfig.json` files override this setting.
	"javascript.implicitProjectConfig.experimentalDecorators": false,

	// Enable/disable inlay hints for implicit return types on function signatures:
	// ```typescript
	// 
	// function foo() /* :number */ {
	// 	return Date.now();
	// } 
	//  
	// ```
	"javascript.inlayHints.functionLikeReturnTypes.enabled": false,

	// Enable/disable inlay hints for parameter names:
	// ```typescript
	// 
	// parseInt(/* str: */ '123', /* radix: */ 8)
	//  
	// ```
	//  - none: Disable parameter name hints.
	//  - literals: Enable parameter name hints only for literal arguments.
	//  - all: Enable parameter name hints for literal and non-literal arguments.
	"javascript.inlayHints.parameterNames.enabled": "none",

	// Suppress parameter name hints on arguments whose text is identical to the parameter name.
	"javascript.inlayHints.parameterNames.suppressWhenArgumentMatchesName": true,

	// Enable/disable inlay hints for implicit parameter types:
	// ```typescript
	// 
	// el.addEventListener('click', e /* :MouseEvent */ => ...)
	//  
	// ```
	"javascript.inlayHints.parameterTypes.enabled": false,

	// Enable/disable inlay hints for implicit types on property declarations:
	// ```typescript
	// 
	// class Foo {
	// 	prop /* :number */ = Date.now();
	// }
	//  
	// ```
	"javascript.inlayHints.propertyDeclarationTypes.enabled": false,

	// Enable/disable inlay hints for implicit variable types:
	// ```typescript
	// 
	// const foo /* :number */ = Date.now();
	//  
	// ```
	"javascript.inlayHints.variableTypes.enabled": false,

	// Suppress type hints on variables whose name is identical to the type name.
	"javascript.inlayHints.variableTypes.suppressWhenTypeMatchesName": true,

	// Specify glob patterns of files to exclude from auto imports. Relative paths are resolved relative to the workspace root. Patterns are evaluated using tsconfig.json [`exclude`](https://www.typescriptlang.org/tsconfig#exclude) semantics.
	"javascript.preferences.autoImportFileExcludePatterns": [],

	// Specify regular expressions to exclude auto imports with matching import specifiers. Examples:
	// 
	// - `^node:`
	// - `lib/internal` (slashes don't need to be escaped...)
	// - `/lib\/internal/i` (...unless including surrounding slashes for `i` or `u` flags)
	// - `^lodash$` (only allow subpath imports from lodash)
	"javascript.preferences.autoImportSpecifierExcludeRegexes": [],

	// Preferred path style for auto imports.
	//  - shortest: Prefers a non-relative import only if one is available that has fewer path segments than a relative import.
	//  - relative: Prefers a relative path to the imported file location.
	//  - non-relative: Prefers a non-relative import based on the `baseUrl` or `paths` configured in your `jsconfig.json` / `tsconfig.json`.
	//  - project-relative: Prefers a non-relative import only if the relative import path would leave the package or project directory.
	"javascript.preferences.importModuleSpecifier": "shortest",

	// Preferred path ending for auto imports.
	//  - auto: Use project settings to select a default.
	//  - minimal: Shorten `./component/index.js` to `./component`.
	//  - index: Shorten `./component/index.js` to `./component/index`.
	//  - js: Do not shorten path endings; include the `.js` or `.ts` extension.
	"javascript.preferences.importModuleSpecifierEnding": "auto",

	// Preferred style for JSX attribute completions.
	//  - auto: Insert `={}` or `=""` after attribute names based on the prop type. See `javascript.preferences.quoteStyle` to control the type of quotes used for string attributes.
	//  - braces: Insert `={}` after attribute names.
	//  - none: Only insert attribute names.
	"javascript.preferences.jsxAttributeCompletionStyle": "auto",

	// Advanced preferences that control how imports are ordered.
	"javascript.preferences.organizeImports": {},

	// Preferred quote style to use for Quick Fixes.
	//  - auto: Infer quote type from existing code
	//  - single: Always use single quotes: `'`
	//  - double: Always use double quotes: `"`
	"javascript.preferences.quoteStyle": "auto",

	// When on a JSX tag, try to rename the matching tag instead of renaming the symbol. Requires using TypeScript 5.1+ in the workspace.
	"javascript.preferences.renameMatchingJsxTags": true,

	// The setting 'typescript.preferences.renameShorthandProperties' has been deprecated in favor of 'typescript.preferences.useAliasesForRenames'
	// Enable/disable introducing aliases for object shorthand properties during renames.
	"javascript.preferences.renameShorthandProperties": true,

	// Enable/disable introducing aliases for object shorthand properties during renames.
	"javascript.preferences.useAliasesForRenames": true,

	// Makes `Go to Definition` avoid type declaration files when possible by triggering `Go to Source Definition` instead. This allows `Go to Source Definition` to be triggered with the mouse gesture.
	"javascript.preferGoToSourceDefinition": false,

	// Enable/disable references CodeLens in JavaScript files.
	"javascript.referencesCodeLens.enabled": false,

	// Enable/disable references CodeLens on all functions in JavaScript files.
	"javascript.referencesCodeLens.showOnAllFunctions": false,

	// Enable/disable auto import suggestions.
	"javascript.suggest.autoImports": true,

	// Enable/disable snippet completions for class members.
	"javascript.suggest.classMemberSnippets.enabled": true,

	// Complete functions with their parameter signature.
	"javascript.suggest.completeFunctionCalls": false,

	// Enable/disable suggestion to complete JSDoc comments.
	"javascript.suggest.completeJSDocs": true,

	// Enabled/disable autocomplete suggestions.
	"javascript.suggest.enabled": true,

	// Enable/disable showing completions on potentially undefined values that insert an optional chain call. Requires strict null checks to be enabled.
	"javascript.suggest.includeAutomaticOptionalChainCompletions": true,

	// Enable/disable auto-import-style completions on partially-typed import statements.
	"javascript.suggest.includeCompletionsForImportStatements": true,

	// Enable/disable generating `@returns` annotations for JSDoc templates.
	"javascript.suggest.jsdoc.generateReturns": true,

	// Enable/disable including unique names from the file in JavaScript suggestions. Note that name suggestions are always disabled in JavaScript code that is semantically checked using `@ts-check` or `checkJs`.
	"javascript.suggest.names": true,

	// Enable/disable suggestions for paths in import statements and require calls.
	"javascript.suggest.paths": true,

	// Enable/disable suggestion diagnostics for JavaScript files in the editor.
	"javascript.suggestionActions.enabled": true,

	// Enable/disable automatic updating of import paths when you rename or move a file in VS Code.
	//  - prompt: Prompt on each rename.
	//  - always: Always update paths automatically.
	//  - never: Never rename paths and don't prompt.
	"javascript.updateImportsOnFileMove.enabled": "prompt",

	// Enable updating imports when pasting code. Requires TypeScript 5.7+.
	// 
	// By default this shows a option to update imports after pasting. You can use the `editor.pasteAs.preferences` setting to update imports automatically when pasting: `"editor.pasteAs.preferences": [ "text.updateImports.jsts" ]`.
	"javascript.updateImportsOnPaste.enabled": true,

	// Enable/disable JavaScript validation.
	"javascript.validate.enable": true,

	// Enable/disable semantic checking of JavaScript files. Existing `jsconfig.json` or `tsconfig.json` files override this setting.
	"js/ts.implicitProjectConfig.checkJs": false,

	// Enable/disable `experimentalDecorators` in JavaScript files that are not part of a project. Existing `jsconfig.json` or `tsconfig.json` files override this setting.
	"js/ts.implicitProjectConfig.experimentalDecorators": false,

	// Sets the module system for the program. See more: https://www.typescriptlang.org/tsconfig#module.
	"js/ts.implicitProjectConfig.module": "ESNext",

	// Enable/disable [strict function types](https://www.typescriptlang.org/tsconfig#strictFunctionTypes) in JavaScript and TypeScript files that are not part of a project. Existing `jsconfig.json` or `tsconfig.json` files override this setting.
	"js/ts.implicitProjectConfig.strictFunctionTypes": true,

	// Enable/disable [strict null checks](https://www.typescriptlang.org/tsconfig#strictNullChecks) in JavaScript and TypeScript files that are not part of a project. Existing `jsconfig.json` or `tsconfig.json` files override this setting.
	"js/ts.implicitProjectConfig.strictNullChecks": true,

	// Set target JavaScript language version for emitted JavaScript and include library declarations. See more: https://www.typescriptlang.org/tsconfig#target.
	"js/ts.implicitProjectConfig.target": "ES2022",

	// Enable/disable automatic closing of JSX tags.
	"typescript.autoClosingTags": true,

	// Check if npm is installed for [Automatic Type Acquisition](https://code.visualstudio.com/docs/nodejs/working-with-javascript#_typings-and-automatic-type-acquisition).
	"typescript.check.npmIsInstalled": true,

	// Disables [automatic type acquisition](https://code.visualstudio.com/docs/nodejs/working-with-javascript#_typings-and-automatic-type-acquisition). Automatic type acquisition fetches `@types` packages from npm to improve IntelliSense for external libraries.
	"typescript.disableAutomaticTypeAcquisition": false,

	// Enables prompting of users to use the TypeScript version configured in the workspace for Intellisense.
	"typescript.enablePromptUseWorkspaceTsdk": false,

	// Enable expanding/contracting the hover to reveal more/less information from the TS server.
	"typescript.experimental.expandableHover": false,

	// Enable/disable default TypeScript formatter.
	"typescript.format.enable": true,

	// Indent case clauses in switch statements. Requires using TypeScript 5.1+ in the workspace.
	"typescript.format.indentSwitchCase": true,

	// Defines space handling after a comma delimiter.
	"typescript.format.insertSpaceAfterCommaDelimiter": true,

	// Defines space handling after the constructor keyword.
	"typescript.format.insertSpaceAfterConstructor": false,

	// Defines space handling after function keyword for anonymous functions.
	"typescript.format.insertSpaceAfterFunctionKeywordForAnonymousFunctions": true,

	// Defines space handling after keywords in a control flow statement.
	"typescript.format.insertSpaceAfterKeywordsInControlFlowStatements": true,

	// Defines space handling after opening and before closing empty braces.
	"typescript.format.insertSpaceAfterOpeningAndBeforeClosingEmptyBraces": true,

	// Defines space handling after opening and before closing JSX expression braces.
	"typescript.format.insertSpaceAfterOpeningAndBeforeClosingJsxExpressionBraces": false,

	// Defines space handling after opening and before closing non-empty braces.
	"typescript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBraces": true,

	// Defines space handling after opening and before closing non-empty brackets.
	"typescript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyBrackets": false,

	// Defines space handling after opening and before closing non-empty parenthesis.
	"typescript.format.insertSpaceAfterOpeningAndBeforeClosingNonemptyParenthesis": false,

	// Defines space handling after opening and before closing template string braces.
	"typescript.format.insertSpaceAfterOpeningAndBeforeClosingTemplateStringBraces": false,

	// Defines space handling after a semicolon in a for statement.
	"typescript.format.insertSpaceAfterSemicolonInForStatements": true,

	// Defines space handling after type assertions in TypeScript.
	"typescript.format.insertSpaceAfterTypeAssertion": false,

	// Defines space handling after a binary operator.
	"typescript.format.insertSpaceBeforeAndAfterBinaryOperators": true,

	// Defines space handling before function argument parentheses.
	"typescript.format.insertSpaceBeforeFunctionParenthesis": false,

	// Defines whether an open brace is put onto a new line for control blocks or not.
	"typescript.format.placeOpenBraceOnNewLineForControlBlocks": false,

	// Defines whether an open brace is put onto a new line for functions or not.
	"typescript.format.placeOpenBraceOnNewLineForFunctions": false,

	// Defines handling of optional semicolons.
	//  - ignore: Don't insert or remove any semicolons.
	//  - insert: Insert semicolons at statement ends.
	//  - remove: Remove unnecessary semicolons.
	"typescript.format.semicolons": "ignore",

	// Enable/disable implementations CodeLens. This CodeLens shows the implementers of an interface.
	"typescript.implementationsCodeLens.enabled": false,

	// Enable/disable implementations CodeLens on interface methods.
	"typescript.implementationsCodeLens.showOnInterfaceMethods": false,

	// Enable/disable inlay hints for member values in enum declarations:
	// ```typescript
	// 
	// enum MyValue {
	// 	A /* = 0 */;
	// 	B /* = 1 */;
	// }
	//  
	// ```
	"typescript.inlayHints.enumMemberValues.enabled": false,

	// Enable/disable inlay hints for implicit return types on function signatures:
	// ```typescript
	// 
	// function foo() /* :number */ {
	// 	return Date.now();
	// } 
	//  
	// ```
	"typescript.inlayHints.functionLikeReturnTypes.enabled": false,

	// Enable/disable inlay hints for parameter names:
	// ```typescript
	// 
	// parseInt(/* str: */ '123', /* radix: */ 8)
	//  
	// ```
	//  - none: Disable parameter name hints.
	//  - literals: Enable parameter name hints only for literal arguments.
	//  - all: Enable parameter name hints for literal and non-literal arguments.
	"typescript.inlayHints.parameterNames.enabled": "none",

	// Suppress parameter name hints on arguments whose text is identical to the parameter name.
	"typescript.inlayHints.parameterNames.suppressWhenArgumentMatchesName": true,

	// Enable/disable inlay hints for implicit parameter types:
	// ```typescript
	// 
	// el.addEventListener('click', e /* :MouseEvent */ => ...)
	//  
	// ```
	"typescript.inlayHints.parameterTypes.enabled": false,

	// Enable/disable inlay hints for implicit types on property declarations:
	// ```typescript
	// 
	// class Foo {
	// 	prop /* :number */ = Date.now();
	// }
	//  
	// ```
	"typescript.inlayHints.propertyDeclarationTypes.enabled": false,

	// Enable/disable inlay hints for implicit variable types:
	// ```typescript
	// 
	// const foo /* :number */ = Date.now();
	//  
	// ```
	"typescript.inlayHints.variableTypes.enabled": false,

	// Suppress type hints on variables whose name is identical to the type name.
	"typescript.inlayHints.variableTypes.suppressWhenTypeMatchesName": true,

	// Sets the locale used to report JavaScript and TypeScript errors. Defaults to use VS Code's locale.
	//  - auto: Use VS Code's configured display language.
	//  - de: Deutsch
	//  - es: español
	//  - en: English
	//  - fr: français
	//  - it: italiano
	//  - ja: 日本語
	//  - ko: 한국어
	//  - ru: русский
	//  - zh-CN: 中文(简体)
	//  - zh-TW: 中文(繁體)
	"typescript.locale": "auto",

	// Specifies the path to the npm executable used for [Automatic Type Acquisition](https://code.visualstudio.com/docs/nodejs/working-with-javascript#_typings-and-automatic-type-acquisition).
	"typescript.npm": "",

	// Specify glob patterns of files to exclude from auto imports. Relative paths are resolved relative to the workspace root. Patterns are evaluated using tsconfig.json [`exclude`](https://www.typescriptlang.org/tsconfig#exclude) semantics.
	"typescript.preferences.autoImportFileExcludePatterns": [],

	// Specify regular expressions to exclude auto imports with matching import specifiers. Examples:
	// 
	// - `^node:`
	// - `lib/internal` (slashes don't need to be escaped...)
	// - `/lib\/internal/i` (...unless including surrounding slashes for `i` or `u` flags)
	// - `^lodash$` (only allow subpath imports from lodash)
	"typescript.preferences.autoImportSpecifierExcludeRegexes": [],

	// Preferred path style for auto imports.
	//  - shortest: Prefers a non-relative import only if one is available that has fewer path segments than a relative import.
	//  - relative: Prefers a relative path to the imported file location.
	//  - non-relative: Prefers a non-relative import based on the `baseUrl` or `paths` configured in your `jsconfig.json` / `tsconfig.json`.
	//  - project-relative: Prefers a non-relative import only if the relative import path would leave the package or project directory.
	"typescript.preferences.importModuleSpecifier": "shortest",

	// Preferred path ending for auto imports.
	//  - auto: Use project settings to select a default.
	//  - minimal: Shorten `./component/index.js` to `./component`.
	//  - index: Shorten `./component/index.js` to `./component/index`.
	//  - js: Do not shorten path endings; include the `.js` or `.ts` extension.
	"typescript.preferences.importModuleSpecifierEnding": "auto",

	// Enable/disable searching `package.json` dependencies for available auto imports.
	//  - auto: Search dependencies based on estimated performance impact.
	//  - on: Always search dependencies.
	//  - off: Never search dependencies.
	"typescript.preferences.includePackageJsonAutoImports": "auto",

	// Preferred style for JSX attribute completions.
	//  - auto: Insert `={}` or `=""` after attribute names based on the prop type. See `typescript.preferences.quoteStyle` to control the type of quotes used for string attributes.
	//  - braces: Insert `={}` after attribute names.
	//  - none: Only insert attribute names.
	"typescript.preferences.jsxAttributeCompletionStyle": "auto",

	// Advanced preferences that control how imports are ordered.
	"typescript.preferences.organizeImports": {},

	// Include the `type` keyword in auto-imports whenever possible. Requires using TypeScript 5.3+ in the workspace.
	"typescript.preferences.preferTypeOnlyAutoImports": false,

	// Preferred quote style to use for Quick Fixes.
	//  - auto: Infer quote type from existing code
	//  - single: Always use single quotes: `'`
	//  - double: Always use double quotes: `"`
	"typescript.preferences.quoteStyle": "auto",

	// When on a JSX tag, try to rename the matching tag instead of renaming the symbol. Requires using TypeScript 5.1+ in the workspace.
	"typescript.preferences.renameMatchingJsxTags": true,

	// The setting 'typescript.preferences.renameShorthandProperties' has been deprecated in favor of 'typescript.preferences.useAliasesForRenames'
	// Enable/disable introducing aliases for object shorthand properties during renames.
	"typescript.preferences.renameShorthandProperties": true,

	// Enable/disable introducing aliases for object shorthand properties during renames.
	"typescript.preferences.useAliasesForRenames": true,

	// Makes `Go to Definition` avoid type declaration files when possible by triggering `Go to Source Definition` instead. This allows `Go to Source Definition` to be triggered with the mouse gesture.
	"typescript.preferGoToSourceDefinition": false,

	// Enable/disable references CodeLens in TypeScript files.
	"typescript.referencesCodeLens.enabled": false,

	// Enable/disable references CodeLens on all functions in TypeScript files.
	"typescript.referencesCodeLens.showOnAllFunctions": false,

	// Report style checks as warnings.
	"typescript.reportStyleChecksAsWarnings": true,

	// Enable/disable auto import suggestions.
	"typescript.suggest.autoImports": true,

	// Enable/disable snippet completions for class members.
	"typescript.suggest.classMemberSnippets.enabled": true,

	// Complete functions with their parameter signature.
	"typescript.suggest.completeFunctionCalls": false,

	// Enable/disable suggestion to complete JSDoc comments.
	"typescript.suggest.completeJSDocs": true,

	// Enabled/disable autocomplete suggestions.
	"typescript.suggest.enabled": true,

	// Enable/disable showing completions on potentially undefined values that insert an optional chain call. Requires strict null checks to be enabled.
	"typescript.suggest.includeAutomaticOptionalChainCompletions": true,

	// Enable/disable auto-import-style completions on partially-typed import statements.
	"typescript.suggest.includeCompletionsForImportStatements": true,

	// Enable/disable generating `@returns` annotations for JSDoc templates.
	"typescript.suggest.jsdoc.generateReturns": true,

	// Enable/disable snippet completions for methods in object literals.
	"typescript.suggest.objectLiteralMethodSnippets.enabled": true,

	// Enable/disable suggestions for paths in import statements and require calls.
	"typescript.suggest.paths": true,

	// Enable/disable suggestion diagnostics for TypeScript files in the editor.
	"typescript.suggestionActions.enabled": true,

	// Enabled/disable occasional surveys that help us improve VS Code's JavaScript and TypeScript support.
	"typescript.surveys.enabled": true,

	// Controls auto detection of tsc tasks.
	//  - on: Create both build and watch tasks.
	//  - off: Disable this feature.
	//  - build: Only create single run compile tasks.
	//  - watch: Only create compile and watch tasks.
	"typescript.tsc.autoDetect": "on",

	// Specifies the folder path to the tsserver and `lib*.d.ts` files under a TypeScript install to use for IntelliSense, for example: `./node_modules/typescript/lib`.
	// 
	// - When specified as a user setting, the TypeScript version from `typescript.tsdk` automatically replaces the built-in TypeScript version.
	// - When specified as a workspace setting, `typescript.tsdk` allows you to switch to use that workspace version of TypeScript for IntelliSense with the `TypeScript: Select TypeScript version` command.
	// 
	// See the [TypeScript documentation](https://code.visualstudio.com/docs/typescript/typescript-compiling#_using-newer-typescript-versions) for more detail about managing TypeScript versions.
	"typescript.tsdk": "",

	// Enables region-based diagnostics in TypeScript. Requires using TypeScript 5.6+ in the workspace.
	"typescript.tsserver.enableRegionDiagnostics": true,

	// Enables tracing TS server performance to a directory. These trace files can be used to diagnose TS Server performance issues. The log may contain file paths, source code, and other potentially sensitive information from your project.
	"typescript.tsserver.enableTracing": false,

	// Enables project wide error reporting.
	"typescript.tsserver.experimental.enableProjectDiagnostics": false,

	// Please use the `typescript.tsserver.watchOptions` setting instead.
	// Use VS Code's file watchers instead of TypeScript's. Requires using TypeScript 5.4+ in the workspace.
	"typescript.tsserver.experimental.useVsCodeWatcher": true,

	// Enables logging of the TS server to a file. This log can be used to diagnose TS Server issues. The log may contain file paths, source code, and other potentially sensitive information from your project.
	"typescript.tsserver.log": "off",

	// The maximum amount of memory (in MB) to allocate to the TypeScript server process. To use a memory limit greater than 4 GB, use `typescript.tsserver.nodePath` to run TS Server with a custom Node installation.
	"typescript.tsserver.maxTsServerMemory": 3072,

	// Run TS Server on a custom Node installation. This can be a path to a Node executable, or 'node' if you want VS Code to detect a Node installation.
	"typescript.tsserver.nodePath": "",

	// Additional paths to discover TypeScript Language Service plugins.
	"typescript.tsserver.pluginPaths": [],

	// This setting has been deprecated in favor of `typescript.tsserver.useSyntaxServer`.
	// Enable/disable spawning a separate TypeScript server that can more quickly respond to syntax related operations, such as calculating folding or computing document symbols.
	"typescript.tsserver.useSeparateSyntaxServer": true,

	// Controls if TypeScript launches a dedicated server to more quickly handle syntax related operations, such as computing code folding.
	//  - always: Use a lighter weight syntax server to handle all IntelliSense operations. This syntax server can only provide IntelliSense for opened files.
	//  - never: Don't use a dedicated syntax server. Use a single server to handle all IntelliSense operations.
	//  - auto: Spawn both a full server and a lighter weight server dedicated to syntax operations. The syntax server is used to speed up syntax operations and provide IntelliSense while projects are loading.
	"typescript.tsserver.useSyntaxServer": "auto",

	// Configure which watching strategies should be used to keep track of files and directories.
	"typescript.tsserver.watchOptions": "vscode",

	// Enable/disable project-wide IntelliSense on web. Requires that VS Code is running in a trusted context.
	"typescript.tsserver.web.projectWideIntellisense.enabled": true,

	// Suppresses semantic errors on web even when project wide IntelliSense is enabled. This is always on when project wide IntelliSense is not enabled or available. See `typescript.tsserver.web.projectWideIntellisense.enabled`
	"typescript.tsserver.web.projectWideIntellisense.suppressSemanticErrors": false,

	// Enable/disable package acquisition on the web. This enables IntelliSense for imported packages. Requires `typescript.tsserver.web.projectWideIntellisense.enabled`. Currently not supported for Safari.
	"typescript.tsserver.web.typeAcquisition.enabled": true,

	// Enable/disable automatic updating of import paths when you rename or move a file in VS Code.
	//  - prompt: Prompt on each rename.
	//  - always: Always update paths automatically.
	//  - never: Never rename paths and don't prompt.
	"typescript.updateImportsOnFileMove.enabled": "prompt",

	// Enable updating imports when pasting code. Requires TypeScript 5.7+.
	// 
	// By default this shows a option to update imports after pasting. You can use the `editor.pasteAs.preferences` setting to update imports automatically when pasting: `"editor.pasteAs.preferences": [ "text.updateImports.jsts" ]`.
	"typescript.updateImportsOnPaste.enabled": true,

	// Enable/disable TypeScript validation.
	"typescript.validate.enable": true,

	// Exclude symbols that come from library files in `Go to Symbol in Workspace` results. Requires using TypeScript 5.3+ in the workspace.
	"typescript.workspaceSymbols.excludeLibrarySymbols": true,

	// Controls which files are searched by [Go to Symbol in Workspace](https://code.visualstudio.com/docs/editor/editingevolved#_open-symbol-by-name).
	//  - allOpenProjects: Search all open JavaScript or TypeScript projects for symbols.
	//  - currentProject: Only search for symbols in the current JavaScript or TypeScript project.
	"typescript.workspaceSymbols.scope": "allOpenProjects",

	// Always reveal the executed test when `testing.followRunningTest` is on. If this setting is turned off, only failed tests will be revealed.
	"testing.alwaysRevealTestOnStateChange": false,

	// Configures when the error Peek view is automatically opened.
	//  - failureAnywhere: Open automatically no matter where the failure is.
	//  - failureInVisibleDocument: Open automatically when a test fails in a visible document.
	//  - never: Never automatically open.
	"testing.automaticallyOpenPeekView": "never",

	// Controls whether to automatically open the Peek view during continuous run mode.
	"testing.automaticallyOpenPeekViewDuringAutoRun": false,

	// Controls when the testing view should open.
	//  - neverOpen: Never automatically open the testing views
	//  - openOnTestStart: Open the test results view when tests start
	//  - openOnTestFailure: Open the test result view on any test failure
	//  - openExplorerOnTestStart: Open the test explorer when tests start
	"testing.automaticallyOpenTestResults": "openOnTestStart",

	// Controls the count badge on the Testing icon on the Activity Bar.
	//  - failed: Show the number of failed tests
	//  - off: Disable the testing count badge
	//  - passed: Show the number of passed tests
	//  - skipped: Show the number of skipped tests
	"testing.countBadge": "failed",

	// Configures the colors used for percentages in test coverage bars.
	"testing.coverageBarThresholds": {
		"red": 0,
		"yellow": 60,
		"green": 90
	},

	// Controls whether the coverage toolbar is shown in the editor.
	"testing.coverageToolbarEnabled": false,

	// Controls the action to take when left-clicking on a test decoration in the gutter.
	//  - run: Run the test.
	//  - debug: Debug the test.
	//  - runWithCoverage: Run the test with coverage.
	//  - contextMenu: Open the context menu for more options.
	"testing.defaultGutterClickAction": "run",

	// Configures what percentage is displayed by default for test coverage.
	//  - totalCoverage: A calculation of the combined statement, function, and branch coverage.
	//  - statement: The statement coverage.
	//  - minimum: The minimum of statement, function, and branch coverage.
	"testing.displayedCoveragePercent": "totalCoverage",

	// Controls whether the running test should be followed in the Test Explorer view.
	"testing.followRunningTest": false,

	// Controls whether test decorations are shown in the editor gutter.
	"testing.gutterEnabled": true,

	// Control whether save all dirty editors before running a test.
	"testing.saveBeforeTest": true,

	// Controls whether to show messages from all test runs.
	"testing.showAllMessages": false,

	// Whether test coverage should be down in the File Explorer view.
	"testing.showCoverageInExplorer": true,

	// Insert semicolon at end of line when completing CSS properties.
	"css.completion.completePropertyWithSemicolon": true,

	// By default, VS Code triggers property value completion after selecting a CSS property. Use this setting to disable this behavior.
	"css.completion.triggerPropertyValueCompletion": true,

	// A list of relative file paths pointing to JSON files following the [custom data format](https://github.com/microsoft/vscode-css-languageservice/blob/master/docs/customData.md).
	// 
	// VS Code loads custom data on startup to enhance its CSS support for CSS custom properties (variables), at-rules, pseudo-classes, and pseudo-elements you specify in the JSON files.
	// 
	// The file paths are relative to workspace and only workspace folder settings are considered.
	"css.customData": [],

	// Put braces on the same line as rules (`collapse`) or put braces on own line (`expand`).
	"css.format.braceStyle": "collapse",

	// Enable/disable default CSS formatter.
	"css.format.enable": true,

	// Maximum number of line breaks to be preserved in one chunk, when `css.format.preserveNewLines` is enabled.
	"css.format.maxPreserveNewLines": null,

	// Separate rulesets by a blank line.
	"css.format.newlineBetweenRules": true,

	// Separate selectors with a new line.
	"css.format.newlineBetweenSelectors": true,

	// Whether existing line breaks before rules and declarations should be preserved.
	"css.format.preserveNewLines": true,

	// Ensure a space character around selector separators '>', '+', '~' (e.g. `a > b`).
	"css.format.spaceAroundSelectorSeparator": false,

	// Show property and value documentation in CSS hovers.
	"css.hover.documentation": true,

	// Show references to MDN in CSS hovers.
	"css.hover.references": true,

	// Invalid number of parameters.
	"css.lint.argumentsInColorFunction": "error",

	// Do not use `width` or `height` when using `padding` or `border`.
	"css.lint.boxModel": "ignore",

	// When using a vendor-specific prefix make sure to also include all other vendor-specific properties.
	"css.lint.compatibleVendorPrefixes": "ignore",

	// Do not use duplicate style definitions.
	"css.lint.duplicateProperties": "ignore",

	// Do not use empty rulesets.
	"css.lint.emptyRules": "warning",

	// Avoid using `float`. Floats lead to fragile CSS that is easy to break if one aspect of the layout changes.
	"css.lint.float": "ignore",

	// `@font-face` rule must define `src` and `font-family` properties.
	"css.lint.fontFaceProperties": "warning",

	// Hex colors must consist of 3, 4, 6 or 8 hex numbers.
	"css.lint.hexColorLength": "error",

	// Selectors should not contain IDs because these rules are too tightly coupled with the HTML.
	"css.lint.idSelector": "ignore",

	// IE hacks are only necessary when supporting IE7 and older.
	"css.lint.ieHack": "ignore",

	// Avoid using `!important`. It is an indication that the specificity of the entire CSS has gotten out of control and needs to be refactored.
	"css.lint.important": "ignore",

	// Import statements do not load in parallel.
	"css.lint.importStatement": "ignore",

	// Property is ignored due to the display. E.g. with `display: inline`, the `width`, `height`, `margin-top`, `margin-bottom`, and `float` properties have no effect.
	"css.lint.propertyIgnoredDueToDisplay": "warning",

	// The universal selector (`*`) is known to be slow.
	"css.lint.universalSelector": "ignore",

	// Unknown at-rule.
	"css.lint.unknownAtRules": "warning",

	// Unknown property.
	"css.lint.unknownProperties": "warning",

	// Unknown vendor specific property.
	"css.lint.unknownVendorSpecificProperties": "ignore",

	// A list of properties that are not validated against the `unknownProperties` rule.
	"css.lint.validProperties": [],

	// When using a vendor-specific prefix, also include the standard property.
	"css.lint.vendorPrefix": "warning",

	// No unit for zero needed.
	"css.lint.zeroUnits": "ignore",

	// Traces the communication between VS Code and the CSS language server.
	"css.trace.server": "off",

	// Enables or disables all validations.
	"css.validate": true,

	// Insert semicolon at end of line when completing CSS properties.
	"less.completion.completePropertyWithSemicolon": true,

	// By default, VS Code triggers property value completion after selecting a CSS property. Use this setting to disable this behavior.
	"less.completion.triggerPropertyValueCompletion": true,

	// Put braces on the same line as rules (`collapse`) or put braces on own line (`expand`).
	"less.format.braceStyle": "collapse",

	// Enable/disable default LESS formatter.
	"less.format.enable": true,

	// Maximum number of line breaks to be preserved in one chunk, when `less.format.preserveNewLines` is enabled.
	"less.format.maxPreserveNewLines": null,

	// Separate rulesets by a blank line.
	"less.format.newlineBetweenRules": true,

	// Separate selectors with a new line.
	"less.format.newlineBetweenSelectors": true,

	// Whether existing line breaks before rules and declarations should be preserved.
	"less.format.preserveNewLines": true,

	// Ensure a space character around selector separators '>', '+', '~' (e.g. `a > b`).
	"less.format.spaceAroundSelectorSeparator": false,

	// Show property and value documentation in LESS hovers.
	"less.hover.documentation": true,

	// Show references to MDN in LESS hovers.
	"less.hover.references": true,

	// Invalid number of parameters.
	"less.lint.argumentsInColorFunction": "error",

	// Do not use `width` or `height` when using `padding` or `border`.
	"less.lint.boxModel": "ignore",

	// When using a vendor-specific prefix make sure to also include all other vendor-specific properties.
	"less.lint.compatibleVendorPrefixes": "ignore",

	// Do not use duplicate style definitions.
	"less.lint.duplicateProperties": "ignore",

	// Do not use empty rulesets.
	"less.lint.emptyRules": "warning",

	// Avoid using `float`. Floats lead to fragile CSS that is easy to break if one aspect of the layout changes.
	"less.lint.float": "ignore",

	// `@font-face` rule must define `src` and `font-family` properties.
	"less.lint.fontFaceProperties": "warning",

	// Hex colors must consist of 3, 4, 6 or 8 hex numbers.
	"less.lint.hexColorLength": "error",

	// Selectors should not contain IDs because these rules are too tightly coupled with the HTML.
	"less.lint.idSelector": "ignore",

	// IE hacks are only necessary when supporting IE7 and older.
	"less.lint.ieHack": "ignore",

	// Avoid using `!important`. It is an indication that the specificity of the entire CSS has gotten out of control and needs to be refactored.
	"less.lint.important": "ignore",

	// Import statements do not load in parallel.
	"less.lint.importStatement": "ignore",

	// Property is ignored due to the display. E.g. with `display: inline`, the `width`, `height`, `margin-top`, `margin-bottom`, and `float` properties have no effect.
	"less.lint.propertyIgnoredDueToDisplay": "warning",

	// The universal selector (`*`) is known to be slow.
	"less.lint.universalSelector": "ignore",

	// Unknown at-rule.
	"less.lint.unknownAtRules": "warning",

	// Unknown property.
	"less.lint.unknownProperties": "warning",

	// Unknown vendor specific property.
	"less.lint.unknownVendorSpecificProperties": "ignore",

	// A list of properties that are not validated against the `unknownProperties` rule.
	"less.lint.validProperties": [],

	// When using a vendor-specific prefix, also include the standard property.
	"less.lint.vendorPrefix": "warning",

	// No unit for zero needed.
	"less.lint.zeroUnits": "ignore",

	// Enables or disables all validations.
	"less.validate": true,

	// Insert semicolon at end of line when completing CSS properties.
	"scss.completion.completePropertyWithSemicolon": true,

	// By default, VS Code triggers property value completion after selecting a CSS property. Use this setting to disable this behavior.
	"scss.completion.triggerPropertyValueCompletion": true,

	// Put braces on the same line as rules (`collapse`) or put braces on own line (`expand`).
	"scss.format.braceStyle": "collapse",

	// Enable/disable default SCSS formatter.
	"scss.format.enable": true,

	// Maximum number of line breaks to be preserved in one chunk, when `scss.format.preserveNewLines` is enabled.
	"scss.format.maxPreserveNewLines": null,

	// Separate rulesets by a blank line.
	"scss.format.newlineBetweenRules": true,

	// Separate selectors with a new line.
	"scss.format.newlineBetweenSelectors": true,

	// Whether existing line breaks before rules and declarations should be preserved.
	"scss.format.preserveNewLines": true,

	// Ensure a space character around selector separators '>', '+', '~' (e.g. `a > b`).
	"scss.format.spaceAroundSelectorSeparator": false,

	// Show property and value documentation in SCSS hovers.
	"scss.hover.documentation": true,

	// Show references to MDN in SCSS hovers.
	"scss.hover.references": true,

	// Invalid number of parameters.
	"scss.lint.argumentsInColorFunction": "error",

	// Do not use `width` or `height` when using `padding` or `border`.
	"scss.lint.boxModel": "ignore",

	// When using a vendor-specific prefix make sure to also include all other vendor-specific properties.
	"scss.lint.compatibleVendorPrefixes": "ignore",

	// Do not use duplicate style definitions.
	"scss.lint.duplicateProperties": "ignore",

	// Do not use empty rulesets.
	"scss.lint.emptyRules": "warning",

	// Avoid using `float`. Floats lead to fragile CSS that is easy to break if one aspect of the layout changes.
	"scss.lint.float": "ignore",

	// `@font-face` rule must define `src` and `font-family` properties.
	"scss.lint.fontFaceProperties": "warning",

	// Hex colors must consist of 3, 4, 6 or 8 hex numbers.
	"scss.lint.hexColorLength": "error",

	// Selectors should not contain IDs because these rules are too tightly coupled with the HTML.
	"scss.lint.idSelector": "ignore",

	// IE hacks are only necessary when supporting IE7 and older.
	"scss.lint.ieHack": "ignore",

	// Avoid using `!important`. It is an indication that the specificity of the entire CSS has gotten out of control and needs to be refactored.
	"scss.lint.important": "ignore",

	// Import statements do not load in parallel.
	"scss.lint.importStatement": "ignore",

	// Property is ignored due to the display. E.g. with `display: inline`, the `width`, `height`, `margin-top`, `margin-bottom`, and `float` properties have no effect.
	"scss.lint.propertyIgnoredDueToDisplay": "warning",

	// The universal selector (`*`) is known to be slow.
	"scss.lint.universalSelector": "ignore",

	// Unknown at-rule.
	"scss.lint.unknownAtRules": "warning",

	// Unknown property.
	"scss.lint.unknownProperties": "warning",

	// Unknown vendor specific property.
	"scss.lint.unknownVendorSpecificProperties": "ignore",

	// A list of properties that are not validated against the `unknownProperties` rule.
	"scss.lint.validProperties": [],

	// When using a vendor-specific prefix, also include the standard property.
	"scss.lint.vendorPrefix": "warning",

	// No unit for zero needed.
	"scss.lint.zeroUnits": "ignore",

	// Enables or disables all validations.
	"scss.validate": true,

	// Specify a list of extensions that are allowed to use. This helps maintain a secure and consistent development environment by restricting the use of unauthorized extensions. For more information on how to configure this setting, please visit the [Configure Allowed Extensions](https://code.visualstudio.com/docs/setup/enterprise#_configure-allowed-extensions) section.
	"extensions.allowed": "*",

	// When enabled, automatically checks extensions for updates. If an extension has an update, it is marked as outdated in the Extensions view. The updates are fetched from a Microsoft online service.
	"extensions.autoCheckUpdates": true,

	// Controls the automatic update behavior of extensions. The updates are fetched from a Microsoft online service.
	//  - true: Download and install updates automatically for all extensions.
	//  - onlyEnabledExtensions: Download and install updates automatically only for enabled extensions.
	//  - false: Extensions are not automatically updated.
	"extensions.autoUpdate": true,

	// When enabled, editors with extension details will be automatically closed upon navigating away from the Extensions View.
	"extensions.closeExtensionDetailsOnViewChange": false,

	// When an extension is listed here, a confirmation prompt will not be shown when that extension handles a URI.
	"extensions.confirmedUriHandlerExtensionIds": [],

	// Configure an extension to execute in a different extension host process.
	"extensions.experimental.affinity": {},

	// When enabled, extensions which declare the `onStartupFinished` activation event will be activated after a timeout.
	"extensions.experimental.deferredStartupFinishedActivation": false,

	// When enabled, extensions can be searched for via Quick Access and report issues from there.
	"extensions.experimental.issueQuickAccess": true,

	// When enabled, extensions to update are fetched from Unpkg service.
	"extensions.gallery.useUnpkgResourceApi": true,

	// When enabled, the notifications for extension recommendations will not be shown.
	"extensions.ignoreRecommendations": false,

	// This setting is deprecated. Use extensions.ignoreRecommendations setting to control recommendation notifications. Use Extensions view's visibility actions to hide Recommended view by default.
	// 
	"extensions.showRecommendationsOnlyOnDemand": false,

	// Override the untrusted workspace support of an extension. Extensions using `true` will always be enabled. Extensions using `limited` will always be enabled, and the extension will hide functionality that requires trust. Extensions using `false` will only be enabled only when the workspace is trusted.
	"extensions.supportUntrustedWorkspaces": {},

	// Override the virtual workspaces support of an extension.
	"extensions.supportVirtualWorkspaces": {},

	// When enabled, extensions are verified to be signed before getting installed.
	"extensions.verifySignature": true,

	// Enable web worker extension host.
	//  - true: The Web Worker Extension Host will always be launched.
	//  - false: The Web Worker Extension Host will never be launched.
	//  - auto: The Web Worker Extension Host will be launched when a web extension needs it.
	"extensions.webWorker": "auto",

	// Enable/disable the ability of smart scrolling in the output view. Smart scrolling allows you to lock scrolling automatically when you click in the output view and unlocks when you click in the last line.
	"output.smartScroll.enabled": true,

	// List of extensions to be ignored while synchronizing. The identifier of an extension is always `${publisher}.${name}`. For example: `vscode.csharp`.
	"settingsSync.ignoredExtensions": [],

	// Configure settings to be ignored while synchronizing.
	"settingsSync.ignoredSettings": [],

	// Synchronize keybindings for each platform.
	"settingsSync.keybindingsPerPlatform": true,

	// Controls whether code cells in the interactive window are collapsed by default.
	"interactiveWindow.collapseCellInputCode": "fromEditor",

	// The limit of notebook output size in kilobytes (KB) where notebook files will no longer be backed up for hot reload. Use 0 for unlimited.
	"notebook.backup.sizeLimit": 10000,

	// When enabled, notebook breadcrumbs contain code cells.
	"notebook.breadcrumbs.showCodeCells": true,

	// Controls the verbosity of the cell execution time in the cell status bar.
	//  - default: The cell execution duration is visible, with advanced information in the hover tooltip.
	//  - verbose: The cell last execution timestamp and duration are visible, with advanced information in the hover tooltip.
	"notebook.cellExecutionTimeVerbosity": "default",

	// Show available diagnostics for cell failures.
	"notebook.cellFailureDiagnostics": true,

	// Controls where the focus indicator is rendered, either along the cell borders or on the left gutter.
	"notebook.cellFocusIndicator": "gutter",

	// Where the cell toolbar should be shown, or whether it should be hidden.
	"notebook.cellToolbarLocation": {
		"default": "right"
	},

	// Whether the cell toolbar should appear on hover or click.
	"notebook.cellToolbarVisibility": "click",

	// Control whether the notebook editor should be rendered in a compact form. For example, when turned on, it will decrease the left margin width.
	"notebook.compactView": true,

	// Control whether a confirmation prompt is required to delete a running cell.
	"notebook.confirmDeleteRunningCell": true,

	// Control whether outputs action should be rendered in the output toolbar.
	"notebook.consolidatedOutputButton": true,

	// Control whether extra actions are shown in a dropdown next to the run button.
	"notebook.consolidatedRunButton": false,

	// Defines a default notebook formatter which takes precedence over all other formatter settings. Must be the identifier of an extension contributing a formatter.
	//  - null: None
	//  - formulahendry.auto-rename-tag: Auto rename paired HTML/XML tag
	//  - formulahendry.code-runner: Run C, C++, Java, JS, PHP, Python, Perl, Ruby, Go, Lua, Groovy, PowerShell, CMD, BASH, F#, C#, VBScript, TypeScript, CoffeeScript, Scala, Swift, Julia, Crystal, OCaml, R, AppleScript, Elixir, VB.NET, Clojure, Haxe, Obj-C, Rust, Racket, Scheme, AutoHotkey, AutoIt, Kotlin, Dart, Pascal, Haskell, Nim, D, Lisp, Kit, V, SCSS, Sass, CUDA, Less, Fortran, Ring, Standard ML, Zig, Mojo, Erlang, SPWN, Pkl, Gleam
	//  - vscode.css-language-features: Provides rich language support for CSS, LESS and SCSS files.
	//  - vscode.html-language-features: Provides rich language support for HTML and Handlebar files
	//  - solnurkarim.html-to-css-autocompletion: Provides completion suggestions for classes and ids from markup documents to stylesheets.
	//  - vscode.json-language-features: Provides rich language support for JSON files.
	//  - vscode.markdown-language-features: Provides rich language support for Markdown.
	//  - vscode.markdown-math: Adds math support to Markdown in notebooks.
	//  - vscode.php-language-features: Provides rich language support for PHP files.
	//  - esbenp.prettier-vscode: Code formatter using prettier
	//  - ms-python.python: Python language support with extension access points for IntelliSense (Pylance), Debugging (Python Debugger), linting, formatting, refactoring, unit tests, and more.
	//  - vscode.typescript-language-features: Provides rich language support for JavaScript and TypeScript.
	//  - ecmel.vscode-html-css: CSS Intellisense for HTML
	//  - ms-python.vscode-pylance: A performant, feature-rich language server for Python in VS Code
	//  - standard.vscode-standard: Visual Studio Code extension for JavaScript Standard Style with automatic fixing.
	//  - BracketPairColorDLW.bracket-pair-color-dlw: Quickly 'Bracket Pair Color DLW' setting with a simple command
	//  - vscode.configuration-editing: Provides capabilities (advanced IntelliSense, auto-fixing) in configuration files like settings, launch, and extension recommendation files.
	//  - Wscats.cors-browser: 🚀Preview file in your default browser
	//  - vscode.debug-auto-launch: Helper for auto-attach feature when node-debug extensions are not active.
	//  - vscode.debug-server-ready: Open URI in browser if server under debugging is ready.
	//  - ms-python.debugpy: Python Debugger extension using debugpy.
	//  - atariq11700.debugpy-old: Python Debugger extension using `debugpy` for python <= 3.6.
	//  - vscode.emmet: Emmet support for VS Code
	//  - vscode.extension-editing: Provides linting capabilities for authoring extensions.
	//  - vscode.git: Git SCM Integration
	//  - vscode.git-base: Git static contributions and pickers.
	//  - vscode.github: GitHub features for VS Code
	//  - vscode.github-authentication: GitHub Authentication Provider
	//  - vscode.grunt: Extension to add Grunt capabilities to VS Code.
	//  - vscode.gulp: Extension to add Gulp capabilities to VSCode.
	//  - bianxianyang.htmlplay: html/js/css playground
	//  - vscode.ipynb: Provides basic support for opening and reading Jupyter's .ipynb notebook files
	//  - vscode.jake: Extension to add Jake capabilities to VS Code.
	//  - ms-vscode.js-debug: An extension for debugging Node.js programs and Chrome.
	//  - ms-vscode.js-debug-companion: Companion extension to js-debug that provides capability for remote debugging
	//  - ms-vscode.js-debug-nightly: An extension for debugging Node.js programs and Chrome.
	//  - ritwickdey.LiveServer: Launch a development local Server with live reload feature for static & dynamic pages
	//  - vscode.media-preview: Provides VS Code's built-in previews for images, audio, and video
	//  - vscode.merge-conflict: Highlighting and commands for inline merge conflicts.
	//  - vscode.microsoft-authentication: Microsoft authentication provider
	//  - vscode.npm: Extension to add task support for npm scripts.
	//  - christian-kohler.npm-intellisense: Visual Studio Code plugin that autocompletes npm modules in import statements
	//  - techer.open-in-browser: This allows you to open the current file in your default browser or application.
	//  - vscode.references-view: Reference Search results as separate, stable view in the sidebar
	//  - vscode.search-result: Provides syntax highlighting and language features for tabbed search results.
	//  - vscode.simple-browser: A very basic built-in webview for displaying web content.
	//  - vscode.terminal-suggest: Extension to add terminal completions for zsh, bash, and fish terminals.
	//  - vscode.tunnel-forwarding: Allows forwarding local ports to be accessible over the internet.
	//  - ms-vscode.vscode-js-profile-table: Text visualizer for profiles taken from the JavaScript debugger
	//  - GitHub.vscode-pull-request-github: Pull Request and Issue Provider for GitHub
	//  - vitaliymaz.vscode-svg-previewer: Show SVG preview to the side panel
	"notebook.defaultFormatter": null,

	// Whether to use the enhanced text diff editor for notebook.
	"notebook.diff.enablePreview": true,

	// Hide Metadata Differences
	"notebook.diff.ignoreMetadata": false,

	// Hide Outputs Differences
	"notebook.diff.ignoreOutputs": false,

	// Whether to render the overview ruler in the diff editor for notebook.
	"notebook.diff.overviewRuler": false,

	// Priority list for output mime types
	"notebook.displayOrder": [],

	// Control whether the notebook editor should allow moving cells through drag and drop.
	"notebook.dragAndDropEnabled": true,

	// Settings for code editors used in notebooks. This can be used to customize most editor.* settings.
	"notebook.editorOptionsCustomizations": {},

	// Enable experimental generate action to create code cell with inline chat enabled.
	"notebook.experimental.generate": true,

	// Enables the incremental saving of notebooks between processes and across Remote connections. When enabled, only the changes to the notebook are sent to the extension host, improving performance for large notebooks and slow network connections.
	"notebook.experimental.remoteSave": false,

	// Customize the Find Widget behavior for searching within notebook cells. When both markup source and markup preview are enabled, the Find Widget will search either the source code or preview based on the current state of the cell.
	"notebook.find.filters": {
		"markupSource": true,
		"markupPreview": true,
		"codeSource": true,
		"codeOutput": true
	},

	// Format a notebook cell upon execution. A formatter must be available.
	"notebook.formatOnCellExecution": false,

	// Format a notebook on save. A formatter must be available and the editor must not be shutting down. When `files.autoSave` is set to `afterDelay`, the file will only be formatted when saved explicitly.
	"notebook.formatOnSave.enabled": false,

	// Control whether to render a global toolbar inside the notebook editor.
	"notebook.globalToolbar": true,

	// Control whether the actions on the notebook toolbar should render label or not.
	"notebook.globalToolbarShowLabel": "always",

	// When enabled, the Go to Symbol Quick Pick will display full code symbols from the notebook, as well as Markdown headers.
	"notebook.gotoSymbols.showAllSymbols": true,

	// Enable the showing of inline values within notebook code cells after cell execution. Values will remain until the cell is edited, re-executed, or explicitly cleared via the Clear All Outputs toolbar button or the `Notebook: Clear Inline Values` command. 
	"notebook.inlineValues": false,

	// When enabled, insert a final new line into the end of code cells when saving a notebook.
	"notebook.insertFinalNewline": false,

	// Control where the insert cell actions should appear.
	//  - betweenCells: A toolbar that appears on hover between cells.
	//  - notebookToolbar: The toolbar at the top of the notebook editor.
	//  - both: Both toolbars.
	//  - hidden: The insert actions don't appear anywhere.
	"notebook.insertToolbarLocation": "both",

	// Controls the display of line numbers in the cell editor.
	"notebook.lineNumbers": "off",

	// Controls the line height in pixels of markdown cells in notebooks. When set to `0`, `normal` will be used
	"notebook.markdown.lineHeight": 0,

	// Controls the font family of rendered markup in notebooks. When left blank, this will fall back to the default workbench font family.
	"notebook.markup.fontFamily": "",

	// Controls the font size in pixels of rendered markup in notebooks. When set to `0`, 120% of `editor.fontSize` is used.
	"notebook.markup.fontSize": 0,

	// Experimental. Enables a limited set of multi cursor controls across multiple cells in the notebook editor. Currently supported are core editor actions (typing/cut/copy/paste/composition) and a limited subset of editor commands.
	"notebook.multiCursor.enabled": false,

	// When enabled cursor can navigate to the next/previous cell when the current cursor in the cell editor is at the first/last line.
	"notebook.navigation.allowNavigateToSurroundingCells": true,

	// When enabled, notebook outline shows code cells.
	"notebook.outline.showCodeCells": false,

	// When enabled, notebook outline shows code cell symbols. Relies on `notebook.outline.showCodeCells` being enabled.
	"notebook.outline.showCodeCellSymbols": true,

	// When enabled, notebook outline will show only markdown cells containing a header.
	"notebook.outline.showMarkdownHeadersOnly": true,

	// The font family of the output text within notebook cells. When set to empty, the `editor.fontFamily` is used.
	"notebook.output.fontFamily": "",

	// Font size for the output text within notebook cells. When set to 0, `editor.fontSize` is used.
	"notebook.output.fontSize": 0,

	// Line height of the output text within notebook cells.
	//  - When set to 0, editor line height is used.
	//  - Values between 0 and 8 will be used as a multiplier with the font size.
	//  - Values greater than or equal to 8 will be used as effective values.
	"notebook.output.lineHeight": 0,

	// Control whether to disable filepath links in the output of notebook cells.
	"notebook.output.linkifyFilePaths": true,

	// Control whether to render error output in a minimal style.
	"notebook.output.minimalErrorRendering": false,

	// Initially render notebook outputs in a scrollable region when longer than the limit.
	"notebook.output.scrolling": false,

	// Controls how many lines of text are displayed in a text output. If `notebook.output.scrolling` is enabled, this setting is used to determine the scroll height of the output.
	"notebook.output.textLineLimit": 30,

	// Controls whether the lines in output should wrap.
	"notebook.output.wordWrap": false,

	// How far to scroll when revealing the next cell upon running notebook.cell.executeAndSelectBelow.
	//  - fullCell: Scroll to fully reveal the next cell.
	//  - firstLine: Scroll to reveal the first line of the next cell.
	//  - none: Do not scroll.
	"notebook.scrolling.revealNextCellOnExecute": "fullCell",

	// Whether the cell status bar should be shown.
	//  - hidden: The cell Status bar is always hidden.
	//  - visible: The cell Status bar is always visible.
	//  - visibleAfterExecute: The cell Status bar is hidden until the cell has executed. Then it becomes visible to show the execution status.
	"notebook.showCellStatusBar": "visible",

	// Controls when the Markdown header folding arrow is shown.
	//  - always: The folding controls are always visible.
	//  - never: Never show the folding controls and reduce the gutter size.
	//  - mouseover: The folding controls are visible only on mouseover.
	"notebook.showFoldingControls": "mouseover",

	// Experimental. Control whether to render notebook Sticky Scroll headers in the notebook editor.
	"notebook.stickyScroll.enabled": false,

	// Control whether nested sticky lines appear to stack flat or indented.
	//  - flat: Nested sticky lines appear flat.
	//  - indented: Nested sticky lines appear indented.
	"notebook.stickyScroll.mode": "indented",

	// Whether to use separate undo/redo stack for each cell.
	"notebook.undoRedoPerCell": true,

	// Enable the experimental notebook variables view within the debug panel.
	"notebook.variablesView": false,

	// Automatically scroll the interactive window to show the output of the last statement executed. If this value is false, the window will only scroll if the last cell was already the one scrolled to.
	"interactiveWindow.alwaysScrollOnNewCell": true,

	// Execute the Interactive Window (REPL) input box with shift+enter, so that enter can be used to create a newline.
	"interactiveWindow.executeWithShiftEnter": false,

	// Prompt to save the interactive window when it is closed. Only new interactive windows will be affected by this setting change.
	"interactiveWindow.promptToSaveOnClose": false,

	// Display a hint in the Interactive Window (REPL) input box to indicate how to execute code.
	"interactiveWindow.showExecutionHint": true,

	// When enabled, slow renderers are automatically profiled.
	"application.experimental.rendererProfiling": false,

	// When opening a file from the Explorer in a terminal, determines what kind of terminal will be launched
	//  - integrated: Use VS Code's integrated terminal.
	//  - external: Use the configured external terminal.
	//  - both: Use the other two together.
	"terminal.explorerKind": "integrated",

	// Customizes which terminal to run on Linux.
	"terminal.external.linuxExec": "xterm",

	// Customizes which terminal application to run on macOS.
	"terminal.external.osxExec": "Terminal.app",

	// Customizes which terminal to run on Windows.
	"terminal.external.windowsExec": "C:\\Windows\\System32\\cmd.exe",

	// When opening a repository from the Source Control Repositories view in a terminal, determines what kind of terminal will be launched
	//  - integrated: Use VS Code's integrated terminal.
	//  - external: Use the configured external terminal.
	//  - both: Use the other two together.
	"terminal.sourceControlRepositoriesKind": "integrated",

	// Focus the terminal accessible view when a command is executed.
	"terminal.integrated.accessibleViewFocusOnCommandExecution": false,

	// Preserve the cursor position on reopen of the terminal's accessible view rather than setting it to the bottom of the buffer.
	"terminal.integrated.accessibleViewPreserveCursorPosition": false,

	// Whether or not to allow chord keybindings in the terminal. Note that when this is true and the keystroke results in a chord it will bypass `terminal.integrated.commandsToSkipShell`, setting this to false is particularly useful when you want ctrl+k to go to your shell (not VS Code).
	"terminal.integrated.allowChords": true,

	// An array of strings containing the URI schemes that the terminal is allowed to open links for. By default, only a small subset of possible schemes are allowed for security reasons.
	"terminal.integrated.allowedLinkSchemes": [
		"file",
		"http",
		"https",
		"mailto",
		"vscode",
		"vscode-insiders"
	],

	// Whether to allow menubar mnemonics (for example Alt+F) to trigger the open of the menubar. Note that this will cause all alt keystrokes to skip the shell when true. This does nothing on macOS.
	"terminal.integrated.allowMnemonics": false,

	// If enabled, alt/option + click will reposition the prompt cursor to underneath the mouse when `editor.multiCursorModifier` is set to `'alt'` (the default value). This may not work reliably depending on your shell.
	"terminal.integrated.altClickMovesCursor": true,

	// The terminal profile to use on Linux for automation-related terminal usage like tasks and debug.
	"terminal.integrated.automationProfile.linux": null,

	// The terminal profile to use on macOS for automation-related terminal usage like tasks and debug.
	"terminal.integrated.automationProfile.osx": null,

	// The terminal profile to use for automation-related terminal usage like tasks and debug. This setting will currently be ignored if `terminal.integrated.automationShell.windows` (now deprecated) is set.
	"terminal.integrated.automationProfile.windows": null,

	// A set of messages that, when encountered in the terminal, will be automatically responded to. Provided the message is specific enough, this can help automate away common responses.
	// 
	// Remarks:
	// 
	// - Use `"Terminate batch job (Y/N)": "Y\r"` to automatically respond to the terminate batch job prompt on Windows.
	// - The message includes escape sequences so the reply might not happen with styled text.
	// - Each reply can only happen once every second.
	// - Use `"\r"` in the reply to mean the enter key.
	// - To unset a default key, set the value to null.
	// - Restart VS Code if new don't apply.
	"terminal.integrated.autoReplies": {},

	// The number of milliseconds to show the bell within a terminal tab when triggered.
	"terminal.integrated.bellDuration": 1000,

	// A set of command IDs whose keybindings will not be sent to the shell but instead always be handled by VS Code. This allows keybindings that would normally be consumed by the shell to act instead the same as when the terminal is not focused, for example `Ctrl+P` to launch Quick Open.
	// 
	// &nbsp;
	// 
	// Many commands are skipped by default. To override a default and pass that command's keybinding to the shell instead, add the command prefixed with the `-` character. For example add `-workbench.action.quickOpen` to allow `Ctrl+P` to reach the shell.
	// 
	// &nbsp;
	// 
	// The following list of default skipped commands is truncated when viewed in Settings Editor. To see the full list, [open the default settings JSON](command:workbench.action.openRawDefaultSettings 'Open Default Settings (JSON)') and search for the first command from the list below.
	// 
	// &nbsp;
	// 
	// Default Skipped Commands:
	// 
	// - editor.action.accessibilityHelp
	// - editor.action.toggleTabFocusMode
	// - notification.acceptPrimaryAction
	// - notifications.hideList
	// - notifications.hideToasts
	// - runCommands
	// - workbench.action.closeQuickOpen
	// - workbench.action.debug.continue
	// - workbench.action.debug.disconnect
	// - workbench.action.debug.pause
	// - workbench.action.debug.restart
	// - workbench.action.debug.run
	// - workbench.action.debug.start
	// - workbench.action.debug.stepInto
	// - workbench.action.debug.stepOut
	// - workbench.action.debug.stepOver
	// - workbench.action.debug.stop
	// - workbench.action.firstEditorInGroup
	// - workbench.action.focusActiveEditorGroup
	// - workbench.action.focusEighthEditorGroup
	// - workbench.action.focusFifthEditorGroup
	// - workbench.action.focusFirstEditorGroup
	// - workbench.action.focusFourthEditorGroup
	// - workbench.action.focusLastEditorGroup
	// - workbench.action.focusNextPart
	// - workbench.action.focusPreviousPart
	// - workbench.action.focusSecondEditorGroup
	// - workbench.action.focusSeventhEditorGroup
	// - workbench.action.focusSixthEditorGroup
	// - workbench.action.focusThirdEditorGroup
	// - workbench.action.lastEditorInGroup
	// - workbench.action.navigateDown
	// - workbench.action.navigateLeft
	// - workbench.action.navigateRight
	// - workbench.action.navigateUp
	// - workbench.action.nextEditor
	// - workbench.action.nextEditorInGroup
	// - workbench.action.nextPanelView
	// - workbench.action.nextSideBarView
	// - workbench.action.openNextRecentlyUsedEditor
	// - workbench.action.openNextRecentlyUsedEditorInGroup
	// - workbench.action.openPreviousRecentlyUsedEditor
	// - workbench.action.openPreviousRecentlyUsedEditorInGroup
	// - workbench.action.previousEditor
	// - workbench.action.previousEditorInGroup
	// - workbench.action.previousPanelView
	// - workbench.action.previousSideBarView
	// - workbench.action.quickOpen
	// - workbench.action.quickOpenLeastRecentlyUsedEditor
	// - workbench.action.quickOpenLeastRecentlyUsedEditorInGroup
	// - workbench.action.quickOpenPreviousEditor
	// - workbench.action.quickOpenPreviousRecentlyUsedEditor
	// - workbench.action.quickOpenPreviousRecentlyUsedEditorInGroup
	// - workbench.action.quickOpenView
	// - workbench.action.showCommands
	// - workbench.action.tasks.build
	// - workbench.action.tasks.reRunTask
	// - workbench.action.tasks.restartTask
	// - workbench.action.tasks.runTask
	// - workbench.action.tasks.showLog
	// - workbench.action.tasks.showTasks
	// - workbench.action.tasks.terminate
	// - workbench.action.tasks.test
	// - workbench.action.terminal.acceptSelectedSuggestion
	// - workbench.action.terminal.acceptSelectedSuggestionEnter
	// - workbench.action.terminal.chat.cancel
	// - workbench.action.terminal.chat.close
	// - workbench.action.terminal.chat.discard
	// - workbench.action.terminal.chat.feedbackHelpful
	// - workbench.action.terminal.chat.feedbackReportIssue
	// - workbench.action.terminal.chat.feedbackUnhelpful
	// - workbench.action.terminal.chat.insertCommand
	// - workbench.action.terminal.chat.makeRequest
	// - workbench.action.terminal.chat.runCommand
	// - workbench.action.terminal.chat.start
	// - workbench.action.terminal.chat.viewInChat
	// - workbench.action.terminal.clear
	// - workbench.action.terminal.clearSelection
	// - workbench.action.terminal.clearSuggestCache
	// - workbench.action.terminal.copyAndClearSelection
	// - workbench.action.terminal.copyLastCommand
	// - workbench.action.terminal.copyLastCommandAndLastCommandOutput
	// - workbench.action.terminal.copyLastCommandOutput
	// - workbench.action.terminal.copySelection
	// - workbench.action.terminal.copySelectionAsHtml
	// - workbench.action.terminal.deleteToLineStart
	// - workbench.action.terminal.deleteWordLeft
	// - workbench.action.terminal.deleteWordRight
	// - workbench.action.terminal.findNext
	// - workbench.action.terminal.findPrevious
	// - workbench.action.terminal.focus
	// - workbench.action.terminal.focusAccessibleBuffer
	// - workbench.action.terminal.focusAtIndex1
	// - workbench.action.terminal.focusAtIndex2
	// - workbench.action.terminal.focusAtIndex3
	// - workbench.action.terminal.focusAtIndex4
	// - workbench.action.terminal.focusAtIndex5
	// - workbench.action.terminal.focusAtIndex6
	// - workbench.action.terminal.focusAtIndex7
	// - workbench.action.terminal.focusAtIndex8
	// - workbench.action.terminal.focusAtIndex9
	// - workbench.action.terminal.focusFind
	// - workbench.action.terminal.focusHover
	// - workbench.action.terminal.focusNext
	// - workbench.action.terminal.focusNextPane
	// - workbench.action.terminal.focusPrevious
	// - workbench.action.terminal.focusPreviousPane
	// - workbench.action.terminal.goToRecentDirectory
	// - workbench.action.terminal.hideFind
	// - workbench.action.terminal.hideSuggestWidget
	// - workbench.action.terminal.kill
	// - workbench.action.terminal.killEditor
	// - workbench.action.terminal.moveToEditor
	// - workbench.action.terminal.moveToLineEnd
	// - workbench.action.terminal.moveToLineStart
	// - workbench.action.terminal.moveToTerminalPanel
	// - workbench.action.terminal.new
	// - workbench.action.terminal.newInActiveWorkspace
	// - workbench.action.terminal.paste
	// - workbench.action.terminal.pasteSelection
	// - workbench.action.terminal.requestCompletions
	// - workbench.action.terminal.resizePaneDown
	// - workbench.action.terminal.resizePaneLeft
	// - workbench.action.terminal.resizePaneRight
	// - workbench.action.terminal.resizePaneUp
	// - workbench.action.terminal.runActiveFile
	// - workbench.action.terminal.runRecentCommand
	// - workbench.action.terminal.runSelectedText
	// - workbench.action.terminal.scrollDown
	// - workbench.action.terminal.scrollDownPage
	// - workbench.action.terminal.scrollToBottom
	// - workbench.action.terminal.scrollToNextCommand
	// - workbench.action.terminal.scrollToPreviousCommand
	// - workbench.action.terminal.scrollToTop
	// - workbench.action.terminal.scrollUp
	// - workbench.action.terminal.scrollUpPage
	// - workbench.action.terminal.searchWorkspace
	// - workbench.action.terminal.selectAll
	// - workbench.action.terminal.selectNextPageSuggestion
	// - workbench.action.terminal.selectNextSuggestion
	// - workbench.action.terminal.selectPrevPageSuggestion
	// - workbench.action.terminal.selectPrevSuggestion
	// - workbench.action.terminal.selectToNextCommand
	// - workbench.action.terminal.selectToNextLine
	// - workbench.action.terminal.selectToPreviousCommand
	// - workbench.action.terminal.selectToPreviousLine
	// - workbench.action.terminal.sendSequence
	// - workbench.action.terminal.sizeToContentWidth
	// - workbench.action.terminal.split
	// - workbench.action.terminal.splitInActiveWorkspace
	// - workbench.action.terminal.suggestToggleDetails
	// - workbench.action.terminal.suggestToggleDetailsFocus
	// - workbench.action.terminal.toggleFindCaseSensitive
	// - workbench.action.terminal.toggleFindRegex
	// - workbench.action.terminal.toggleFindWholeWord
	// - workbench.action.terminal.toggleTerminal
	// - workbench.action.toggleFullScreen
	// - workbench.action.toggleMaximizedPanel
	// - workbench.action.togglePanel
	"terminal.integrated.commandsToSkipShell": [],

	// Controls whether to confirm when the window closes if there are active terminal sessions.
	//  - never: Never confirm.
	//  - always: Always confirm if there are terminals.
	//  - hasChildProcesses: Confirm if there are any terminals that have child processes.
	"terminal.integrated.confirmOnExit": "never",

	// Controls whether to confirm killing terminals when they have child processes. When set to editor, terminals in the editor area will be marked as changed when they have child processes. Note that child process detection may not work well for shells like Git Bash which don't run their processes as child processes of the shell. Background terminals like those launched by some extensions will not trigger the confirmation.
	//  - never: Never confirm.
	//  - editor: Confirm if the terminal is in the editor.
	//  - panel: Confirm if the terminal is in the panel.
	//  - always: Confirm if the terminal is either in the editor or panel.
	"terminal.integrated.confirmOnKill": "editor",

	// Controls whether text selected in the terminal will be copied to the clipboard.
	"terminal.integrated.copyOnSelection": false,

	// Controls whether the terminal cursor blinks.
	"terminal.integrated.cursorBlinking": false,

	// Controls the style of terminal cursor when the terminal is focused.
	"terminal.integrated.cursorStyle": "block",

	// Controls the style of terminal cursor when the terminal is not focused.
	"terminal.integrated.cursorStyleInactive": "outline",

	// Controls the width of the cursor when `terminal.integrated.cursorStyle` is set to `line`.
	"terminal.integrated.cursorWidth": 1,

	// Whether to draw custom glyphs for block element and box drawing characters instead of using the font, which typically yields better rendering with continuous lines. Note that this doesn't work when `terminal.integrated.gpuAcceleration` is disabled.
	"terminal.integrated.customGlyphs": true,

	// An explicit start path where the terminal will be launched, this is used as the current working directory (cwd) for the shell process. This may be particularly useful in workspace settings if the root directory is not a convenient cwd.
	"terminal.integrated.cwd": "",

	// Controls where newly created terminals will appear.
	//  - editor: Create terminals in the editor
	//  - view: Create terminals in the terminal view
	"terminal.integrated.defaultLocation": "view",

	// The default terminal profile on Linux.
	"terminal.integrated.defaultProfile.linux": null,

	// The default terminal profile on macOS.
	"terminal.integrated.defaultProfile.osx": null,

	// The default terminal profile on Windows.
	//  - null: Automatically detect the default
	//  - PowerShell: $(terminal-powershell) PowerShell
	// - path: C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
	//  - Windows PowerShell: $(terminal-powershell) Windows PowerShell
	// - path: C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
	//  - Git Bash: $(terminal) Git Bash
	// - path: C:\Users\Daud A\AppData\Local\Programs\Git\bin\bash.exe
	// - args: ['--login','-i']
	//  - Command Prompt: $(terminal-cmd) Command Prompt
	// - path: C:\Windows\System32\cmd.exe
	// - args: []
	//  - JavaScript Debug Terminal: $($(debug)) JavaScript Debug Terminal
	// - extensionIdentifier: ms-vscode.js-debug
	//  - JavaScript Debug Terminal: $($(debug)) JavaScript Debug Terminal
	// - extensionIdentifier: ms-vscode.js-debug-nightly
	"terminal.integrated.defaultProfile.windows": null,

	// Controls whether to detect and set the `$LANG` environment variable to a UTF-8 compliant option since VS Code's terminal only supports UTF-8 encoded data coming from the shell.
	//  - auto: Set the `$LANG` environment variable if the existing variable does not exist or it does not end in `'.UTF-8'`.
	//  - off: Do not set the `$LANG` environment variable.
	//  - on: Always set the `$LANG` environment variable.
	"terminal.integrated.detectLocale": "auto",

	// Controls whether bold text in the terminal will always use the "bright" ANSI color variant.
	"terminal.integrated.drawBoldTextInBrightColors": true,

	// This is now deprecated. Instead use the `terminal.integrated.enableVisualBell` and `accessibility.signals.terminalBell` settings.
	// 
	"terminal.integrated.enableBell": false,

	// Whether to enable file links in terminals. Links can be slow when working on a network drive in particular because each file link is verified against the file system. Changing this will take effect only in new terminals.
	//  - off: Always off.
	//  - on: Always on.
	//  - notRemote: Enable only when not in a remote workspace.
	"terminal.integrated.enableFileLinks": "on",

	// Enables image support in the terminal, this will only work when `terminal.integrated.gpuAcceleration#` is enabled. Both sixel and iTerm's inline image protocol are supported on Linux and macOS. This will only work on Windows for versions of ConPTY >= v2 which is shipped with Windows itself, see also `#terminal.integrated.experimental.windowsUseConptyDll`. Images will currently not be restored between window reloads/reconnects.
	"terminal.integrated.enableImages": false,

	// Controls whether to show a warning dialog when pasting multiple lines into the terminal.
	//  - auto: Enable the warning but do not show it when:
	// 
	// - Bracketed paste mode is enabled (the shell supports multi-line paste natively)
	// - The paste is handled by the shell's readline (in the case of pwsh)
	//  - always: Always show the warning if the text contains a new line.
	//  - never: Never show the warning.
	"terminal.integrated.enableMultiLinePasteWarning": "auto",

	// Persist terminal sessions/history for the workspace across window reloads.
	"terminal.integrated.enablePersistentSessions": true,

	// Controls whether the visual terminal bell is enabled. This shows up next to the terminal's name.
	"terminal.integrated.enableVisualBell": false,

	// Object with environment variables that will be added to the VS Code process to be used by the terminal on Linux. Set to `null` to delete the environment variable.
	"terminal.integrated.env.linux": {},

	// Object with environment variables that will be added to the VS Code process to be used by the terminal on macOS. Set to `null` to delete the environment variable.
	"terminal.integrated.env.osx": {},

	// Object with environment variables that will be added to the VS Code process to be used by the terminal on Windows. Set to `null` to delete the environment variable.
	"terminal.integrated.env.windows": {},

	// Whether to display the environment changes indicator on each terminal which explains whether extensions have made, or want to make changes to the terminal's environment.
	//  - off: Disable the indicator.
	//  - on: Enable the indicator.
	//  - warnonly: Only show the warning indicator when a terminal's environment is 'stale', not the information indicator that shows a terminal has had its environment modified by an extension.
	"terminal.integrated.environmentChangesIndicator": "warnonly",

	// Whether to relaunch terminals automatically if extensions want to contribute to their environment and have not been interacted with yet.
	"terminal.integrated.environmentChangesRelaunch": true,

	// Whether to use the experimental conpty.dll (v1.20.240626001) shipped with VS Code, instead of the one bundled with Windows.
	"terminal.integrated.experimental.windowsUseConptyDll": false,

	// Scrolling speed multiplier when pressing `Alt`.
	"terminal.integrated.fastScrollSensitivity": 5,

	// Controls whether the terminal, accessible buffer, or neither will be focused after `Terminal: Run Selected Text In Active Terminal` has been run.
	//  - terminal: Always focus the terminal.
	//  - accessible-buffer: Always focus the accessible buffer.
	//  - none: Do nothing.
	"terminal.integrated.focusAfterRun": "none",

	// Controls the font family of the terminal. Defaults to `editor.fontFamily`'s value.
	"terminal.integrated.fontFamily": "",

	// Controls whether font ligatures are enabled in the terminal. Ligatures will only work if the configured `terminal.integrated.fontFamily` supports them.
	"terminal.integrated.fontLigatures.enabled": false,

	// When `terminal.integrated.gpuAcceleration#` is enabled and the particular `#terminal.integrated.fontFamily` cannot be parsed, this is the set of character sequences that will always be drawn together. This allows the use of a fixed set of ligatures even when the font isn't supported.
	"terminal.integrated.fontLigatures.fallbackLigatures": [
		"<--",
		"<---",
		"<<-",
		"<-",
		"->",
		"->>",
		"-->",
		"--->",
		"<==",
		"<===",
		"<<=",
		"<=",
		"=>",
		"=>>",
		"==>",
		"===>",
		">=",
		">>=",
		"<->",
		"<-->",
		"<--->",
		"<---->",
		"<=>",
		"<==>",
		"<===>",
		"<====>",
		"::",
		":::",
		"<~~",
		"</",
		"</>",
		"/>",
		"~~>",
		"==",
		"!=",
		"/=",
		"~=",
		"<>",
		"===",
		"!==",
		"!===",
		"<:",
		":=",
		"*=",
		"*+",
		"<*",
		"<*>",
		"*>",
		"<|",
		"<|>",
		"|>",
		"+*",
		"=*",
		"=:",
		":>",
		"/*",
		"*/",
		"+++",
		"<!--",
		"<!---"
	],

	// Controls what font feature settings are used when ligatures are enabled, in the format of the `font-feature-settings` CSS property. Some examples which may be valid depending on the font:
	// 
	// - `"calt" off, "ss03"`
	// - `"liga" on`
	// - `"calt" off, "dlig" on`
	"terminal.integrated.fontLigatures.featureSettings": "\"calt\" on",

	// Controls the font size in pixels of the terminal.
	"terminal.integrated.fontSize": 14,

	// The font weight to use within the terminal for non-bold text. Accepts "normal" and "bold" keywords or numbers between 1 and 1000.
	"terminal.integrated.fontWeight": "normal",

	// The font weight to use within the terminal for bold text. Accepts "normal" and "bold" keywords or numbers between 1 and 1000.
	"terminal.integrated.fontWeightBold": "bold",

	// Controls whether the terminal will leverage the GPU to do its rendering.
	//  - auto: Let VS Code detect which renderer will give the best experience.
	//  - on: Enable GPU acceleration within the terminal.
	//  - off: Disable GPU acceleration within the terminal. The terminal will render much slower when GPU acceleration is off but it should reliably work on all systems.
	"terminal.integrated.gpuAcceleration": "auto",

	// Whether to hide the terminal view when the last terminal is closed. This will only happen when the terminal is the only visible view in the view container.
	"terminal.integrated.hideOnLastClosed": true,

	// Whether to hide the terminal view on startup, avoiding creating a terminal when there are no persistent sessions.
	//  - never: Never hide the terminal view on startup.
	//  - whenEmpty: Only hide the terminal when there are no persistent sessions restored.
	//  - always: Always hide the terminal, even when there are persistent sessions restored.
	"terminal.integrated.hideOnStartup": "never",

	// Controls whether the terminal will ignore bracketed paste mode even if the terminal was put into the mode, omitting the `\x1b[200~` and `\x1b[201~` sequences when pasting. This is useful when the shell is not respecting the mode which can happen in sub-shells for example.
	"terminal.integrated.ignoreBracketedPasteMode": false,

	// A set of process names to ignore when using the `terminal.integrated.confirmOnKill` setting.
	"terminal.integrated.ignoreProcessNames": [
		"starship",
		"oh-my-posh",
		"bash",
		"zsh"
	],

	// Whether new shells should inherit their environment from VS Code, which may source a login shell to ensure $PATH and other development variables are initialized. This has no effect on Windows.
	"terminal.integrated.inheritEnv": true,

	// Controls if the first terminal without input will show a hint about available actions when it is focused.
	"terminal.integrated.initialHint": true,

	// Controls the letter spacing of the terminal. This is an integer value which represents the number of additional pixels to add between characters.
	"terminal.integrated.letterSpacing": 0,

	// Controls the line height of the terminal. This number is multiplied by the terminal font size to get the actual line-height in pixels.
	"terminal.integrated.lineHeight": 1,

	// When local echo should be enabled. This will override `terminal.integrated.localEchoLatencyThreshold`
	//  - on: Always enabled
	//  - off: Always disabled
	//  - auto: Enabled only for remote workspaces
	"terminal.integrated.localEchoEnabled": "auto",

	// Local echo will be disabled when any of these program names are found in the terminal title.
	"terminal.integrated.localEchoExcludePrograms": [
		"vim",
		"vi",
		"nano",
		"tmux"
	],

	// Length of network delay, in milliseconds, where local edits will be echoed on the terminal without waiting for server acknowledgement. If '0', local echo will always be on, and if '-1' it will be disabled.
	"terminal.integrated.localEchoLatencyThreshold": 30,

	// Terminal style of locally echoed text; either a font style or an RGB color.
	"terminal.integrated.localEchoStyle": "dim",

	// Controls whether to force selection when using Option+click on macOS. This will force a regular (line) selection and disallow the use of column selection mode. This enables copying and pasting using the regular terminal selection, for example, when mouse mode is enabled in tmux.
	"terminal.integrated.macOptionClickForcesSelection": false,

	// Controls whether to treat the option key as the meta key in the terminal on macOS.
	"terminal.integrated.macOptionIsMeta": false,

	// Controls how terminal reacts to middle click.
	//  - default: The platform default to focus the terminal. On Linux this will also paste the selection.
	//  - paste: Paste on middle click.
	"terminal.integrated.middleClickBehavior": "default",

	// When set, the foreground color of each cell will change to try meet the contrast ratio specified. Note that this will not apply to `powerline` characters per #146406. Example values:
	// 
	// - 1: Do nothing and use the standard theme colors.
	// - 4.5: [WCAG AA compliance (minimum)](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html) (default).
	// - 7: [WCAG AAA compliance (enhanced)](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast7.html).
	// - 21: White on black or black on white.
	"terminal.integrated.minimumContrastRatio": 4.5,

	// A multiplier to be used on the `deltaY` of mouse wheel scroll events.
	"terminal.integrated.mouseWheelScrollSensitivity": 1,

	// Zoom the font of the terminal when using mouse wheel and holding `Ctrl`.
	"terminal.integrated.mouseWheelZoom": false,

	// When the terminal process must be shut down (for example on window or application close), this determines when the previous terminal session contents/history should be restored and processes be recreated when the workspace is next opened.
	// 
	// Caveats:
	// 
	// - Restoring of the process current working directory depends on whether it is supported by the shell.
	// - Time to persist the session during shutdown is limited, so it may be aborted when using high-latency remote connections.
	//  - onExit: Revive the processes after the last window is closed on Windows/Linux or when the `workbench.action.quit` command is triggered (command palette, keybinding, menu).
	//  - onExitAndWindowClose: Revive the processes after the last window is closed on Windows/Linux or when the `workbench.action.quit` command is triggered (command palette, keybinding, menu), or when the window is closed.
	//  - never: Never restore the terminal buffers or recreate the process.
	"terminal.integrated.persistentSessionReviveProcess": "onExit",

	// Controls the maximum amount of lines that will be restored when reconnecting to a persistent terminal session. Increasing this will restore more lines of scrollback at the cost of more memory and increase the time it takes to connect to terminals on start up. This setting requires a restart to take effect and should be set to a value less than or equal to `terminal.integrated.scrollback`.
	"terminal.integrated.persistentSessionScrollback": 100,

	// A set of terminal profile customizations for Linux which allows adding, removing or changing how terminals are launched. Profiles are made up of a mandatory path, optional arguments and other presentation options.
	// 
	// To override an existing profile use its profile name as the key, for example:
	// 
	// ```json
	// "terminal.integrated.profile.linux": {
	//   "bash": null
	// }
	// ```
	// 
	// [Read more about configuring profiles](https://code.visualstudio.com/docs/terminal/profiles).
	"terminal.integrated.profiles.linux": {
		"bash": {
			"path": "bash",
			"icon": "terminal-bash"
		},
		"zsh": {
			"path": "zsh"
		},
		"fish": {
			"path": "fish"
		},
		"tmux": {
			"path": "tmux",
			"icon": "terminal-tmux"
		},
		"pwsh": {
			"path": "pwsh",
			"icon": "terminal-powershell"
		}
	},

	// A set of terminal profile customizations for Mac which allows adding, removing or changing how terminals are launched. Profiles are made up of a mandatory path, optional arguments and other presentation options.
	// 
	// To override an existing profile use its profile name as the key, for example:
	// 
	// ```json
	// "terminal.integrated.profile.osx": {
	//   "bash": null
	// }
	// ```
	// 
	// [Read more about configuring profiles](https://code.visualstudio.com/docs/terminal/profiles).
	"terminal.integrated.profiles.osx": {
		"bash": {
			"path": "bash",
			"args": [
				"-l"
			],
			"icon": "terminal-bash"
		},
		"zsh": {
			"path": "zsh",
			"args": [
				"-l"
			]
		},
		"fish": {
			"path": "fish",
			"args": [
				"-l"
			]
		},
		"tmux": {
			"path": "tmux",
			"icon": "terminal-tmux"
		},
		"pwsh": {
			"path": "pwsh",
			"icon": "terminal-powershell"
		}
	},

	// A set of terminal profile customizations for Windows which allows adding, removing or changing how terminals are launched. Profiles are made up of a mandatory path, optional arguments and other presentation options.
	// 
	// To override an existing profile use its profile name as the key, for example:
	// 
	// ```json
	// "terminal.integrated.profile.windows": {
	//   "bash": null
	// }
	// ```
	// 
	// [Read more about configuring profiles](https://code.visualstudio.com/docs/terminal/profiles).
	"terminal.integrated.profiles.windows": {
		"PowerShell": {
			"source": "PowerShell",
			"icon": "terminal-powershell"
		},
		"Command Prompt": {
			"path": [
				"${env:windir}\\Sysnative\\cmd.exe",
				"${env:windir}\\System32\\cmd.exe"
			],
			"args": [],
			"icon": "terminal-cmd"
		},
		"Git Bash": {
			"source": "Git Bash"
		}
	},

	// Whether to rescale glyphs horizontally that are a single cell wide but have glyphs that would overlap following cell(s). This typically happens for ambiguous width characters (eg. the roman numeral characters U+2160+) which aren't featured in monospace fonts. Emoji glyphs are never rescaled.
	"terminal.integrated.rescaleOverlappingGlyphs": true,

	// Controls how terminal reacts to right click.
	//  - default: Show the context menu.
	//  - copyPaste: Copy when there is a selection, otherwise paste.
	//  - paste: Paste on right click.
	//  - selectWord: Select the word under the cursor and show the context menu.
	//  - nothing: Do nothing and pass event to terminal.
	"terminal.integrated.rightClickBehavior": "copyPaste",

	// Controls the maximum number of lines the terminal keeps in its buffer. We pre-allocate memory based on this value in order to ensure a smooth experience. As such, as the value increases, so will the amount of memory.
	"terminal.integrated.scrollback": 1000,

	// Dispatches most keybindings to the terminal instead of the workbench, overriding `terminal.integrated.commandsToSkipShell`, which can be used alternatively for fine tuning.
	"terminal.integrated.sendKeybindingsToShell": false,

	// When shell integration is enabled, adds a decoration for each command.
	//  - both: Show decorations in the gutter (left) and overview ruler (right)
	//  - gutter: Show gutter decorations to the left of the terminal
	//  - overviewRuler: Show overview ruler decorations to the right of the terminal
	//  - never: Do not show decorations
	"terminal.integrated.shellIntegration.decorationsEnabled": "both",

	// Determines whether or not shell integration is auto-injected to support features like enhanced command tracking and current working directory detection. 
	// 
	// Shell integration works by injecting the shell with a startup script. The script gives VS Code insight into what is happening within the terminal.
	// 
	// Supported shells:
	// 
	// - Linux/macOS: bash, fish, pwsh, zsh
	//  - Windows: pwsh, git bash
	// 
	// This setting applies only when terminals are created, so you will need to restart your terminals for it to take effect.
	// 
	//  Note that the script injection may not work if you have custom arguments defined in the terminal profile, have enabled `editor.accessibilitySupport#`, have a [complex bash `PROMPT_COMMAND`](https://code.visualstudio.com/docs/editor/integrated-terminal#_complex-bash-promptcommand), or other unsupported setup. To disable decorations, see `#terminal.integrated.shellIntegration.decorationsEnabled`
	"terminal.integrated.shellIntegration.enabled": true,

	// Controls the number of recently used commands to keep in the terminal command history. Set to 0 to disable terminal command history.
	"terminal.integrated.shellIntegration.history": 100,

	// Whether to show the command guide when hovering over a command in the terminal.
	"terminal.integrated.shellIntegration.showCommandGuide": true,

	// Controls whether to show the alert "The terminal process terminated with exit code" when exit code is non-zero.
	"terminal.integrated.showExitAlert": true,

	// Whether to show hovers for links in the terminal output.
	"terminal.integrated.showLinkHover": true,

	// Controls whether the terminal will scroll using an animation.
	"terminal.integrated.smoothScrolling": false,

	// Controls the working directory a split terminal starts with.
	//  - workspaceRoot: A new split terminal will use the workspace root as the working directory. In a multi-root workspace a choice for which root folder to use is offered.
	//  - initial: A new split terminal will use the working directory that the parent terminal started with.
	//  - inherited: On macOS and Linux, a new split terminal will use the working directory of the parent terminal. On Windows, this behaves the same as initial.
	"terminal.integrated.splitCwd": "inherited",

	// Shows the current command at the top of the terminal. This feature requires [shell integration](https://code.visualstudio.com/docs/terminal/shell-integration) to be activated. See `terminal.integrated.shellIntegration.enabled`.
	"terminal.integrated.stickyScroll.enabled": false,

	// Defines the maximum number of sticky lines to show. Sticky scroll lines will never exceed 40% of the viewport regardless of this setting.
	"terminal.integrated.stickyScroll.maxLineCount": 5,

	// Controls which built-in completions are activated. This setting can cause conflicts if custom shell completions are configured in the shell profile.
	"terminal.integrated.suggest.builtinCompletions": {
		"pwshCode": true,
		"pwshGit": true
	},

	// Enables experimental terminal Intellisense suggestions for supported shells (PowerShell v7+, zsh, bash, fish) when `terminal.integrated.shellIntegration.enabled` is set to `true`.
	// 
	// If shell integration is installed manually, `VSCODE_SUGGEST` needs to be set to `1` before calling the shell integration script.
	"terminal.integrated.suggest.enabled": false,

	// Providers are enabled by default. Omit them by setting the id of the provider to `false`.
	"terminal.integrated.suggest.providers": {
		"terminal-suggest": true,
		"pwsh-shell-integration": false
	},

	// Controls whether suggestions should automatically show up while typing. Also be aware of the `terminal.integrated.suggest.suggestOnTriggerCharacters`-setting which controls if suggestions are triggered by special characters.
	"terminal.integrated.suggest.quickSuggestions": true,

	// Controls whether suggestions should run immediately when `Enter` (not `Tab`) is used to accept the result.
	//  - ignore: Ignore suggestions and send the enter directly to the shell without completing. This is used as the default value so the suggest widget is as unobtrusive as possible.
	//  - never: Never run on `Enter`.
	//  - exactMatch: Run on `Enter` when the suggestion is typed in its entirety.
	//  - exactMatchIgnoreExtension: Run on `Enter` when the suggestion is typed in its entirety or when a file is typed without its extension included.
	//  - always: Always run on `Enter`.
	"terminal.integrated.suggest.runOnEnter": "ignore",

	// Controls whether the terminal suggestions status bar should be shown.
	"terminal.integrated.suggest.showStatusBar": true,

	// Controls whether suggestions should automatically show up when typing trigger characters.
	"terminal.integrated.suggest.suggestOnTriggerCharacters": true,

	// A set of windows command executable extensions that will be included as suggestions in the terminal.
	// 
	// Many executables are included by default, listed below:
	// 
	// - bat
	// - cmd
	// - com
	// - exe
	// - jar
	// - js
	// - msi
	// - pl
	// - ps1
	// - py
	// - rb
	// - sh
	// - vbs.
	// 
	// To exclude an extension, set it to `false`
	// 
	// . To include one not in the list, add it and set it to `true`.
	"terminal.integrated.suggest.windowsExecutableExtensions": {},

	// A theme color ID to associate with terminal icons by default.
	"terminal.integrated.tabs.defaultColor": null,

	// A codicon ID to associate with terminal icons by default.
	//  - add: $(add)
	//  - plus: $(plus)
	//  - gist-new: $(gist-new)
	//  - repo-create: $(repo-create)
	//  - lightbulb: $(lightbulb)
	//  - light-bulb: $(light-bulb)
	//  - repo: $(repo)
	//  - repo-delete: $(repo-delete)
	//  - gist-fork: $(gist-fork)
	//  - repo-forked: $(repo-forked)
	//  - git-pull-request: $(git-pull-request)
	//  - git-pull-request-abandoned: $(git-pull-request-abandoned)
	//  - record-keys: $(record-keys)
	//  - keyboard: $(keyboard)
	//  - tag: $(tag)
	//  - git-pull-request-label: $(git-pull-request-label)
	//  - tag-add: $(tag-add)
	//  - tag-remove: $(tag-remove)
	//  - person: $(person)
	//  - person-follow: $(person-follow)
	//  - person-outline: $(person-outline)
	//  - person-filled: $(person-filled)
	//  - git-branch: $(git-branch)
	//  - git-branch-create: $(git-branch-create)
	//  - git-branch-delete: $(git-branch-delete)
	//  - source-control: $(source-control)
	//  - mirror: $(mirror)
	//  - mirror-public: $(mirror-public)
	//  - star: $(star)
	//  - star-add: $(star-add)
	//  - star-delete: $(star-delete)
	//  - star-empty: $(star-empty)
	//  - comment: $(comment)
	//  - comment-add: $(comment-add)
	//  - alert: $(alert)
	//  - warning: $(warning)
	//  - search: $(search)
	//  - search-save: $(search-save)
	//  - log-out: $(log-out)
	//  - sign-out: $(sign-out)
	//  - log-in: $(log-in)
	//  - sign-in: $(sign-in)
	//  - eye: $(eye)
	//  - eye-unwatch: $(eye-unwatch)
	//  - eye-watch: $(eye-watch)
	//  - circle-filled: $(circle-filled)
	//  - primitive-dot: $(primitive-dot)
	//  - close-dirty: $(close-dirty)
	//  - debug-breakpoint: $(debug-breakpoint)
	//  - debug-breakpoint-disabled: $(debug-breakpoint-disabled)
	//  - debug-hint: $(debug-hint)
	//  - terminal-decoration-success: $(terminal-decoration-success)
	//  - primitive-square: $(primitive-square)
	//  - edit: $(edit)
	//  - pencil: $(pencil)
	//  - info: $(info)
	//  - issue-opened: $(issue-opened)
	//  - gist-private: $(gist-private)
	//  - git-fork-private: $(git-fork-private)
	//  - lock: $(lock)
	//  - mirror-private: $(mirror-private)
	//  - close: $(close)
	//  - remove-close: $(remove-close)
	//  - x: $(x)
	//  - repo-sync: $(repo-sync)
	//  - sync: $(sync)
	//  - clone: $(clone)
	//  - desktop-download: $(desktop-download)
	//  - beaker: $(beaker)
	//  - microscope: $(microscope)
	//  - vm: $(vm)
	//  - device-desktop: $(device-desktop)
	//  - file: $(file)
	//  - file-text: $(file-text)
	//  - more: $(more)
	//  - ellipsis: $(ellipsis)
	//  - kebab-horizontal: $(kebab-horizontal)
	//  - mail-reply: $(mail-reply)
	//  - reply: $(reply)
	//  - organization: $(organization)
	//  - organization-filled: $(organization-filled)
	//  - organization-outline: $(organization-outline)
	//  - new-file: $(new-file)
	//  - file-add: $(file-add)
	//  - new-folder: $(new-folder)
	//  - file-directory-create: $(file-directory-create)
	//  - trash: $(trash)
	//  - trashcan: $(trashcan)
	//  - history: $(history)
	//  - clock: $(clock)
	//  - folder: $(folder)
	//  - file-directory: $(file-directory)
	//  - symbol-folder: $(symbol-folder)
	//  - logo-github: $(logo-github)
	//  - mark-github: $(mark-github)
	//  - github: $(github)
	//  - terminal: $(terminal)
	//  - console: $(console)
	//  - repl: $(repl)
	//  - zap: $(zap)
	//  - symbol-event: $(symbol-event)
	//  - error: $(error)
	//  - stop: $(stop)
	//  - variable: $(variable)
	//  - symbol-variable: $(symbol-variable)
	//  - array: $(array)
	//  - symbol-array: $(symbol-array)
	//  - symbol-module: $(symbol-module)
	//  - symbol-package: $(symbol-package)
	//  - symbol-namespace: $(symbol-namespace)
	//  - symbol-object: $(symbol-object)
	//  - symbol-method: $(symbol-method)
	//  - symbol-function: $(symbol-function)
	//  - symbol-constructor: $(symbol-constructor)
	//  - symbol-boolean: $(symbol-boolean)
	//  - symbol-null: $(symbol-null)
	//  - symbol-numeric: $(symbol-numeric)
	//  - symbol-number: $(symbol-number)
	//  - symbol-structure: $(symbol-structure)
	//  - symbol-struct: $(symbol-struct)
	//  - symbol-parameter: $(symbol-parameter)
	//  - symbol-type-parameter: $(symbol-type-parameter)
	//  - symbol-key: $(symbol-key)
	//  - symbol-text: $(symbol-text)
	//  - symbol-reference: $(symbol-reference)
	//  - go-to-file: $(go-to-file)
	//  - symbol-enum: $(symbol-enum)
	//  - symbol-value: $(symbol-value)
	//  - symbol-ruler: $(symbol-ruler)
	//  - symbol-unit: $(symbol-unit)
	//  - activate-breakpoints: $(activate-breakpoints)
	//  - archive: $(archive)
	//  - arrow-both: $(arrow-both)
	//  - arrow-down: $(arrow-down)
	//  - arrow-left: $(arrow-left)
	//  - arrow-right: $(arrow-right)
	//  - arrow-small-down: $(arrow-small-down)
	//  - arrow-small-left: $(arrow-small-left)
	//  - arrow-small-right: $(arrow-small-right)
	//  - arrow-small-up: $(arrow-small-up)
	//  - arrow-up: $(arrow-up)
	//  - bell: $(bell)
	//  - bold: $(bold)
	//  - book: $(book)
	//  - bookmark: $(bookmark)
	//  - debug-breakpoint-conditional-unverified: $(debug-breakpoint-conditional-unverified)
	//  - debug-breakpoint-conditional: $(debug-breakpoint-conditional)
	//  - debug-breakpoint-conditional-disabled: $(debug-breakpoint-conditional-disabled)
	//  - debug-breakpoint-data-unverified: $(debug-breakpoint-data-unverified)
	//  - debug-breakpoint-data: $(debug-breakpoint-data)
	//  - debug-breakpoint-data-disabled: $(debug-breakpoint-data-disabled)
	//  - debug-breakpoint-log-unverified: $(debug-breakpoint-log-unverified)
	//  - debug-breakpoint-log: $(debug-breakpoint-log)
	//  - debug-breakpoint-log-disabled: $(debug-breakpoint-log-disabled)
	//  - briefcase: $(briefcase)
	//  - broadcast: $(broadcast)
	//  - browser: $(browser)
	//  - bug: $(bug)
	//  - calendar: $(calendar)
	//  - case-sensitive: $(case-sensitive)
	//  - check: $(check)
	//  - checklist: $(checklist)
	//  - chevron-down: $(chevron-down)
	//  - chevron-left: $(chevron-left)
	//  - chevron-right: $(chevron-right)
	//  - chevron-up: $(chevron-up)
	//  - chrome-close: $(chrome-close)
	//  - chrome-maximize: $(chrome-maximize)
	//  - chrome-minimize: $(chrome-minimize)
	//  - chrome-restore: $(chrome-restore)
	//  - circle-outline: $(circle-outline)
	//  - circle: $(circle)
	//  - debug-breakpoint-unverified: $(debug-breakpoint-unverified)
	//  - terminal-decoration-incomplete: $(terminal-decoration-incomplete)
	//  - circle-slash: $(circle-slash)
	//  - circuit-board: $(circuit-board)
	//  - clear-all: $(clear-all)
	//  - clippy: $(clippy)
	//  - close-all: $(close-all)
	//  - cloud-download: $(cloud-download)
	//  - cloud-upload: $(cloud-upload)
	//  - code: $(code)
	//  - collapse-all: $(collapse-all)
	//  - color-mode: $(color-mode)
	//  - comment-discussion: $(comment-discussion)
	//  - credit-card: $(credit-card)
	//  - dash: $(dash)
	//  - dashboard: $(dashboard)
	//  - database: $(database)
	//  - debug-continue: $(debug-continue)
	//  - debug-disconnect: $(debug-disconnect)
	//  - debug-pause: $(debug-pause)
	//  - debug-restart: $(debug-restart)
	//  - debug-start: $(debug-start)
	//  - debug-step-into: $(debug-step-into)
	//  - debug-step-out: $(debug-step-out)
	//  - debug-step-over: $(debug-step-over)
	//  - debug-stop: $(debug-stop)
	//  - debug: $(debug)
	//  - device-camera-video: $(device-camera-video)
	//  - device-camera: $(device-camera)
	//  - device-mobile: $(device-mobile)
	//  - diff-added: $(diff-added)
	//  - diff-ignored: $(diff-ignored)
	//  - diff-modified: $(diff-modified)
	//  - diff-removed: $(diff-removed)
	//  - diff-renamed: $(diff-renamed)
	//  - diff: $(diff)
	//  - diff-sidebyside: $(diff-sidebyside)
	//  - discard: $(discard)
	//  - editor-layout: $(editor-layout)
	//  - empty-window: $(empty-window)
	//  - exclude: $(exclude)
	//  - extensions: $(extensions)
	//  - eye-closed: $(eye-closed)
	//  - file-binary: $(file-binary)
	//  - file-code: $(file-code)
	//  - file-media: $(file-media)
	//  - file-pdf: $(file-pdf)
	//  - file-submodule: $(file-submodule)
	//  - file-symlink-directory: $(file-symlink-directory)
	//  - file-symlink-file: $(file-symlink-file)
	//  - file-zip: $(file-zip)
	//  - files: $(files)
	//  - filter: $(filter)
	//  - flame: $(flame)
	//  - fold-down: $(fold-down)
	//  - fold-up: $(fold-up)
	//  - fold: $(fold)
	//  - folder-active: $(folder-active)
	//  - folder-opened: $(folder-opened)
	//  - gear: $(gear)
	//  - gift: $(gift)
	//  - gist-secret: $(gist-secret)
	//  - gist: $(gist)
	//  - git-commit: $(git-commit)
	//  - git-compare: $(git-compare)
	//  - compare-changes: $(compare-changes)
	//  - git-merge: $(git-merge)
	//  - github-action: $(github-action)
	//  - github-alt: $(github-alt)
	//  - globe: $(globe)
	//  - grabber: $(grabber)
	//  - graph: $(graph)
	//  - gripper: $(gripper)
	//  - heart: $(heart)
	//  - home: $(home)
	//  - horizontal-rule: $(horizontal-rule)
	//  - hubot: $(hubot)
	//  - inbox: $(inbox)
	//  - issue-reopened: $(issue-reopened)
	//  - issues: $(issues)
	//  - italic: $(italic)
	//  - jersey: $(jersey)
	//  - json: $(json)
	//  - kebab-vertical: $(kebab-vertical)
	//  - key: $(key)
	//  - law: $(law)
	//  - lightbulb-autofix: $(lightbulb-autofix)
	//  - link-external: $(link-external)
	//  - link: $(link)
	//  - list-ordered: $(list-ordered)
	//  - list-unordered: $(list-unordered)
	//  - live-share: $(live-share)
	//  - loading: $(loading)
	//  - location: $(location)
	//  - mail-read: $(mail-read)
	//  - mail: $(mail)
	//  - markdown: $(markdown)
	//  - megaphone: $(megaphone)
	//  - mention: $(mention)
	//  - milestone: $(milestone)
	//  - git-pull-request-milestone: $(git-pull-request-milestone)
	//  - mortar-board: $(mortar-board)
	//  - move: $(move)
	//  - multiple-windows: $(multiple-windows)
	//  - mute: $(mute)
	//  - no-newline: $(no-newline)
	//  - note: $(note)
	//  - octoface: $(octoface)
	//  - open-preview: $(open-preview)
	//  - package: $(package)
	//  - paintcan: $(paintcan)
	//  - pin: $(pin)
	//  - play: $(play)
	//  - run: $(run)
	//  - plug: $(plug)
	//  - preserve-case: $(preserve-case)
	//  - preview: $(preview)
	//  - project: $(project)
	//  - pulse: $(pulse)
	//  - question: $(question)
	//  - quote: $(quote)
	//  - radio-tower: $(radio-tower)
	//  - reactions: $(reactions)
	//  - references: $(references)
	//  - refresh: $(refresh)
	//  - regex: $(regex)
	//  - remote-explorer: $(remote-explorer)
	//  - remote: $(remote)
	//  - remove: $(remove)
	//  - replace-all: $(replace-all)
	//  - replace: $(replace)
	//  - repo-clone: $(repo-clone)
	//  - repo-force-push: $(repo-force-push)
	//  - repo-pull: $(repo-pull)
	//  - repo-push: $(repo-push)
	//  - report: $(report)
	//  - request-changes: $(request-changes)
	//  - rocket: $(rocket)
	//  - root-folder-opened: $(root-folder-opened)
	//  - root-folder: $(root-folder)
	//  - rss: $(rss)
	//  - ruby: $(ruby)
	//  - save-all: $(save-all)
	//  - save-as: $(save-as)
	//  - save: $(save)
	//  - screen-full: $(screen-full)
	//  - screen-normal: $(screen-normal)
	//  - search-stop: $(search-stop)
	//  - server: $(server)
	//  - settings-gear: $(settings-gear)
	//  - settings: $(settings)
	//  - shield: $(shield)
	//  - smiley: $(smiley)
	//  - sort-precedence: $(sort-precedence)
	//  - split-horizontal: $(split-horizontal)
	//  - split-vertical: $(split-vertical)
	//  - squirrel: $(squirrel)
	//  - star-full: $(star-full)
	//  - star-half: $(star-half)
	//  - symbol-class: $(symbol-class)
	//  - symbol-color: $(symbol-color)
	//  - symbol-constant: $(symbol-constant)
	//  - symbol-enum-member: $(symbol-enum-member)
	//  - symbol-field: $(symbol-field)
	//  - symbol-file: $(symbol-file)
	//  - symbol-interface: $(symbol-interface)
	//  - symbol-keyword: $(symbol-keyword)
	//  - symbol-misc: $(symbol-misc)
	//  - symbol-operator: $(symbol-operator)
	//  - symbol-property: $(symbol-property)
	//  - wrench: $(wrench)
	//  - wrench-subaction: $(wrench-subaction)
	//  - symbol-snippet: $(symbol-snippet)
	//  - tasklist: $(tasklist)
	//  - telescope: $(telescope)
	//  - text-size: $(text-size)
	//  - three-bars: $(three-bars)
	//  - thumbsdown: $(thumbsdown)
	//  - thumbsup: $(thumbsup)
	//  - tools: $(tools)
	//  - triangle-down: $(triangle-down)
	//  - triangle-left: $(triangle-left)
	//  - triangle-right: $(triangle-right)
	//  - triangle-up: $(triangle-up)
	//  - twitter: $(twitter)
	//  - unfold: $(unfold)
	//  - unlock: $(unlock)
	//  - unmute: $(unmute)
	//  - unverified: $(unverified)
	//  - verified: $(verified)
	//  - versions: $(versions)
	//  - vm-active: $(vm-active)
	//  - vm-outline: $(vm-outline)
	//  - vm-running: $(vm-running)
	//  - watch: $(watch)
	//  - whitespace: $(whitespace)
	//  - whole-word: $(whole-word)
	//  - window: $(window)
	//  - word-wrap: $(word-wrap)
	//  - zoom-in: $(zoom-in)
	//  - zoom-out: $(zoom-out)
	//  - list-filter: $(list-filter)
	//  - list-flat: $(list-flat)
	//  - list-selection: $(list-selection)
	//  - selection: $(selection)
	//  - list-tree: $(list-tree)
	//  - debug-breakpoint-function-unverified: $(debug-breakpoint-function-unverified)
	//  - debug-breakpoint-function: $(debug-breakpoint-function)
	//  - debug-breakpoint-function-disabled: $(debug-breakpoint-function-disabled)
	//  - debug-stackframe-active: $(debug-stackframe-active)
	//  - circle-small-filled: $(circle-small-filled)
	//  - debug-stackframe-dot: $(debug-stackframe-dot)
	//  - terminal-decoration-mark: $(terminal-decoration-mark)
	//  - debug-stackframe: $(debug-stackframe)
	//  - debug-stackframe-focused: $(debug-stackframe-focused)
	//  - debug-breakpoint-unsupported: $(debug-breakpoint-unsupported)
	//  - symbol-string: $(symbol-string)
	//  - debug-reverse-continue: $(debug-reverse-continue)
	//  - debug-step-back: $(debug-step-back)
	//  - debug-restart-frame: $(debug-restart-frame)
	//  - debug-alt: $(debug-alt)
	//  - call-incoming: $(call-incoming)
	//  - call-outgoing: $(call-outgoing)
	//  - menu: $(menu)
	//  - expand-all: $(expand-all)
	//  - feedback: $(feedback)
	//  - git-pull-request-reviewer: $(git-pull-request-reviewer)
	//  - group-by-ref-type: $(group-by-ref-type)
	//  - ungroup-by-ref-type: $(ungroup-by-ref-type)
	//  - account: $(account)
	//  - git-pull-request-assignee: $(git-pull-request-assignee)
	//  - bell-dot: $(bell-dot)
	//  - debug-console: $(debug-console)
	//  - library: $(library)
	//  - output: $(output)
	//  - run-all: $(run-all)
	//  - sync-ignored: $(sync-ignored)
	//  - pinned: $(pinned)
	//  - github-inverted: $(github-inverted)
	//  - server-process: $(server-process)
	//  - server-environment: $(server-environment)
	//  - pass: $(pass)
	//  - issue-closed: $(issue-closed)
	//  - stop-circle: $(stop-circle)
	//  - play-circle: $(play-circle)
	//  - record: $(record)
	//  - debug-alt-small: $(debug-alt-small)
	//  - vm-connect: $(vm-connect)
	//  - cloud: $(cloud)
	//  - merge: $(merge)
	//  - export: $(export)
	//  - graph-left: $(graph-left)
	//  - magnet: $(magnet)
	//  - notebook: $(notebook)
	//  - redo: $(redo)
	//  - check-all: $(check-all)
	//  - pinned-dirty: $(pinned-dirty)
	//  - pass-filled: $(pass-filled)
	//  - circle-large-filled: $(circle-large-filled)
	//  - circle-large: $(circle-large)
	//  - circle-large-outline: $(circle-large-outline)
	//  - combine: $(combine)
	//  - gather: $(gather)
	//  - table: $(table)
	//  - variable-group: $(variable-group)
	//  - type-hierarchy: $(type-hierarchy)
	//  - type-hierarchy-sub: $(type-hierarchy-sub)
	//  - type-hierarchy-super: $(type-hierarchy-super)
	//  - git-pull-request-create: $(git-pull-request-create)
	//  - run-above: $(run-above)
	//  - run-below: $(run-below)
	//  - notebook-template: $(notebook-template)
	//  - debug-rerun: $(debug-rerun)
	//  - workspace-trusted: $(workspace-trusted)
	//  - workspace-untrusted: $(workspace-untrusted)
	//  - workspace-unknown: $(workspace-unknown)
	//  - terminal-cmd: $(terminal-cmd)
	//  - terminal-debian: $(terminal-debian)
	//  - terminal-linux: $(terminal-linux)
	//  - terminal-powershell: $(terminal-powershell)
	//  - terminal-tmux: $(terminal-tmux)
	//  - terminal-ubuntu: $(terminal-ubuntu)
	//  - terminal-bash: $(terminal-bash)
	//  - arrow-swap: $(arrow-swap)
	//  - copy: $(copy)
	//  - person-add: $(person-add)
	//  - filter-filled: $(filter-filled)
	//  - wand: $(wand)
	//  - debug-line-by-line: $(debug-line-by-line)
	//  - inspect: $(inspect)
	//  - layers: $(layers)
	//  - layers-dot: $(layers-dot)
	//  - layers-active: $(layers-active)
	//  - compass: $(compass)
	//  - compass-dot: $(compass-dot)
	//  - compass-active: $(compass-active)
	//  - azure: $(azure)
	//  - issue-draft: $(issue-draft)
	//  - git-pull-request-closed: $(git-pull-request-closed)
	//  - git-pull-request-draft: $(git-pull-request-draft)
	//  - debug-all: $(debug-all)
	//  - debug-coverage: $(debug-coverage)
	//  - run-errors: $(run-errors)
	//  - folder-library: $(folder-library)
	//  - debug-continue-small: $(debug-continue-small)
	//  - beaker-stop: $(beaker-stop)
	//  - graph-line: $(graph-line)
	//  - graph-scatter: $(graph-scatter)
	//  - pie-chart: $(pie-chart)
	//  - bracket: $(bracket)
	//  - bracket-dot: $(bracket-dot)
	//  - bracket-error: $(bracket-error)
	//  - lock-small: $(lock-small)
	//  - azure-devops: $(azure-devops)
	//  - verified-filled: $(verified-filled)
	//  - newline: $(newline)
	//  - layout: $(layout)
	//  - layout-activitybar-left: $(layout-activitybar-left)
	//  - layout-activitybar-right: $(layout-activitybar-right)
	//  - layout-panel-left: $(layout-panel-left)
	//  - layout-panel-center: $(layout-panel-center)
	//  - layout-panel-justify: $(layout-panel-justify)
	//  - layout-panel-right: $(layout-panel-right)
	//  - layout-panel: $(layout-panel)
	//  - layout-sidebar-left: $(layout-sidebar-left)
	//  - layout-sidebar-right: $(layout-sidebar-right)
	//  - layout-statusbar: $(layout-statusbar)
	//  - layout-menubar: $(layout-menubar)
	//  - layout-centered: $(layout-centered)
	//  - target: $(target)
	//  - indent: $(indent)
	//  - record-small: $(record-small)
	//  - error-small: $(error-small)
	//  - terminal-decoration-error: $(terminal-decoration-error)
	//  - arrow-circle-down: $(arrow-circle-down)
	//  - arrow-circle-left: $(arrow-circle-left)
	//  - arrow-circle-right: $(arrow-circle-right)
	//  - arrow-circle-up: $(arrow-circle-up)
	//  - layout-sidebar-right-off: $(layout-sidebar-right-off)
	//  - layout-panel-off: $(layout-panel-off)
	//  - layout-sidebar-left-off: $(layout-sidebar-left-off)
	//  - blank: $(blank)
	//  - heart-filled: $(heart-filled)
	//  - map: $(map)
	//  - map-horizontal: $(map-horizontal)
	//  - fold-horizontal: $(fold-horizontal)
	//  - map-filled: $(map-filled)
	//  - map-horizontal-filled: $(map-horizontal-filled)
	//  - fold-horizontal-filled: $(fold-horizontal-filled)
	//  - circle-small: $(circle-small)
	//  - bell-slash: $(bell-slash)
	//  - bell-slash-dot: $(bell-slash-dot)
	//  - comment-unresolved: $(comment-unresolved)
	//  - git-pull-request-go-to-changes: $(git-pull-request-go-to-changes)
	//  - git-pull-request-new-changes: $(git-pull-request-new-changes)
	//  - search-fuzzy: $(search-fuzzy)
	//  - comment-draft: $(comment-draft)
	//  - send: $(send)
	//  - sparkle: $(sparkle)
	//  - insert: $(insert)
	//  - mic: $(mic)
	//  - thumbsdown-filled: $(thumbsdown-filled)
	//  - thumbsup-filled: $(thumbsup-filled)
	//  - coffee: $(coffee)
	//  - snake: $(snake)
	//  - game: $(game)
	//  - vr: $(vr)
	//  - chip: $(chip)
	//  - piano: $(piano)
	//  - music: $(music)
	//  - mic-filled: $(mic-filled)
	//  - repo-fetch: $(repo-fetch)
	//  - copilot: $(copilot)
	//  - lightbulb-sparkle: $(lightbulb-sparkle)
	//  - robot: $(robot)
	//  - sparkle-filled: $(sparkle-filled)
	//  - diff-single: $(diff-single)
	//  - diff-multiple: $(diff-multiple)
	//  - surround-with: $(surround-with)
	//  - share: $(share)
	//  - git-stash: $(git-stash)
	//  - git-stash-apply: $(git-stash-apply)
	//  - git-stash-pop: $(git-stash-pop)
	//  - vscode: $(vscode)
	//  - vscode-insiders: $(vscode-insiders)
	//  - code-oss: $(code-oss)
	//  - run-coverage: $(run-coverage)
	//  - run-all-coverage: $(run-all-coverage)
	//  - coverage: $(coverage)
	//  - github-project: $(github-project)
	//  - map-vertical: $(map-vertical)
	//  - fold-vertical: $(fold-vertical)
	//  - map-vertical-filled: $(map-vertical-filled)
	//  - fold-vertical-filled: $(fold-vertical-filled)
	//  - go-to-search: $(go-to-search)
	//  - percentage: $(percentage)
	//  - sort-percentage: $(sort-percentage)
	//  - attach: $(attach)
	//  - go-to-editing-session: $(go-to-editing-session)
	//  - edit-session: $(edit-session)
	//  - code-review: $(code-review)
	//  - copilot-warning: $(copilot-warning)
	//  - python: $(python)
	//  - copilot-large: $(copilot-large)
	//  - copilot-warning-large: $(copilot-warning-large)
	//  - keyboard-tab: $(keyboard-tab)
	//  - dialog-error: $(dialog-error)
	//  - dialog-warning: $(dialog-warning)
	//  - dialog-info: $(dialog-info)
	//  - dialog-close: $(dialog-close)
	//  - tree-item-expanded: $(tree-item-expanded)
	//  - tree-filter-on-type-on: $(tree-filter-on-type-on)
	//  - tree-filter-on-type-off: $(tree-filter-on-type-off)
	//  - tree-filter-clear: $(tree-filter-clear)
	//  - tree-item-loading: $(tree-item-loading)
	//  - menu-selection: $(menu-selection)
	//  - menu-submenu: $(menu-submenu)
	//  - menubar-more: $(menubar-more)
	//  - scrollbar-button-left: $(scrollbar-button-left)
	//  - scrollbar-button-right: $(scrollbar-button-right)
	//  - scrollbar-button-up: $(scrollbar-button-up)
	//  - scrollbar-button-down: $(scrollbar-button-down)
	//  - toolbar-more: $(toolbar-more)
	//  - quick-input-back: $(quick-input-back)
	//  - drop-down-button: $(drop-down-button)
	//  - symbol-customcolor: $(symbol-customcolor)
	//  - export: $(export)
	//  - workspace-unspecified: $(workspace-unspecified)
	//  - newline: $(newline)
	//  - thumbsdown-filled: $(thumbsdown-filled)
	//  - thumbsup-filled: $(thumbsup-filled)
	//  - git-fetch: $(git-fetch)
	//  - lightbulb-sparkle-autofix: $(lightbulb-sparkle-autofix)
	//  - debug-breakpoint-pending: $(debug-breakpoint-pending)
	"terminal.integrated.tabs.defaultIcon": "terminal",

	// Controls the terminal description, which appears to the right of the title. Variables are substituted based on the context:
	// - `${cwd}`: the terminal's current working directory
	// - `${cwdFolder}`: the terminal's current working directory, displayed for multi-root workspaces or in a single root workspace when the value differs from the initial working directory. On Windows, this will only be displayed when shell integration is enabled.
	// - `${workspaceFolder}`: the workspace in which the terminal was launched
	// - `${workspaceFolderName}`: the `name` of the workspace in which the terminal was launched
	// - `${local}`: indicates a local terminal in a remote workspace
	// - `${process}`: the name of the terminal process
	// - `${progress}`: the progress state as reported by the `OSC 9;4` sequence
	// - `${separator}`: a conditional separator (` - `) that only shows when surrounded by variables with values or static text.
	// - `${sequence}`: the name provided to the terminal by the process
	// - `${task}`: indicates this terminal is associated with a task
	// - `${shellType}`: the detected shell type
	// - `${shellCommand}`: the command being executed according to shell integration. This also requires high confidence in the detected command line which may not work in some prompt frameworks.
	// - `${shellPromptInput}`: the shell's full prompt input according to shell integration
	"terminal.integrated.tabs.description": "${task}${separator}${local}${separator}${cwdFolder}",

	// Controls whether terminal tab statuses support animation (eg. in progress tasks).
	"terminal.integrated.tabs.enableAnimation": true,

	// Controls whether terminal tabs display as a list to the side of the terminal. When this is disabled a dropdown will display instead.
	"terminal.integrated.tabs.enabled": true,

	// Controls whether focusing the terminal of a tab happens on double or single click.
	//  - singleClick: Focus the terminal when clicking a terminal tab
	//  - doubleClick: Focus the terminal when double-clicking a terminal tab
	"terminal.integrated.tabs.focusMode": "doubleClick",

	// Controls whether the terminal tabs view will hide under certain conditions.
	//  - never: Never hide the terminal tabs view
	//  - singleTerminal: Hide the terminal tabs view when there is only a single terminal opened
	//  - singleGroup: Hide the terminal tabs view when there is only a single terminal group opened
	"terminal.integrated.tabs.hideCondition": "singleTerminal",

	// Controls the location of the terminal tabs, either to the left or right of the actual terminal(s).
	//  - left: Show the terminal tabs view to the left of the terminal
	//  - right: Show the terminal tabs view to the right of the terminal
	"terminal.integrated.tabs.location": "right",

	// Separator used by `terminal.integrated.tabs.title#` and `#terminal.integrated.tabs.description`.
	"terminal.integrated.tabs.separator": " - ",

	// Controls whether terminal split and kill buttons are displays next to the new terminal button.
	//  - always: Always show the actions
	//  - singleTerminal: Show the actions when it is the only terminal opened
	//  - singleTerminalOrNarrow: Show the actions when it is the only terminal opened or when the tabs view is in its narrow textless state
	//  - never: Never show the actions
	"terminal.integrated.tabs.showActions": "singleTerminalOrNarrow",

	// Shows the active terminal information in the view. This is particularly useful when the title within the tabs aren't visible.
	//  - always: Always show the active terminal
	//  - singleTerminal: Show the active terminal when it is the only terminal opened
	//  - singleTerminalOrNarrow: Show the active terminal when it is the only terminal opened or when the tabs view is in its narrow textless state
	//  - never: Never show the active terminal
	"terminal.integrated.tabs.showActiveTerminal": "singleTerminalOrNarrow",

	// Controls the terminal title. Variables are substituted based on the context:
	// - `${cwd}`: the terminal's current working directory
	// - `${cwdFolder}`: the terminal's current working directory, displayed for multi-root workspaces or in a single root workspace when the value differs from the initial working directory. On Windows, this will only be displayed when shell integration is enabled.
	// - `${workspaceFolder}`: the workspace in which the terminal was launched
	// - `${workspaceFolderName}`: the `name` of the workspace in which the terminal was launched
	// - `${local}`: indicates a local terminal in a remote workspace
	// - `${process}`: the name of the terminal process
	// - `${progress}`: the progress state as reported by the `OSC 9;4` sequence
	// - `${separator}`: a conditional separator (` - `) that only shows when surrounded by variables with values or static text.
	// - `${sequence}`: the name provided to the terminal by the process
	// - `${task}`: indicates this terminal is associated with a task
	// - `${shellType}`: the detected shell type
	// - `${shellCommand}`: the command being executed according to shell integration. This also requires high confidence in the detected command line which may not work in some prompt frameworks.
	// - `${shellPromptInput}`: the shell's full prompt input according to shell integration
	"terminal.integrated.tabs.title": "${process}",

	// The number of cells in a tab stop.
	"terminal.integrated.tabStopWidth": 8,

	// Controls what version of Unicode to use when evaluating the width of characters in the terminal. If you experience emoji or other wide characters not taking up the right amount of space or backspace either deleting too much or too little then you may want to try tweaking this setting.
	//  - 6: Version 6 of Unicode. This is an older version which should work better on older systems.
	//  - 11: Version 11 of Unicode. This version provides better support on modern systems that use modern versions of Unicode.
	"terminal.integrated.unicodeVersion": "11",

	// Controls whether or not WSL distros are shown in the terminal dropdown
	"terminal.integrated.useWslProfiles": true,

	// Whether to use ConPTY for Windows terminal process communication (requires Windows 10 build number 18309+). Winpty will be used if this is false.
	"terminal.integrated.windowsEnableConpty": true,

	// A string containing all characters to be considered word separators when double-clicking to select word and in the fallback 'word' link detection. Since this is used for link detection, including characters such as `:` that are used when detecting links will cause the line and column part of links like `file:10:5` to be ignored.
	"terminal.integrated.wordSeparators": " ()[]{}',\"`─‘’“”|",

	// Enable automatic tasks - note that tasks won't run in an untrusted workspace.
	//  - on: Always
	//  - off: Never
	"task.allowAutomaticTasks": "on",

	// Controls enablement of `provideTasks` for all task provider extension. If the Tasks: Run Task command is slow, disabling auto detect for task providers may help. Individual extensions may also provide settings that disable auto detection.
	"task.autoDetect": "on",

	// Configures whether to show the problem matcher prompt when running a task. Set to `true` to never prompt, or use a dictionary of task types to turn off prompting only for specific task types.
	"task.problemMatchers.neverPrompt": false,

	// Controls whether to show the task detail for tasks that have a detail in task quick picks, such as Run Task.
	"task.quickOpen.detail": true,

	// Controls the number of recent items tracked in task quick open dialog.
	"task.quickOpen.history": 30,

	// Causes the Tasks: Run Task command to use the slower "show all" behavior instead of the faster two level picker where tasks are grouped by provider.
	"task.quickOpen.showAll": false,

	// Controls whether the task quick pick is skipped when there is only one task to pick from.
	"task.quickOpen.skip": false,

	// On window reload, reconnect to tasks that have problem matchers.
	"task.reconnection": true,

	// Save all dirty editors before running a task.
	//  - always: Always saves all editors before running.
	//  - never: Never saves editors before running.
	//  - prompt: Prompts whether to save editors before running.
	"task.saveBeforeRun": "always",

	// Configures whether a warning is shown when a provider is slow
	"task.slowProviderWarning": true,

	// Enable verbose logging for tasks.
	"task.verboseLogging": false,

	// Controls whether Problems view should automatically reveal files when opening them.
	"problems.autoReveal": true,

	// Show Errors & Warnings on files and folder. Overwritten by `problems.visibility` when it is off.
	"problems.decorations.enabled": true,

	// Controls the default view mode of the Problems view.
	"problems.defaultViewMode": "tree",

	// When enabled shows the current problem in the status bar.
	"problems.showCurrentInStatus": false,

	// Controls the order in which problems are navigated.
	//  - severity: Navigate problems ordered by severity
	//  - position: Navigate problems ordered by position
	"problems.sortOrder": "severity",

	// Controls whether the problems are visible throughout the editor and workbench.
	"problems.visibility": true,

	// Enable/disable navigation breadcrumbs.
	"breadcrumbs.enabled": true,

	// Controls whether and how file paths are shown in the breadcrumbs view.
	//  - on: Show the file path in the breadcrumbs view.
	//  - off: Do not show the file path in the breadcrumbs view.
	//  - last: Only show the last element of the file path in the breadcrumbs view.
	"breadcrumbs.filePath": "on",

	// Render breadcrumb items with icons.
	"breadcrumbs.icons": true,

	// When enabled breadcrumbs show `array`-symbols.
	"breadcrumbs.showArrays": true,

	// When enabled breadcrumbs show `boolean`-symbols.
	"breadcrumbs.showBooleans": true,

	// When enabled breadcrumbs show `class`-symbols.
	"breadcrumbs.showClasses": true,

	// When enabled breadcrumbs show `constant`-symbols.
	"breadcrumbs.showConstants": true,

	// When enabled breadcrumbs show `constructor`-symbols.
	"breadcrumbs.showConstructors": true,

	// When enabled breadcrumbs show `enumMember`-symbols.
	"breadcrumbs.showEnumMembers": true,

	// When enabled breadcrumbs show `enum`-symbols.
	"breadcrumbs.showEnums": true,

	// When enabled breadcrumbs show `event`-symbols.
	"breadcrumbs.showEvents": true,

	// When enabled breadcrumbs show `field`-symbols.
	"breadcrumbs.showFields": true,

	// When enabled breadcrumbs show `file`-symbols.
	"breadcrumbs.showFiles": true,

	// When enabled breadcrumbs show `function`-symbols.
	"breadcrumbs.showFunctions": true,

	// When enabled breadcrumbs show `interface`-symbols.
	"breadcrumbs.showInterfaces": true,

	// When enabled breadcrumbs show `key`-symbols.
	"breadcrumbs.showKeys": true,

	// When enabled breadcrumbs show `method`-symbols.
	"breadcrumbs.showMethods": true,

	// When enabled breadcrumbs show `module`-symbols.
	"breadcrumbs.showModules": true,

	// When enabled breadcrumbs show `namespace`-symbols.
	"breadcrumbs.showNamespaces": true,

	// When enabled breadcrumbs show `null`-symbols.
	"breadcrumbs.showNull": true,

	// When enabled breadcrumbs show `number`-symbols.
	"breadcrumbs.showNumbers": true,

	// When enabled breadcrumbs show `object`-symbols.
	"breadcrumbs.showObjects": true,

	// When enabled breadcrumbs show `operator`-symbols.
	"breadcrumbs.showOperators": true,

	// When enabled breadcrumbs show `package`-symbols.
	"breadcrumbs.showPackages": true,

	// When enabled breadcrumbs show `property`-symbols.
	"breadcrumbs.showProperties": true,

	// When enabled breadcrumbs show `string`-symbols.
	"breadcrumbs.showStrings": true,

	// When enabled breadcrumbs show `struct`-symbols.
	"breadcrumbs.showStructs": true,

	// When enabled breadcrumbs show `typeParameter`-symbols.
	"breadcrumbs.showTypeParameters": true,

	// When enabled breadcrumbs show `variable`-symbols.
	"breadcrumbs.showVariables": true,

	// Controls whether and how symbols are shown in the breadcrumbs view.
	//  - on: Show all symbols in the breadcrumbs view.
	//  - off: Do not show symbols in the breadcrumbs view.
	//  - last: Only show the current symbol in the breadcrumbs view.
	"breadcrumbs.symbolPath": "on",

	// Controls how symbols are sorted in the breadcrumbs outline view.
	//  - position: Show symbol outline in file position order.
	//  - name: Show symbol outline in alphabetical order.
	//  - type: Show symbol outline in symbol type order.
	"breadcrumbs.symbolSortOrder": "position",

	// Controls whether Outline items are collapsed or expanded.
	//  - alwaysCollapse: Collapse all items.
	//  - alwaysExpand: Expand all items.
	"outline.collapseItems": "alwaysExpand",

	// Render Outline elements with icons.
	"outline.icons": true,

	// Use badges for errors and warnings on Outline elements. Overwritten by `problems.visibility` when it is off.
	"outline.problems.badges": true,

	// Use colors for errors and warnings on Outline elements. Overwritten by `problems.visibility` when it is off.
	"outline.problems.colors": true,

	// Show errors and warnings on Outline elements. Overwritten by `problems.visibility` when it is off.
	"outline.problems.enabled": true,

	// When enabled, Outline shows `array`-symbols.
	"outline.showArrays": true,

	// When enabled, Outline shows `boolean`-symbols.
	"outline.showBooleans": true,

	// When enabled, Outline shows `class`-symbols.
	"outline.showClasses": true,

	// When enabled, Outline shows `constant`-symbols.
	"outline.showConstants": true,

	// When enabled, Outline shows `constructor`-symbols.
	"outline.showConstructors": true,

	// When enabled, Outline shows `enumMember`-symbols.
	"outline.showEnumMembers": true,

	// When enabled, Outline shows `enum`-symbols.
	"outline.showEnums": true,

	// When enabled, Outline shows `event`-symbols.
	"outline.showEvents": true,

	// When enabled, Outline shows `field`-symbols.
	"outline.showFields": true,

	// When enabled, Outline shows `file`-symbols.
	"outline.showFiles": true,

	// When enabled, Outline shows `function`-symbols.
	"outline.showFunctions": true,

	// When enabled, Outline shows `interface`-symbols.
	"outline.showInterfaces": true,

	// When enabled, Outline shows `key`-symbols.
	"outline.showKeys": true,

	// When enabled, Outline shows `method`-symbols.
	"outline.showMethods": true,

	// When enabled, Outline shows `module`-symbols.
	"outline.showModules": true,

	// When enabled, Outline shows `namespace`-symbols.
	"outline.showNamespaces": true,

	// When enabled, Outline shows `null`-symbols.
	"outline.showNull": true,

	// When enabled, Outline shows `number`-symbols.
	"outline.showNumbers": true,

	// When enabled, Outline shows `object`-symbols.
	"outline.showObjects": true,

	// When enabled, Outline shows `operator`-symbols.
	"outline.showOperators": true,

	// When enabled, Outline shows `package`-symbols.
	"outline.showPackages": true,

	// When enabled, Outline shows `property`-symbols.
	"outline.showProperties": true,

	// When enabled, Outline shows `string`-symbols.
	"outline.showStrings": true,

	// When enabled, Outline shows `struct`-symbols.
	"outline.showStructs": true,

	// When enabled, Outline shows `typeParameter`-symbols.
	"outline.showTypeParameters": true,

	// When enabled, Outline shows `variable`-symbols.
	"outline.showVariables": true,

	// Controls whether the Timeline view will load the next page of items when you scroll to the end of the list.
	"timeline.pageOnScroll": true,

	// The number of items to show in the Timeline view by default and when loading more items. Setting to `null` will automatically choose a page size based on the visible area of the Timeline view.
	"timeline.pageSize": 50,

	// Configure settings to be overridden for the clojure language.
	"[clojure]":  {
		"diffEditor.ignoreTrimWhitespace": false
	},

	// Configure settings to be overridden for the coffeescript language.
	"[coffeescript]":  {
		"diffEditor.ignoreTrimWhitespace": false,
		"editor.defaultColorDecorators": false
	},

	// Configure settings to be overridden for the csharp language.
	"[csharp]":  {
		"editor.maxTokenizationLineLength": 2500
	},

	// Configure settings to be overridden for the css language.
	"[css]":  {
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the dockercompose language.
	"[dockercompose]":  {
		"editor.insertSpaces": true,
		"editor.tabSize": 2,
		"editor.autoIndent": "advanced"
	},

	// Configure settings to be overridden for the dockerfile language.
	"[dockerfile]":  {
		"editor.quickSuggestions": {
				"strings": true
		}
	},

	// Configure settings to be overridden for the fsharp language.
	"[fsharp]":  {
		"diffEditor.ignoreTrimWhitespace": false
	},

	// Configure settings to be overridden for the git-commit language.
	"[git-commit]":  {
		"editor.rulers": [
				50,
				72
		],
		"editor.wordWrap": "off",
		"workbench.editor.restoreViewState": false
	},

	// Configure settings to be overridden for the git-rebase language.
	"[git-rebase]":  {
		"workbench.editor.restoreViewState": false
	},

	// Configure settings to be overridden for the go language.
	"[go]":  {
		"editor.insertSpaces": false
	},

	// Configure settings to be overridden for the handlebars language.
	"[handlebars]":  {
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the html language.
	"[html]":  {
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the jade language.
	"[jade]":  {
		"diffEditor.ignoreTrimWhitespace": false
	},

	// Configure settings to be overridden for the javascript language.
	"[javascript]":  {
		"editor.maxTokenizationLineLength": 2500
	},

	// Configure settings to be overridden for the json language.
	"[json]":  {
		"editor.quickSuggestions": {
				"strings": true
		},
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the jsonc language.
	"[jsonc]":  {
		"editor.quickSuggestions": {
				"strings": true
		},
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the julia language.
	"[julia]":  {
		"editor.defaultColorDecorators": false
	},

	// Configure settings to be overridden for the less language.
	"[less]":  {
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the makefile language.
	"[makefile]":  {
		"editor.insertSpaces": false
	},

	// Configure settings to be overridden for the markdown language.
	"[markdown]":  {
		"editor.unicodeHighlight.ambiguousCharacters": false,
		"editor.unicodeHighlight.invisibleCharacters": false,
		"diffEditor.ignoreTrimWhitespace": false,
		"editor.wordWrap": "on",
		"editor.quickSuggestions": {
				"comments": "off",
				"strings": "off",
				"other": "off"
		}
	},

	// Configure settings to be overridden for the plaintext language.
	"[plaintext]":  {
		"editor.unicodeHighlight.ambiguousCharacters": false,
		"editor.unicodeHighlight.invisibleCharacters": false
	},

	// Configure settings to be overridden for the python language.
	"[python]":  {
		"diffEditor.ignoreTrimWhitespace": false,
		"editor.defaultColorDecorators": false,
		"editor.formatOnType": true,
		"editor.wordBasedSuggestions": "off"
	},

	// Configure settings to be overridden for the ruby language.
	"[ruby]":  {
		"editor.defaultColorDecorators": false
	},

	// Configure settings to be overridden for the scss language.
	"[scss]":  {
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the search-result language.
	"[search-result]":  {
		"editor.lineNumbers": "off"
	},

	// Configure settings to be overridden for the shellscript language.
	"[shellscript]":  {
		"files.eol": "\n",
		"editor.defaultColorDecorators": false
	},

	// Configure settings to be overridden for the snippets language.
	"[snippets]":  {
		"editor.quickSuggestions": {
				"strings": true
		},
		"editor.suggest.insertMode": "replace"
	},

	// Configure settings to be overridden for the yaml language.
	"[yaml]":  {
		"editor.insertSpaces": true,
		"editor.tabSize": 2,
		"editor.autoIndent": "advanced",
		"diffEditor.ignoreTrimWhitespace": false,
		"editor.defaultColorDecorators": false
	},

	// The maximum number of requests to allow Copilot Edits to use in agent mode.
	"chat.agent.maxRequests": 5,

	// Controls whether the command center shows a menu for actions to control Copilot (requires `window.commandCenter`).
	"chat.commandCenter.enabled": true,

	// Enables chat participant autodetection for panel chat.
	"chat.detectParticipant.enabled": true,

	// Delay after which changes made by chat are automatically accepted. Values are in seconds, `0` means disabled and `100` seconds is the maximum.
	"chat.editing.autoAcceptDelay": 0,

	// Whether to show a confirmation before removing a request and its associated edits.
	"chat.editing.confirmEditRequestRemoval": true,

	// Whether to show a confirmation before retrying a request and its associated edits.
	"chat.editing.confirmEditRequestRetry": true,

	// Controls the font family in chat codeblocks.
	"chat.editor.fontFamily": "default",

	// Controls the font size in pixels in chat codeblocks.
	"chat.editor.fontSize": 14,

	// Controls the font weight in chat codeblocks.
	"chat.editor.fontWeight": "default",

	// Controls the line height in pixels in chat codeblocks. Use 0 to compute the line height from the font size.
	"chat.editor.lineHeight": 0,

	// Controls whether lines should wrap in chat codeblocks.
	"chat.editor.wordWrap": "off",

	// This setting is deprecated. Please use `chat.detectParticipant.enabled` instead.
	// Enables chat participant autodetection for panel chat.
	"chat.experimental.detectParticipant.enabled": null,

	// Enable support for attaching reusable prompt files (`*.prompt.md`) for Chat, Edits, and Inline Chat sessions. [Learn More](https://aka.ms/vscode-ghcp-prompt-snippets).
	"chat.promptFiles": null,

	// 
	//  - legacy: Uses the legacy diffing algorithm.
	//  - advanced: Uses the advanced diffing algorithm.
	"mergeEditor.diffAlgorithm": "advanced",

	// Controls if deletions in base or one of the inputs should be indicated by a vertical bar.
	"mergeEditor.showDeletionMarkers": true,

	// Enable experimental multi diff editor.
	"multiDiffEditor.experimental.enabled": true,

	// When enabled, new running processes are detected and ports that they listen on are automatically forwarded. Disabling this setting will not prevent all ports from being forwarded. Even when disabled, extensions will still be able to cause ports to be forwarded, and opening some URLs will still cause ports to forwarded. Also see `remote.autoForwardPortsSource`.
	"remote.autoForwardPorts": true,

	// The number of auto forwarded ports that will trigger the switch from `process` to `hybrid` when automatically forwarding ports and `remote.autoForwardPortsSource` is set to `process` by default. Set to `0` to disable the fallback. When `remote.autoForwardPortsFallback` hasn't been configured, but `remote.autoForwardPortsSource` has, `remote.autoForwardPortsFallback` will be treated as though it's set to `0`.
	"remote.autoForwardPortsFallback": 20,

	// Sets the source from which ports are automatically forwarded when `remote.autoForwardPorts#` is true. When `#remote.autoForwardPorts#` is false, `#remote.autoForwardPortsSource` will be used to find information about ports that have already been forwarded. On Windows and macOS remotes, the `process` and `hybrid` options have no effect and `output` will be used.
	//  - process: Ports will be automatically forwarded when discovered by watching for processes that are started and include a port.
	//  - output: Ports will be automatically forwarded when discovered by reading terminal and debug output. Not all processes that use ports will print to the integrated terminal or debug console, so some ports will be missed. Ports forwarded based on output will not be "un-forwarded" until reload or until the port is closed by the user in the Ports view.
	//  - hybrid: Ports will be automatically forwarded when discovered by reading terminal and debug output. Not all processes that use ports will print to the integrated terminal or debug console, so some ports will be missed. Ports will be "un-forwarded" by watching for processes that listen on that port to be terminated.
	"remote.autoForwardPortsSource": "process",

	// When enabled extensions are downloaded locally and installed on remote.
	"remote.downloadExtensionsLocally": false,

	// Override the kind of an extension. `ui` extensions are installed and run on the local machine while `workspace` extensions are run on the remote. By overriding an extension's default kind using this setting, you specify if that extension should be installed and enabled locally or remotely.
	"remote.extensionKind": {
		"pub.name": [
			"ui"
		]
	},

	// Controls whether local URLs with a port will be forwarded when opened from the terminal and the debug console.
	"remote.forwardOnOpen": true,

	// Specifies the local host name that will be used for port forwarding.
	"remote.localPortHost": "localhost",

	// Set default properties that are applied to all ports that don't get properties from the setting `remote.portsAttributes`. For example:
	// 
	// ```
	// {
	//   "onAutoForward": "ignore"
	// }
	// ```
	"remote.otherPortsAttributes": {},

	// Set properties that are applied when a specific port number is forwarded. For example:
	// 
	// ```
	// "3000": {
	//   "label": "Application"
	// },
	// "40000-55000": {
	//   "onAutoForward": "ignore"
	// },
	// ".+\\/server.js": {
	//  "onAutoForward": "openPreview"
	// }
	// ```
	"remote.portsAttributes": {
		"443": {
			"protocol": "https"
		},
		"8443": {
			"protocol": "https"
		}
	},

	// Restores the ports you forwarded in a workspace.
	"remote.restoreForwardedPorts": true,

	// On keypress, close the Accessible View and focus the element from which it was invoked.
	"accessibility.accessibleView.closeOnKeyPress": true,

	// Controls whether variable changes should be announced in the debug watch view.
	"accessibility.debugWatchVariableAnnouncements": true,

	// Control whether focus should automatically be sent to the REPL when code is executed.
	"accessibility.replEditor.autoFocusReplExecution": "input",

	// Controls whether the output from an execution in the native REPL will be announced.
	"accessibility.replEditor.readLastExecutionOutput": true,

	// Whether or not position changes should be debounced
	"accessibility.signalOptions.debouncePositionChanges": false,

	// 
	"accessibility.signalOptions.experimental.delays.errorAtPosition": {},

	// Delays for all signals besides error and warning at position
	"accessibility.signalOptions.experimental.delays.general": {},

	// 
	"accessibility.signalOptions.experimental.delays.warningAtPosition": {},

	// The volume of the sounds in percent (0-100).
	"accessibility.signalOptions.volume": 70,

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a chat request is made.
	"accessibility.signals.chatRequestSent": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a sound / audio cue when the response has been received.
	"accessibility.signals.chatResponseReceived": {
		"sound": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a feature is cleared (for example, the terminal, Debug Console, or Output channel).
	"accessibility.signals.clear": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a sound / audio cue when the code action has been applied.
	"accessibility.signals.codeActionApplied": {
		"sound": "auto"
	},

	// Plays a sound / audio cue - when a code action has been triggered.
	"accessibility.signals.codeActionTriggered": {
		"sound": "auto"
	},

	// Plays a sound / audio cue when the focus moves to an deleted line in Accessible Diff Viewer mode or to the next/previous change.
	"accessibility.signals.diffLineDeleted": {
		"sound": "auto"
	},

	// Plays a sound / audio cue when the focus moves to an inserted line in Accessible Diff Viewer mode or to the next/previous change.
	"accessibility.signals.diffLineInserted": {
		"sound": "auto"
	},

	// Plays a sound / audio cue when the focus moves to an modified line in Accessible Diff Viewer mode or to the next/previous change.
	"accessibility.signals.diffLineModified": {
		"sound": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a file or notebook is formatted.
	"accessibility.signals.format": {
		"sound": "never",
		"announcement": "never"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when the active line has a breakpoint.
	"accessibility.signals.lineHasBreakpoint": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when the active line has an error.
	"accessibility.signals.lineHasError": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - the active line has a folded area that can be unfolded.
	"accessibility.signals.lineHasFoldedArea": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a sound / audio cue when the active line has an inline suggestion.
	"accessibility.signals.lineHasInlineSuggestion": {
		"sound": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when the active line has a warning.
	"accessibility.signals.lineHasWarning": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when trying to read a line with inlay hints that has no inlay hints.
	"accessibility.signals.noInlayHints": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a notebook cell execution is successfully completed.
	"accessibility.signals.notebookCellCompleted": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a notebook cell execution fails.
	"accessibility.signals.notebookCellFailed": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when the debugger stopped on a breakpoint.
	"accessibility.signals.onDebugBreak": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when the active line has a warning.
	"accessibility.signals.positionHasError": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when the active line has a warning.
	"accessibility.signals.positionHasWarning": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - on loop while progress is occurring.
	"accessibility.signals.progress": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a file is saved.
	"accessibility.signals.save": {
		"sound": "never",
		"announcement": "never"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a task is completed.
	"accessibility.signals.taskCompleted": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a task fails (non-zero exit code).
	"accessibility.signals.taskFailed": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when the terminal bell is ringing.
	"accessibility.signals.terminalBell": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a terminal command fails (non-zero exit code) or when a command with such an exit code is navigated to in the accessible view.
	"accessibility.signals.terminalCommandFailed": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when a terminal command succeeds (zero exit code) or when a command with such an exit code is navigated to in the accessible view.
	"accessibility.signals.terminalCommandSucceeded": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a signal - sound (audio cue) and/or announcement (alert) - when terminal Quick Fixes are available.
	"accessibility.signals.terminalQuickFix": {
		"sound": "auto",
		"announcement": "auto"
	},

	// Plays a sound / audio cue when the voice recording has started.
	"accessibility.signals.voiceRecordingStarted": {
		"sound": "on"
	},

	// Plays a sound / audio cue when the voice recording has stopped.
	"accessibility.signals.voiceRecordingStopped": {
		"sound": "auto"
	},

	// Controls whether links should be underlined in the workbench.
	"accessibility.underlineLinks": false,

	// Provide information about actions that can be taken in the comment widget or in a file which contains comments.
	"accessibility.verbosity.comments": true,

	// Provide information about how to access the debug console accessibility help dialog when the debug console or run and debug viewlet is focused. Note that a reload of the window is required for this to take effect.
	"accessibility.verbosity.debug": true,

	// Provide information about how to navigate changes in the diff editor when it is focused.
	"accessibility.verbosity.diffEditor": true,

	// Indicate when a diff editor becomes the active editor.
	"accessibility.verbosity.diffEditorActive": true,

	// Provide information about relevant actions in an empty text editor.
	"accessibility.verbosity.emptyEditorHint": true,

	// Provide information about how to open the hover in an Accessible View.
	"accessibility.verbosity.hover": true,

	// Provide information about how to access the inline editor chat accessibility help menu and alert with hints that describe how to use the feature when the input is focused.
	"accessibility.verbosity.inlineChat": true,

	// Provide information about how to access the inline completions hover and Accessible View.
	"accessibility.verbosity.inlineCompletions": true,

	// Provide information about how to change a keybinding in the keybindings editor when a row is focused.
	"accessibility.verbosity.keybindingsEditor": true,

	// Provide information about how to focus the cell container or inner editor when a notebook cell is focused.
	"accessibility.verbosity.notebook": true,

	// Provide information about how to open the notification in an Accessible View.
	"accessibility.verbosity.notification": true,

	// Provide information about how to access the chat help menu when the chat input is focused.
	"accessibility.verbosity.panelChat": true,

	// Provide information about how to access the REPL editor accessibility help menu when the REPL editor is focused.
	"accessibility.verbosity.replEditor": true,

	// Provide information about how to access the source control accessibility help menu when the input is focused.
	"accessibility.verbosity.sourceControl": true,

	// Provide information about how to access the terminal accessibility help menu when the terminal is focused.
	"accessibility.verbosity.terminal": true,

	// Provide information about how to open the walkthrough in an Accessible View.
	"accessibility.verbosity.walkthrough": true,

	// Set the color mode for native UI elements such as native dialogs, menus and title bar. Even if your OS is configured in light color mode, you can select a dark system color theme for the window. You can also configure to automatically adjust based on the `workbench.colorTheme` setting.
	// 
	// Note: This setting is ignored when `window.autoDetectColorScheme` is enabled.
	//  - default: Native widget colors match the system colors.
	//  - auto: Use light native widget colors for light color themes and dark for dark color themes.
	//  - light: Use light native widget colors.
	//  - dark: Use dark native widget colors.
	"window.systemColorTheme": "default",

	// The name under which the remote tunnel access is registered. If not set, the host name is used.
	"remote.tunnels.access.hostNameOverride": "",

	// Prevent this computer from sleeping when remote tunnel access is turned on.
	"remote.tunnels.access.preventSleep": false,

	// An array of languages where Emmet abbreviations should not be expanded.
	"emmet.excludeLanguages": [
		"markdown"
	],

	// An array of paths, where each path can contain Emmet syntaxProfiles and/or snippet files.
	// In case of conflicts, the profiles/snippets of later paths will override those of earlier paths.
	// See https://code.visualstudio.com/docs/editor/emmet for more information and an example snippet file.
	"emmet.extensionsPath": [],

	// Enable Emmet abbreviations in languages that are not supported by default. Add a mapping here between the language and Emmet supported language.
	//  For example: `{"vue-html": "html", "javascript": "javascriptreact"}`
	"emmet.includeLanguages": {},

	// When set to `false`, the whole file is parsed to determine if current position is valid for expanding Emmet abbreviations. When set to `true`, only the content around the current position in CSS/SCSS/Less files is parsed.
	"emmet.optimizeStylesheetParsing": true,

	// Preferences used to modify behavior of some actions and resolvers of Emmet.
	"emmet.preferences": {},

	// Shows possible Emmet abbreviations as suggestions. Not applicable in stylesheets or when emmet.showExpandedAbbreviation is set to `"never"`.
	"emmet.showAbbreviationSuggestions": true,

	// Shows expanded Emmet abbreviations as suggestions.
	// The option `"inMarkupAndStylesheetFilesOnly"` applies to html, haml, jade, slim, xml, xsl, css, scss, sass, less and stylus.
	// The option `"always"` applies to all parts of the file regardless of markup/css.
	"emmet.showExpandedAbbreviation": "always",

	// If `true`, then Emmet suggestions will show up as snippets allowing you to order them as per `editor.snippetSuggestions` setting.
	"emmet.showSuggestionsAsSnippets": false,

	// Define profile for specified syntax or use your own profile with specific rules.
	"emmet.syntaxProfiles": {},

	// When enabled, Emmet abbreviations are expanded when pressing TAB, even when completions do not show up. When disabled, completions that show up can still be accepted by pressing TAB.
	"emmet.triggerExpansionOnTab": false,

	// If `true`, Emmet will use inline completions to suggest expansions. To prevent the non-inline completion item provider from showing up as often while this setting is `true`, turn `editor.quickSuggestions` to `inline` or `off` for the `other` item.
	"emmet.useInlineCompletions": false,

	// Variables to be used in Emmet snippets.
	"emmet.variables": {},

	// Controls whether force push (with or without lease) is enabled.
	"git.allowForcePush": false,

	// Controls whether commits without running pre-commit and commit-msg hooks are allowed.
	"git.allowNoVerifyCommit": false,

	// Always show the Staged Changes resource group.
	"git.alwaysShowStagedChangesResourceGroup": false,

	// Controls the signoff flag for all commits.
	"git.alwaysSignOff": false,

	// When set to true, commits will automatically be fetched from the default remote of the current Git repository. Setting to `all` will fetch from all remotes.
	"git.autofetch": false,

	// Duration in seconds between each automatic git fetch, when `git.autofetch` is enabled.
	"git.autofetchPeriod": 180,

	// Whether auto refreshing is enabled.
	"git.autorefresh": true,

	// Configures when repositories should be automatically detected.
	//  - true: Scan for both subfolders of the current opened folder and parent folders of open files.
	//  - false: Disable automatic repository scanning.
	//  - subFolders: Scan for subfolders of the currently opened folder.
	//  - openEditors: Scan for parent folders of open files.
	"git.autoRepositoryDetection": true,

	// Stash any changes before pulling and restore them after successful pull.
	"git.autoStash": false,

	// Controls whether to show blame information in the editor using editor decorations.
	"git.blame.editorDecoration.enabled": false,

	// Template for the blame information editor decoration. Supported variables:
	// 
	// * `hash`: Commit hash
	// 
	// * `hashShort`: First N characters of the commit hash according to `git.commitShortHashLength`
	// 
	// * `subject`: First line of the commit message
	// 
	// * `authorName`: Author name
	// 
	// * `authorEmail`: Author email
	// 
	// * `authorDate`: Author date
	// 
	// * `authorDateAgo`: Time difference between now and the author date
	// 
	// 
	"git.blame.editorDecoration.template": "${subject}, ${authorName} (${authorDateAgo})",

	// Controls whether to show blame information in the status bar.
	"git.blame.statusBarItem.enabled": true,

	// Template for the blame information status bar item. Supported variables:
	// 
	// * `hash`: Commit hash
	// 
	// * `hashShort`: First N characters of the commit hash according to `git.commitShortHashLength`
	// 
	// * `subject`: First line of the commit message
	// 
	// * `authorName`: Author name
	// 
	// * `authorEmail`: Author email
	// 
	// * `authorDate`: Author date
	// 
	// * `authorDateAgo`: Time difference between now and the author date
	// 
	// 
	"git.blame.statusBarItem.template": "${authorName} (${authorDateAgo})",

	// Prefix used when creating a new branch.
	"git.branchPrefix": "",

	// List of protected branches. By default, a prompt is shown before changes are committed to a protected branch. The prompt can be controlled using the `git.branchProtectionPrompt`  setting.
	"git.branchProtection": [],

	// Controls whether a prompt is being shown before changes are committed to a protected branch.
	//  - alwaysCommit: Always commit changes to the protected branch.
	//  - alwaysCommitToNewBranch: Always commit changes to a new branch.
	//  - alwaysPrompt: Always prompt before changes are committed to a protected branch.
	"git.branchProtectionPrompt": "alwaysPrompt",

	// List of dictionaries used for the randomly generated branch name. Each value represents the dictionary used to generate the segment of the branch name. Supported dictionaries: `adjectives`, `animals`, `colors` and `numbers`.
	//  - adjectives: A random adjective
	//  - animals: A random animal name
	//  - colors: A random color name
	//  - numbers: A random number between 100 and 999
	"git.branchRandomName.dictionary": [
		"adjectives",
		"animals"
	],

	// Controls whether a random name is generated when creating a new branch.
	"git.branchRandomName.enable": false,

	// Controls the sort order for branches.
	"git.branchSortOrder": "committerdate",

	// A regular expression to validate new branch names.
	"git.branchValidationRegex": "",

	// The character to replace whitespace in new branch names, and to separate segments of a randomly generated branch name.
	"git.branchWhitespaceChar": "-",

	// Controls what type of Git refs are listed when running `Checkout to...`.
	//  - local: Local branches
	//  - tags: Tags
	//  - remote: Remote branches
	"git.checkoutType": [
		"local",
		"remote",
		"tags"
	],

	// Controls whether the diff editor should be automatically closed when changes are stashed, committed, discarded, staged, or unstaged.
	"git.closeDiffOnOperation": false,

	// List of git commands (ex: commit, push) that would have their `stdout` logged to the [git output](command:git.showOutput). If the git command has a client-side hook configured, the client-side hook's `stdout` will also be logged to the [git output](command:git.showOutput).
	"git.commandsToLog": [],

	// Controls the length of the commit short hash.
	"git.commitShortHashLength": 7,

	// Always confirm the creation of empty commits for the 'Git: Commit Empty' command.
	"git.confirmEmptyCommits": true,

	// Controls whether to ask for confirmation before force-pushing.
	"git.confirmForcePush": true,

	// Controls whether to ask for confirmation before committing without verification.
	"git.confirmNoVerifyCommit": true,

	// Confirm before synchronizing Git repositories.
	"git.confirmSync": true,

	// Controls the Git count badge.
	//  - all: Count all changes.
	//  - tracked: Count only tracked changes.
	//  - off: Turn off counter.
	"git.countBadge": "all",

	// Controls whether Git contributes colors and badges to the Explorer and the Open Editors view.
	"git.decorations.enabled": true,

	// The name of the default branch (example: main, trunk, development) when initializing a new Git repository. When set to empty, the default branch name configured in Git will be used. **Note:** Requires Git version `2.28.0` or later.
	"git.defaultBranchName": "main",

	// The default location to clone a Git repository.
	"git.defaultCloneDirectory": null,

	// Controls whether to automatically detect Git submodules.
	"git.detectSubmodules": true,

	// Controls the limit of Git submodules detected.
	"git.detectSubmodulesLimit": 10,

	// Enables commit signing with GPG, X.509, or SSH.
	"git.enableCommitSigning": false,

	// Whether Git is enabled.
	"git.enabled": true,

	// Commit all changes when there are no staged changes.
	"git.enableSmartCommit": false,

	// Controls whether the Git Sync command appears in the status bar.
	"git.enableStatusBarSync": true,

	// When enabled, fetch all branches when pulling. Otherwise, fetch just the current one.
	"git.fetchOnPull": false,

	// Push all annotated tags when running the sync command.
	"git.followTagsWhenSync": false,

	// This setting is now deprecated, please use `github.gitAuthentication` instead.
	// 
	"git.githubAuthentication": null,

	// List of Git repositories to ignore.
	"git.ignoredRepositories": [],

	// Ignores the legacy Git warning.
	"git.ignoreLegacyWarning": false,

	// Ignores the warning when there are too many changes in a repository.
	"git.ignoreLimitWarning": false,

	// Ignores the warning when Git is missing.
	"git.ignoreMissingGitWarning": false,

	// Ignores the warning when it looks like the branch might have been rebased when pulling.
	"git.ignoreRebaseWarning": false,

	// Ignore modifications to submodules in the file tree.
	"git.ignoreSubmodules": false,

	// Ignores the warning when Git 2.25 - 2.26 is installed on Windows.
	"git.ignoreWindowsGit27Warning": false,

	// Controls whether to show commit message input validation diagnostics.
	"git.inputValidation": false,

	// Controls the commit message length threshold for showing a warning.
	"git.inputValidationLength": 72,

	// Controls the commit message subject length threshold for showing a warning. Unset it to inherit the value of `git.inputValidationLength`.
	"git.inputValidationSubjectLength": 50,

	// Open the merge editor for files that are currently under conflict.
	"git.mergeEditor": false,

	// Controls whether to open a repository automatically after cloning.
	//  - always: Always open in current window.
	//  - alwaysNewWindow: Always open in a new window.
	//  - whenNoFolderOpen: Only open in current window when no folder is opened.
	//  - prompt: Always prompt for action.
	"git.openAfterClone": "prompt",

	// Controls whether the diff editor should be opened when clicking a change. Otherwise the regular editor will be opened.
	"git.openDiffOnClick": true,

	// Control whether a repository in parent folders of workspaces or open files should be opened.
	//  - always: Always open a repository in parent folders of workspaces or open files.
	//  - never: Never open a repository in parent folders of workspaces or open files.
	//  - prompt: Prompt before opening a repository the parent folders of workspaces or open files.
	"git.openRepositoryInParentFolders": "prompt",

	// Controls whether to optimistically update the state of the Source Control view after running git commands.
	"git.optimisticUpdate": true,

	// Path and filename of the git executable, e.g. `C:\Program Files\Git\bin\git.exe` (Windows). This can also be an array of string values containing multiple paths to look up.
	"git.path": null,

	// Run a git command after a successful commit.
	//  - none: Don't run any command after a commit.
	//  - push: Run 'git push' after a successful commit.
	//  - sync: Run 'git pull' and 'git push' after a successful commit.
	"git.postCommitCommand": "none",

	// Controls whether Git should check for unsaved files before committing.
	//  - always: Check for any unsaved files.
	//  - staged: Check only for unsaved staged files.
	//  - never: Disable this check.
	"git.promptToSaveFilesBeforeCommit": "always",

	// Controls whether Git should check for unsaved files before stashing changes.
	//  - always: Check for any unsaved files.
	//  - staged: Check only for unsaved staged files.
	//  - never: Disable this check.
	"git.promptToSaveFilesBeforeStash": "always",

	// Prune when fetching.
	"git.pruneOnFetch": false,

	// Controls whether a branch that does not have outgoing commits is fast-forwarded before it is checked out.
	"git.pullBeforeCheckout": false,

	// Fetch all tags when pulling.
	"git.pullTags": true,

	// Force Git to use rebase when running the sync command.
	"git.rebaseWhenSync": false,

	// Remember the last git command that ran after a commit.
	"git.rememberPostCommitCommand": false,

	// Automatically replace the local tags with the remote tags in case of a conflict when running the pull command.
	"git.replaceTagsWhenPull": false,

	// List of folders that are ignored while scanning for Git repositories when `git.autoRepositoryDetection` is set to `true` or `subFolders`.
	"git.repositoryScanIgnoredFolders": [
		"node_modules"
	],

	// Controls the depth used when scanning workspace folders for Git repositories when `git.autoRepositoryDetection` is set to `true` or `subFolders`. Can be set to `-1` for no limit.
	"git.repositoryScanMaxDepth": 1,

	// Controls whether to require explicit Git user configuration or allow Git to guess if missing.
	"git.requireGitUserConfig": true,

	// List of paths to search for Git repositories in.
	"git.scanRepositories": [],

	// Controls whether an action button is shown in the Source Control view.
	"git.showActionButton": {
		"commit": true,
		"publish": true,
		"sync": true
	},

	// Controls whether to show the commit input in the Git source control panel.
	"git.showCommitInput": true,

	// Controls whether to show an inline Open File action in the Git changes view.
	"git.showInlineOpenFileAction": true,

	// Controls whether Git actions should show progress.
	"git.showProgress": true,

	// Controls whether to show a notification when a push is successful.
	"git.showPushSuccessNotification": false,

	// Controls the threshold of the similarity index (the amount of additions/deletions compared to the file's size) for changes in a pair of added/deleted files to be considered a rename. **Note:** Requires Git version `2.18.0` or later.
	"git.similarityThreshold": 50,

	// Control which changes are automatically staged by Smart Commit.
	//  - all: Automatically stage all changes.
	//  - tracked: Automatically stage tracked changes only.
	"git.smartCommitChanges": "all",

	// Controls how to limit the number of changes that can be parsed from Git status command. Can be set to 0 for no limit.
	"git.statusLimit": 10000,

	// Suggests to enable smart commit (commit all changes when there are no staged changes).
	"git.suggestSmartCommit": true,

	// Controls whether a notification comes up when running the Sync action, which allows the user to cancel the operation.
	"git.supportCancellation": false,

	// Controls whether to enable VS Code to be the authentication handler for Git processes spawned in the Integrated Terminal. Note: Terminals need to be restarted to pick up a change in this setting.
	"git.terminalAuthentication": true,

	// Controls whether to enable VS Code to be the Git editor for Git processes spawned in the integrated terminal. Note: Terminals need to be restarted to pick up a change in this setting.
	"git.terminalGitEditor": false,

	// Controls which date to use for items in the Timeline view.
	//  - committed: Use the committed date
	//  - authored: Use the authored date
	"git.timeline.date": "committed",

	// Controls whether to show the commit author in the Timeline view.
	"git.timeline.showAuthor": true,

	// Controls whether to show uncommitted changes in the Timeline view.
	"git.timeline.showUncommitted": false,

	// Controls how untracked changes behave.
	//  - mixed: All changes, tracked and untracked, appear together and behave equally.
	//  - separate: Untracked changes appear separately in the Source Control view. They are also excluded from several actions.
	//  - hidden: Untracked changes are hidden and excluded from several actions.
	"git.untrackedChanges": "mixed",

	// Controls whether to use the message from the commit input box as the default stash message.
	"git.useCommitInputAsStashMessage": false,

	// Controls whether a full text editor will be used to author commit messages, whenever no message is provided in the commit input box.
	"git.useEditorAsCommitInput": true,

	// Controls whether force pushing uses the safer force-if-includes variant. Note: This setting requires the `git.useForcePushWithLease` setting to be enabled, and Git version `2.30.0` or later.
	"git.useForcePushIfIncludes": true,

	// Controls whether force pushing uses the safer force-with-lease variant.
	"git.useForcePushWithLease": true,

	// Controls whether GIT_ASKPASS should be overwritten to use the integrated version.
	"git.useIntegratedAskPass": true,

	// Enable verbose output when `git.useEditorAsCommitInput` is enabled.
	"git.verboseCommit": false,

	// Controls whether to query repository rules for GitHub repositories
	"github.branchProtection": true,

	// Controls whether to enable automatic GitHub authentication for git commands within VS Code.
	"github.gitAuthentication": true,

	// Controls which protocol is used to clone a GitHub repository
	"github.gitProtocol": "https",

	// Controls whether to show the GitHub avatar of the commit author in various hovers (ex: Git blame, Timeline, Source Control Graph, etc.)
	"github.showAvatar": true,

	// GitHub Enterprise Server URI
	"github-enterprise.uri": "",

	// Controls enablement of Grunt task detection. Grunt task detection can cause files in any open workspace to be executed.
	"grunt.autoDetect": "off",

	// Controls enablement of Gulp task detection. Gulp task detection can cause files in any open workspace to be executed.
	"gulp.autoDetect": "off",

	// Experimental feature to serialize the Jupyter notebook in a worker thread.
	"ipynb.experimental.serialization": false,

	// Enable/disable pasting of images into Markdown cells in ipynb notebook files. Pasted images are inserted as attachments to the cell.
	"ipynb.pasteImagesAsAttachments.enabled": true,

	// Controls enablement of Jake task detection. Jake task detection can cause files in any open workspace to be executed.
	"jake.autoDetect": "off",

	// Enable/disable rendering math in the built-in Markdown preview.
	"markdown.math.enabled": true,

	// A collection of custom macros. Each macro is a key-value pair where the key is a new command name and the value is the expansion of the macro.
	"markdown.math.macros": {},

	// Start playing videos on mute automatically.
	"mediaPreview.video.autoPlay": false,

	// Loop videos over again automatically.
	"mediaPreview.video.loop": false,

	// Whether to automatically navigate to the next merge conflict after resolving a merge conflict.
	"merge-conflict.autoNavigateNextConflict.enabled": false,

	// Create a CodeLens for merge conflict blocks within editor.
	"merge-conflict.codeLens.enabled": true,

	// Create decorators for merge conflict blocks within editor.
	"merge-conflict.decorators.enabled": true,

	// Controls where the diff view should be opened when comparing changes in merge conflicts.
	//  - Current: Open the diff view in the current editor group.
	//  - Beside: Open the diff view next to the current editor group.
	//  - Below: Open the diff view below the current editor group.
	"merge-conflict.diffViewPosition": "Current",

	// The custom configuration for the Sovereign Cloud to use with the Microsoft Sovereign Cloud authentication provider. This along with setting `microsoft-sovereign-cloud.environment` to `custom` is required to use this feature.
	"microsoft-sovereign-cloud.customEnvironment": {},

	// The Sovereign Cloud to use for authentication. If you select `custom`, you must also set the `microsoft-sovereign-cloud.customEnvironment` setting.
	//  - ChinaCloud: Azure China
	//  - USGovernment: Azure US Government
	//  - custom: A custom Microsoft Sovereign Cloud
	"microsoft-sovereign-cloud.environment": "",

	// The version of the Microsoft Account client ID to use for signing in with a Microsoft account. Only change this if you have been asked to. The default is `v1`.
	//  - v2: Use the v2 Microsoft Account client ID to sign in with a Microsoft account.
	//  - v1: Use the v1 Microsoft Account client ID to sign in with a Microsoft account.
	"microsoft-authentication.clientIdVersion": "v1",

	// The authentication implementation to use for signing in with a Microsoft account.
	// 
	// *NOTE: The `classic` implementation is deprecated and will be removed, along with this setting, in a future release. If only the `classic` implementation works for you, please [open an issue](command:workbench.action.openIssueReporter) and explain what you are trying to log in to.*
	//  - msal: Use the Microsoft Authentication Library (MSAL) to sign in with a Microsoft account.
	//  - classic: (deprecated) Use the classic authentication flow to sign in with a Microsoft account.
	"microsoft-authentication.implementation": "msal",

	// Configures which processes to automatically attach and debug when `debug.node.autoAttach` is on. A Node process launched with the `--inspect` flag will always be attached to, regardless of this setting.
	//  - always: Auto attach to every Node.js process launched in the terminal.
	//  - smart: Auto attach when running scripts that aren't in a node_modules folder.
	//  - onlyWithFlag: Only auto attach when the `--inspect` is given.
	//  - disabled: Auto attach is disabled and not shown in status bar.
	"debug.javascript.autoAttachFilter": "disabled",

	// Configures glob patterns for determining when to attach in "smart" `debug.javascript.autoAttachFilter` mode. `$KNOWN_TOOLS$` is replaced with a list of names of common test and code runners. [Read more on the VS Code docs](https://code.visualstudio.com/docs/nodejs/nodejs-debugging#_auto-attach-smart-patterns).
	"debug.javascript.autoAttachSmartPattern": [
		"${workspaceFolder}/**",
		"!**/node_modules/**",
		"**/$KNOWN_TOOLS$/**"
	],

	// When debugging a remote web app, configures whether to automatically tunnel the remote server to your local machine.
	"debug.javascript.automaticallyTunnelRemoteServer": true,

	// Whether to stop when conditional breakpoints throw an error.
	"debug.javascript.breakOnConditionalError": false,

	// Where a "Run" and "Debug" code lens should be shown in your npm scripts. It may be on "all", scripts, on "top" of the script section, or "never".
	"debug.javascript.codelens.npmScripts": "top",

	// Options used when debugging open links clicked from inside the JavaScript Debug Terminal. Can be set to "off" to disable this behavior, or "always" to enable debugging in all terminals.
	"debug.javascript.debugByLinkOptions": "on",

	// The default `runtimeExecutable` used for launch configurations, if unspecified. This can be used to config custom paths to Node.js or browser installations.
	"debug.javascript.defaultRuntimeExecutable": {
		"pwa-node": "node"
	},

	// Enables the experimental network view for targets that support it.
	"debug.javascript.enableNetworkView": false,

	// Default options used when debugging a process through the `Debug: Attach to Node.js Process` command
	"debug.javascript.pickAndAttachOptions": {},

	// Request options to use when loading resources, such as source maps, in the debugger. You may need to configure this if your sourcemaps require authentication or use a self-signed certificate, for instance. Options are used to create a request using the [`got`](https://github.com/sindresorhus/got) library.
	// 
	// A common case to disable certificate verification can be done by passing `{ "https": { "rejectUnauthorized": false } }`.
	"debug.javascript.resourceRequestOptions": {},

	// Default launch options for the JavaScript debug terminal and npm scripts.
	"debug.javascript.terminalOptions": {},

	// Configures whether sourcemapped file where the original file can't be read will automatically be unmapped. If this is false (default), a prompt is shown.
	"debug.javascript.unmapMissingSources": false,

	// Controls whether npm scripts should be automatically detected.
	"npm.autoDetect": "on",

	// Enable running npm scripts contained in a folder from the Explorer context menu.
	"npm.enableRunFromFolder": false,

	// The NPM Script Explorer is now available in 'Views' menu in the Explorer in all folders.
	// Enable an explorer view for npm scripts when there is no top-level 'package.json' file.
	"npm.enableScriptExplorer": false,

	// Configure glob patterns for folders that should be excluded from automatic script detection.
	"npm.exclude": "",

	// Fetch data from https://registry.npmjs.org and https://registry.bower.io to provide auto-completion and information on hover features on npm dependencies.
	"npm.fetchOnlinePackageInfo": true,

	// The package manager used to run scripts.
	//  - auto: Auto-detect which package manager to use for running scripts based on lock files and installed package managers.
	//  - npm: Use npm as the package manager for running scripts.
	//  - yarn: Use yarn as the package manager for running scripts.
	//  - pnpm: Use pnpm as the package manager for running scripts.
	//  - bun: Use bun as the package manager for running scripts.
	"npm.packageManager": "auto",

	// Run npm commands with the `--silent` option.
	"npm.runSilent": false,

	// The default click action used in the NPM Scripts Explorer: `open` or `run`, the default is `open`.
	"npm.scriptExplorerAction": "open",

	// An array of regular expressions that indicate which scripts should be excluded from the NPM Scripts view.
	"npm.scriptExplorerExclude": [],

	// Display hover with 'Run' and 'Debug' commands for scripts.
	"npm.scriptHover": true,

	// Controls whether 'Peek References' or 'Find References' is invoked when selecting CodeLens references.
	//  - peek: Show references in peek editor.
	//  - view: Show references in separate view.
	"references.preferredLocation": "peek",

	// Enable/disable the floating indicator that shows when focused in the simple browser.
	"simpleBrowser.focusLockIndicator.enabled": true,

	// For import command. The declaration type used for require()
	"npm-intellisense.importDeclarationType": "const",

	// For import command. Use import statements instead of require()
	"npm-intellisense.importES6": true,

	// For import command. The linebreak used after the snippet
	"npm-intellisense.importLinebreak": ";\r\n",

	// For import command. The type of quotes to use in the snippet
	"npm-intellisense.importQuotes": "'",

	// (experimental) Enables path intellisense in subfolders of modules
	"npm-intellisense.packageSubfoldersIntellisense": false,

	// Look for package.json inside nearest directory instead of workspace root
	"npm-intellisense.recursivePackageJsonLookup": true,

	// Scans devDependencies as well
	"npm-intellisense.scanDevDependencies": false,

	// shows build in node modules like 'path' of 'fs'
	"npm-intellisense.showBuildInLibs": false,

	// When to validate class selectors.
	"css.autoValidation": "Never",

	// List of languages which suggestions are desired.
	"css.enabledLanguages": [
		"html"
	],

	// List of local or remote style sheets for suggestions.
	"css.styleSheets": [],

	// Include parentheses around a sole arrow function parameter.
	"prettier.arrowParens": "always",

	// Puts the `>` of a multi-line HTML (HTML, JSX, Vue, Angular) element at the end of the last line instead of being alone on the next line (does not apply to self closing elements).
	"prettier.bracketSameLine": false,

	// Controls the printing of spaces inside object literals.
	"prettier.bracketSpacing": true,

	// Path to the prettier configuration file.
	"prettier.configPath": "",

	// This feature is no longer supported. Instead, configure VS Code [default formatters](https://github.com/prettier/prettier-vscode#default-formatter) or use .prettierignore.
	// A list of languages IDs to disable this extension on.
	"prettier.disableLanguages": [],

	// A list of [glob patterns](https://code.visualstudio.com/api/references/vscode-api#GlobPattern) to register Prettier formatter.
	"prettier.documentSelectors": [],

	// Control whether Prettier formats quoted code embedded in the file.
	"prettier.embeddedLanguageFormatting": "auto",

	// Controls whether Prettier is enabled or not. Reload required.
	"prettier.enable": true,

	// Enable debug logs for troubleshooting.
	"prettier.enableDebugLogs": false,

	// Specify the end of line used by prettier.
	"prettier.endOfLine": "lf",

	// Try prettier's [new ternary formatting](https://github.com/prettier/prettier/pull/13183) before it becomes the default behavior.
	"prettier.experimentalTernaries": false,

	// Specify the global [whitespace sensitivity](https://prettier.io/blog/2018/11/07/1.15.0.html#whitespace-sensitive-formatting) for HTML files.
	// Valid options:
	// - `css` - Respect the default value of CSS `display` property.
	// - `strict` - Whitespaces are considered sensitive.
	// - `ignore` - Whitespaces are considered insensitive.
	"prettier.htmlWhitespaceSensitivity": "css",

	// Path to a `.prettierignore` file.
	"prettier.ignorePath": ".prettierignore",

	// Prettier can insert a special `@format` marker at the top of files specifying that the file has been formatted with prettier. This works well when used in tandem with the `--require-pragma` option. If there is already a docblock at the top of the file then this option will add a newline to it with the `@format` marker.
	"prettier.insertPragma": false,

	// This option has been deprecated in v2.4.0, use `bracketSameLine` instead.
	// Puts the `>` of a multi-line jsx element at the end of the last line instead of being alone on the next line (does not apply to self closing elements).
	"prettier.jsxBracketSameLine": false,

	// Use single quotes instead of double quotes in JSX.
	"prettier.jsxSingleQuote": false,

	// Package manager is now automatically detected by VS Code. This setting is no longer used.
	// The package manager you use to install node modules.
	"prettier.packageManager": "npm",

	// Path to the `prettier` module, eg: `./node_modules/prettier`.
	"prettier.prettierPath": "",

	// Fit code within this line limit.
	"prettier.printWidth": 80,

	// (Markdown) wrap prose over multiple lines.
	"prettier.proseWrap": "preserve",

	// Change when properties in objects are quoted.
	// Valid options:
	// - `"as-needed"` - Only add quotes around object properties where required.
	// - `"consistent"` - If at least one property in an object requires quotes, quote all properties.
	// - `"preserve"` - Respect the input use of quotes in object properties.
	"prettier.quoteProps": "as-needed",

	// Require a prettier configuration file to format. See [documentation for valid configuration files](https://prettier.io/docs/en/configuration.html).
	// 
	// > _Note, untitled files will still be formatted using the VS Code prettier settings even when this setting is set._
	"prettier.requireConfig": false,

	// Prettier can restrict itself to only format files that contain a special comment, called a pragma, at the top of the file. This is very useful when gradually transitioning large, unformatted codebases to prettier.
	"prettier.requirePragma": false,

	// When enabled, this extension will attempt to use global npm or yarn modules if local modules cannot be resolved.
	// > _This setting can have a negative performance impact, particularly on Windows when you have attached network drives. Only enable this if you must use global modules._
	"prettier.resolveGlobalModules": false,

	// Whether to add a semicolon at the end of every line.
	"prettier.semi": true,

	// Enforces single attribute per line in HTML, JSX, Vue and Angular.
	"prettier.singleAttributePerLine": false,

	// Use single instead of double quotes.
	"prettier.singleQuote": false,

	// Number of spaces it should use per tab.
	"prettier.tabWidth": 2,

	// Controls the printing of trailing commas wherever possible. 
	// Valid options:
	// - `none` - No trailing commas
	// - `es5` - Trailing commas where valid in ES5 (objects, arrays, etc)
	// - `all` - Trailing commas wherever possible (function arguments)
	"prettier.trailingComma": "es5",

	// Whether or not to take `.editorconfig` into account when parsing configuration. See the [`prettier.resolveConfig`](https://prettier.io/docs/en/api.html) docs for details.
	"prettier.useEditorConfig": true,

	// Indent lines with tabs.
	"prettier.useTabs": false,

	// Whether or not to indent the code inside `<script>` and `<style>` tags in Vue SFC files.
	"prettier.vueIndentScriptAndStyle": false,

	// This extension will process files in `node_modules`.
	"prettier.withNodeModules": false,

	// Set the languages that the extension will be activated.  e.g. ["html","xml","php"] By default, it is ["*"] and will be activated for all languages.
	"auto-rename-tag.activationOnLanguage": [
		"*"
	],

	// Whether to clear previous output before each run.
	"code-runner.clearPreviousOutput": false,

	// Set the custom command to run.
	"code-runner.customCommand": "echo Hello",

	// Set the working directory.
	"code-runner.cwd": "",

	// Set the default language to run.
	"code-runner.defaultLanguage": "",

	// Whether to enable AppInsights to track user telemetry data.
	"code-runner.enableAppInsights": true,

	// Set the executor of each language.
	"code-runner.executorMap": {
		"javascript": "node",
		"java": "cd $dir && javac $fileName && java $fileNameWithoutExt",
		"c": "cd $dir && gcc $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		"zig": "zig run",
		"cpp": "cd $dir && g++ $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		"objective-c": "cd $dir && gcc -framework Cocoa $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		"php": "php",
		"python": "python -u",
		"perl": "perl",
		"perl6": "perl6",
		"ruby": "ruby",
		"go": "go run",
		"lua": "lua",
		"groovy": "groovy",
		"powershell": "powershell -ExecutionPolicy ByPass -File",
		"bat": "cmd /c",
		"shellscript": "bash",
		"fsharp": "fsi",
		"csharp": "scriptcs",
		"vbscript": "cscript //Nologo",
		"typescript": "ts-node",
		"coffeescript": "coffee",
		"scala": "scala",
		"swift": "swift",
		"julia": "julia",
		"crystal": "crystal",
		"ocaml": "ocaml",
		"r": "Rscript",
		"applescript": "osascript",
		"clojure": "lein exec",
		"haxe": "haxe --cwd $dirWithoutTrailingSlash --run $fileNameWithoutExt",
		"rust": "cd $dir && rustc $fileName && $dir$fileNameWithoutExt",
		"racket": "racket",
		"scheme": "csi -script",
		"ahk": "autohotkey",
		"autoit": "autoit3",
		"dart": "dart",
		"pascal": "cd $dir && fpc $fileName && $dir$fileNameWithoutExt",
		"d": "cd $dir && dmd $fileName && $dir$fileNameWithoutExt",
		"haskell": "runghc",
		"nim": "nim compile --verbosity:0 --hints:off --run",
		"lisp": "sbcl --script",
		"kit": "kitc --run",
		"v": "v run",
		"sass": "sass --style expanded",
		"scss": "scss --style expanded",
		"less": "cd $dir && lessc $fileName $fileNameWithoutExt.css",
		"FortranFreeForm": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		"fortran-modern": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		"fortran_fixed-form": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		"fortran": "cd $dir && gfortran $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		"sml": "cd $dir && sml $fileName",
		"mojo": "mojo run",
		"erlang": "escript",
		"spwn": "spwn build",
		"pkl": "cd $dir && pkl eval -f yaml $fileName -o $fileNameWithoutExt.yaml",
		"gleam": "gleam run -m $fileNameWithoutExt"
	},

	// Set the executor of each file extension.
	"code-runner.executorMapByFileExtension": {
		".vb": "cd $dir && vbc /nologo $fileName && $dir$fileNameWithoutExt",
		".vbs": "cscript //Nologo",
		".scala": "scala",
		".jl": "julia",
		".cr": "crystal",
		".ml": "ocaml",
		".zig": "zig run",
		".exs": "elixir",
		".hx": "haxe --cwd $dirWithoutTrailingSlash --run $fileNameWithoutExt",
		".rkt": "racket",
		".scm": "csi -script",
		".ahk": "autohotkey",
		".au3": "autoit3",
		".kt": "cd $dir && kotlinc $fileName -include-runtime -d $fileNameWithoutExt.jar && java -jar $fileNameWithoutExt.jar",
		".kts": "kotlinc -script",
		".dart": "dart",
		".pas": "cd $dir && fpc $fileName && $dir$fileNameWithoutExt",
		".pp": "cd $dir && fpc $fileName && $dir$fileNameWithoutExt",
		".d": "cd $dir && dmd $fileName && $dir$fileNameWithoutExt",
		".hs": "runhaskell",
		".nim": "nim compile --verbosity:0 --hints:off --run",
		".csproj": "dotnet run --project",
		".fsproj": "dotnet run --project",
		".lisp": "sbcl --script",
		".kit": "kitc --run",
		".v": "v run",
		".vsh": "v run",
		".sass": "sass --style expanded",
		".cu": "cd $dir && nvcc $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
		".ring": "ring",
		".sml": "cd $dir && sml $fileName",
		".mojo": "mojo run",
		".erl": "escript",
		".spwn": "spwn build",
		".pkl": "cd $dir && pkl eval -f yaml $fileName -o $fileNameWithoutExt.yaml",
		".gleam": "gleam run -m $fileNameWithoutExt"
	},

	// Set the executor by glob.
	"code-runner.executorMapByGlob": {
		"pom.xml": "cd $dir && mvn clean package"
	},

	// Whether to use the directory of the file to be executed as the working directory.
	"code-runner.fileDirectoryAsCwd": false,

	// Whether to ignore selection to always run entire file.
	"code-runner.ignoreSelection": false,

	// Set the mapping of languageId to file extension.
	"code-runner.languageIdToFileExtensionMap": {
		"bat": ".bat",
		"powershell": ".ps1",
		"typescript": ".ts"
	},

	// Whether to preserve focus on code editor after code run is triggered.
	"code-runner.preserveFocus": true,

	// Whether to respect Shebang to run code.
	"code-runner.respectShebang": true,

	// Whether to run code in Integrated Terminal.
	"code-runner.runInTerminal": false,

	// Whether to save all files before running.
	"code-runner.saveAllFilesBeforeRun": false,

	// Whether to save the current file before running.
	"code-runner.saveFileBeforeRun": false,

	// Whether to show extra execution message like [Running] ... and [Done] ...
	"code-runner.showExecutionMessage": true,

	// Whether to show 'Run Code' command in editor context menu.
	"code-runner.showRunCommandInEditorContextMenu": true,

	// Whether to show 'Run Code' command in explorer context menu.
	"code-runner.showRunCommandInExplorerContextMenu": true,

	// Whether to show 'Run Code' icon in editor title menu.
	"code-runner.showRunIconInEditorTitleMenu": true,

	// Whether to show 'Stop code run' icon in the editor title menu when code is running.
	"code-runner.showStopIconInEditorTitleMenu": true,

	// Temporary file name used in running selected code snippet. When it is set as empty, the file name will be random.
	"code-runner.temporaryFileName": "tempCodeRunnerFile",

	// For Windows system, replaces the Windows style drive letter in the command with a Unix style root when using a custom shell as the terminal, like Bash or Cgywin. Example: Setting this to '/mnt/' will replace 'C:\path' with '/mnt/c/path'
	"code-runner.terminalRoot": "",

	// Enabling will always prompt which repository to create an issue in instead of basing off the current open file.
	"githubIssues.alwaysPromptForNewIssueRepo": false,

	// Assigns the issue you're working on to you. Only applies when the issue you're working on is in a repo you currently have open.
	"githubIssues.assignWhenWorking": true,

	// Controls whether an issue number (ex. #1234) or a full url (ex. https://github.com/owner/name/issues/1234) is inserted when the Create Issue code action is run.
	"githubIssues.createInsertFormat": "number",

	// Strings that will cause the 'Create issue from comment' code action to show.
	"githubIssues.createIssueTriggers": [
		"TODO",
		"todo",
		"BUG",
		"FIXME",
		"ISSUE",
		"HACK"
	],

	// Languages that the '#' character should not be used to trigger issue completion suggestions.
	"githubIssues.ignoreCompletionTrigger": [
		"coffeescript",
		"diff",
		"dockerfile",
		"dockercompose",
		"ignore",
		"ini",
		"julia",
		"makefile",
		"perl",
		"powershell",
		"python",
		"r",
		"ruby",
		"shellscript",
		"yaml"
	],

	// An array of milestones titles to never show issues from.
	"githubIssues.ignoreMilestones": [],

	// Languages that the '@' character should not be used to trigger user completion suggestions.
	"githubIssues.ignoreUserCompletionTrigger": [],

	// Advanced settings for the name of the branch that is created when you start working on an issue. 
	// - `${user}` will be replace with the currently logged in username 
	// - `${issueNumber}` will be replaced with the current issue number 
	// - `${sanitizedIssueTitle}` will be replaced with the issue title, with all spaces and unsupported characters (https://git-scm.com/docs/git-check-ref-format) removed
	"githubIssues.issueBranchTitle": "${user}/issue${issueNumber}",

	// Sets the format of issue completions in the SCM inputbox. 
	// - `${user}` will be replace with the currently logged in username 
	// - `${issueNumber}` will be replaced with the current issue number 
	// - `${issueNumberLabel}` will be replaced with a label formatted as #number or owner/repository#number, depending on whether the issue is in the current repository
	"githubIssues.issueCompletionFormatScm": "${issueTitle} ${issueNumberLabel}",

	// Controls whether completion suggestions are shown for issues.
	"githubIssues.issueCompletions.enabled": true,

	// Specifies what queries should be used in the GitHub issues tree using [GitHub search syntax](https://help.github.com/en/articles/understanding-the-search-syntax) with variables. The first query listed will be expanded in the Issues view. The "default" query includes issues assigned to you by Milestone. If you want to preserve these, make sure they are still in the array when you modify the setting.
	"githubIssues.queries": [
		{
			"label": "My Issues",
			"query": "is:open assignee:${user} repo:${owner}/${repository}",
			"groupBy": [
				"milestone"
			]
		},
		{
			"label": "Created Issues",
			"query": "author:${user} state:open repo:${owner}/${repository} sort:created-desc"
		},
		{
			"label": "Recent Issues",
			"query": "state:open repo:${owner}/${repository} sort:updated-desc"
		}
	],

	// Determines whether a branch should be checked out when working on an issue. To configure the name of the branch, set `githubIssues.issueBranchTitle`.
	//  - on: A branch will always be checked out when you start working on an issue. If the branch doesn't exist, it will be created.
	//  - off: A branch will not be created when you start working on an issue. If you have worked on an issue before and a branch was created for it, that same branch will be checked out.
	//  - prompt: A prompt will show for setting the name of the branch that will be created and checked out.
	"githubIssues.useBranchForIssues": "on",

	// Controls whether completion suggestions are shown for users.
	"githubIssues.userCompletions.enabled": true,

	// Sets the format of the commit message that is set in the SCM inputbox when you **Start Working on an Issue**. Defaults to `${issueTitle} 
	// Fixes ${issueNumberLabel}`
	"githubIssues.workingIssueFormatScm": "${issueTitle} \nFixes ${issueNumberLabel}",

	// Allows `git fetch` to be run for checked-out pull request branches when checking for updates to the pull request.
	"githubPullRequests.allowFetch": true,

	// All pull requests created with this extension will be assigned to this user. To assign to yourself, use the '${user}' variable.
	"githubPullRequests.assignCreated": "",

	// Controls whether comments are expanded when a document with comments is opened. Requires a reload to take effect for comments that have already been added.
	//  - expandUnresolved: All unresolved comments will be expanded.
	//  - collapseAll: All comments will be collapsed
	"githubPullRequests.commentExpandState": "expandUnresolved",

	// Controls what the base branch picker defaults to when creating a pull request
	//  - repositoryDefault: The default branch of the repository
	//  - createdFromBranch: The branch that the current branch was created from, if known
	//  - auto: When the current repository is a fork, this will work like "repositoryDefault". Otherwise, it will work like "createdFromBranch".
	"githubPullRequests.createDefaultBaseBranch": "auto",

	// Use the setting 'githubPullRequests.defaultCreateOption' instead.
	// Whether the "Draft" checkbox will be checked by default when creating a pull request.
	"githubPullRequests.createDraft": false,

	// Create a pull request when a branch is published.
	//  - never: Never create a pull request when a branch is published.
	//  - ask: Ask if you want to create a pull request when a branch is published.
	"githubPullRequests.createOnPublishBranch": "ask",

	// The default comment type to use when submitting a comment and there is no active review
	//  - single: Submits the comment as a single comment that will be immediately visible to other users
	//  - review: Submits the comment as a review comment that will be visible to other users once the review is submitted
	"githubPullRequests.defaultCommentType": "single",

	// The create option that the "Create" button will default to when creating a pull request.
	//  - lastUsed: The most recently used create option.
	//  - create: The pull request will be created.
	//  - createDraft: The pull request will be created as a draft.
	//  - createAutoMerge: The pull request will be created with auto-merge enabled. The merge method selected will be the default for the repo or the value of `githubPullRequests.defaultMergeMethod` if set.
	"githubPullRequests.defaultCreateOption": "lastUsed",

	// When true, the option to delete the local branch will be selected by default when deleting a branch from a pull request.
	"githubPullRequests.defaultDeletionMethod.selectLocalBranch": true,

	// When true, the option to delete the remote will be selected by default when deleting a branch from a pull request.
	"githubPullRequests.defaultDeletionMethod.selectRemote": true,

	// The method to use when merging pull requests.
	"githubPullRequests.defaultMergeMethod": "merge",

	// Enables the `@githubpr` Copilot chat participant in the chat view. `@githubpr` can help search for issues and pull requests, suggest fixes for issues, and summarize issues, pull requests, and notifications.
	"githubPullRequests.experimental.chat": false,

	// Enables the notifications view, which shows a list of your GitHub notifications. When combined with `githubPullRequests.experimental.chat`, you can have Copilot sort and summarize your notifications.
	"githubPullRequests.experimental.notificationsView": false,

	// Controls whether the Copilot "Summarize" commands in the Pull Requests, Issues, and Notifications views will use quick chat. Only has an effect if `githubPullRequests.experimental.chat` is enabled.
	"githubPullRequests.experimental.useQuickChat": false,

	// The layout to use when displaying changed files list.
	"githubPullRequests.fileListLayout": "tree",

	// The layout to use when a pull request is checked out. Set to false to prevent layout changes.
	"githubPullRequests.focusedMode": "multiDiff",

	// Prevents branches that are associated with a pull request from being automatically detected. This will prevent review mode from being entered on these branches.
	"githubPullRequests.ignoredPullRequestBranches": [],

	// The setting `githubPullRequests.includeRemotes` has been deprecated. Use `githubPullRequests.remotes` to configure what remotes are shown.
	// By default we only support remotes created by users. If you want to see pull requests from remotes this extension created for pull requests, change this setting to 'all'.
	"githubPullRequests.includeRemotes": "default",

	// Group of labels that you want to add to the pull request automatically. Labels that don't exist in the repository won't be added.
	"githubPullRequests.labelCreated": [],

	// Log level is now controlled by the [Developer: Set Log Level...](command:workbench.action.setLogLevel) command. You can set the log level for the current session and also the default log level from there.
	// Logging for GitHub Pull Request extension. The log is emitted to the output channel named as GitHub Pull Request.
	"githubPullRequests.logLevel": "info",

	// Never offer to ignore a pull request associated with the default branch of a repository.
	"githubPullRequests.neverIgnoreDefaultBranch": false,

	// If GitHub notifications should be shown to the user.
	"githubPullRequests.notifications": "off",

	// The default branch for a repository is set on github.com. With this setting, you can override that default with another branch.
	"githubPullRequests.overrideDefaultBranch": "",

	// The action to take after creating a pull request.
	//  - none: No action
	//  - openOverview: Open the overview page of the pull request
	//  - checkoutDefaultBranch: Checkout the default branch of the repository
	//  - checkoutDefaultBranchAndShow: Checkout the default branch of the repository and show the pull request in the Pull Requests view
	//  - checkoutDefaultBranchAndCopy: Checkout the default branch of the repository and copy a link to the pull request to the clipboard
	"githubPullRequests.postCreate": "openOverview",

	// Pull changes from the remote when a PR branch is checked out locally. Changes are detected when the PR is manually refreshed and during periodic background updates.
	//  - prompt: Prompt to pull a PR branch when changes are detected in the PR.
	//  - never: Never pull a PR branch when changes are detected in the PR.
	//  - always: Always pull a PR branch when changes are detected in the PR. When `"git.autoStash": true` this will instead `prompt` to prevent unexpected file changes.
	"githubPullRequests.pullBranch": "prompt",

	// Controls whether the pull request branch is pulled before checkout. Can also be set to additionally merge updates from the base branch.
	//  - never: Never pull the pull request branch before checkout.
	//  - pull: Pull the pull request branch before checkout.
	//  - pullAndMergeBase: Pull the pull request branch before checkout, fetch the base branch, and merge the base branch into the pull request branch.
	//  - pullAndUpdateBase: Pull the pull request branch before checkout, fetch the base branch, merge the base branch into the pull request branch, and finally push the pull request branch to the remote.
	"githubPullRequests.pullPullRequestBranchBeforeCheckout": "pull",

	// The description used when creating pull requests.
	//  - template: Use a pull request template and commit description, or just use the commit description if no templates were found
	//  - commit: Use the latest commit message only
	//  - none: Do not have a default description
	//  - Copilot: Generate a pull request title and description from GitHub Copilot. Requires that the GitHub Copilot extension is installed and authenticated. Will fall back to `commit` if Copilot is not set up.
	"githubPullRequests.pullRequestDescription": "template",

	// The pull request title now uses the same defaults as GitHub, and can be edited before create.
	// The title used when creating pull requests.
	//  - commit: Use the latest commit message
	//  - branch: Use the branch name
	//  - custom: Specify a custom title
	//  - ask: Ask which of the above methods to use
	"githubPullRequests.pullRequestTitle": "ask",

	// Push the "from" branch when creating a PR and the "from" branch is not available on the remote.
	//  - prompt: Prompt to push the branch when creating a PR and the "from" branch is not available on the remote.
	//  - always: Always push the branch when creating a PR and the "from" branch is not available on the remote.
	"githubPullRequests.pushBranch": "prompt",

	// Specifies what queries should be used in the GitHub Pull Requests tree. All queries are made against **the currently opened repos**. Each query object has a `label` that will be shown in the tree and a search `query` using [GitHub search syntax](https://help.github.com/en/articles/understanding-the-search-syntax). The following variables can be used: 
	//  - `${user}` will resolve to the currently logged in user 
	//  - `${owner}` will resolve to the owner of the current repository, ex. `microsoft` in `microsoft/vscode` 
	//  - `${repository}` will resolve to the repository name, ex. `vscode` in `microsoft/vscode` 
	//  - `${today-Nd}`, where `N` is the number of days ago, will resolve to a date, ex. `2025-01-04`. 
	// 
	//  By default these queries define the categories "Waiting For My Review", "Assigned To Me" and "Created By Me". If you want to preserve these, make sure they are still in the array when you modify the setting.
	"githubPullRequests.queries": [
		{
			"label": "Waiting For My Review",
			"query": "repo:${owner}/${repository} is:open review-requested:${user}"
		},
		{
			"label": "Assigned To Me",
			"query": "repo:${owner}/${repository} is:open assignee:${user}"
		},
		{
			"label": "Created By Me",
			"query": "repo:${owner}/${repository} is:open author:${user}"
		}
	],

	// Enables quick diff in the editor gutter for checked-out pull requests. Requires a reload to take effect
	"githubPullRequests.quickDiff": false,

	// List of remotes, by name, to fetch pull requests from.
	"githubPullRequests.remotes": [
		"origin",
		"upstream"
	],

	// Use the setting 'githubPullRequests.defaultCreateOption' instead.
	// Checks the "Auto-merge" checkbox in the "Create Pull Request" view.
	"githubPullRequests.setAutoMerge": false,

	// This setting is deprecated. Views can now be dragged to any location.
	// When true, show GitHub Pull Requests within the SCM viewlet. Otherwise show a separate view container for them.
	"githubPullRequests.showInSCM": false,

	// Shows the pull request number in the tree view.
	"githubPullRequests.showPullRequestNumberInTree": false,

	// Default handler for terminal links.
	//  - github: Create the pull request on GitHub
	//  - vscode: Create the pull request in VS Code
	//  - ask: Ask which method to use
	"githubPullRequests.terminalLinksHandler": "ask",

	// Controls whether an `upstream` remote is automatically added for forks
	//  - add: An `upstream` remote will be automatically added for forks
	//  - never: An `upstream` remote will never be automatically added for forks
	"githubPullRequests.upstreamRemote": "add",

	// Choose which pull request states will use review mode. "Open" pull requests will always use review mode. Setting to "auto" will use review mode for open, closed, and merged pull requests in web, but only open pull requests on desktop.
	"githubPullRequests.useReviewMode": "auto",

	// When debugging only step through user-written code. Disable this to allow stepping into library code.
	"debugpy.debugJustMyCode": true,

	// Whether to display inline values in the editor while debugging.
	"debugpy.showPythonInlineValues": false,

	// Path to the State Tool executable for ActiveState runtimes (version 0.36+).
	"python.activeStateToolPath": "state",

	// List of paths to libraries and the like that need to be imported by auto complete engine. E.g. when using Google App SDK, the paths are not in system path, hence need to be added into this list.
	"python.autoComplete.extraPaths": [],

	// Path to the conda executable to use for activation (version 4.4+).
	"python.condaPath": "",

	// Show or hide Create Environment button in the editor for `requirements.txt` or other dependency files.
	"python.createEnvironment.contentButton": "hide",

	// Detect if environment creation is required for the current project
	"python.createEnvironment.trigger": "prompt",

	// Path to default Python to use when extension loads up for the first time, no longer used once an interpreter is selected for the workspace. See [here](https://aka.ms/AAfekmf) to understand when this is used
	"python.defaultInterpreterPath": "python",

	// Absolute path to a file containing environment variable definitions.
	"python.envFile": "${workspaceFolder}/.env",

	// Enables A/B tests experiments in the Python extension. If enabled, you may get included in proposed enhancements and/or features.
	"python.experiments.enabled": true,

	// List of experiments to opt into. If empty, user is assigned the default experiment groups. See [here](https://github.com/microsoft/vscode-python/wiki/AB-Experiments) for more details.
	"python.experiments.optInto": [],

	// List of experiments to opt out of. If empty, user is assigned the default experiment groups. See [here](https://github.com/microsoft/vscode-python/wiki/AB-Experiments) for more details.
	"python.experiments.optOutFrom": [],

	// Whether to install Python modules globally when not using an environment.
	"python.globalModuleInstallation": false,

	// Controls when to display information of selected interpreter in the status bar.
	//  - never: Never display information.
	//  - onPythonRelated: Only display information if Python-related files are opened.
	//  - always: Always display information.
	"python.interpreter.infoVisibility": "onPythonRelated",

	// Defines type of the language server.
	//  - Default: Automatically select a language server: Pylance if installed and available, otherwise fallback to Jedi.
	//  - Jedi: Use Jedi behind the Language Server Protocol (LSP) as a language server.
	//  - Pylance: Use Pylance as a language server.
	//  - None: Disable language server capabilities.
	"python.languageServer": "Default",

	// [Experimental] Select implementation of environment locators. This is an experimental setting while we test native environment location.
	"python.locator": "native",

	// This setting is deprecated. Please use command `Developer: Set Log Level...` to set logging level.
	// The logging level the extension logs at, defaults to 'error'
	"python.logging.level": "error",

	// Set severity of missing packages in requirements.txt or pyproject.toml
	"python.missingPackage.severity": "Hint",

	// Path to the pipenv executable to use for activation.
	"python.pipenvPath": "pipenv",

	// Path to the pixi executable.
	"python.pixiToolPath": "pixi",

	// Path to the poetry executable.
	"python.poetryPath": "poetry",

	// Toggle Smart Send for the Python REPL. Smart Send enables sending the smallest runnable block of code to the REPL on Shift+Enter and moves the cursor accordingly.
	"python.REPL.enableREPLSmartSend": true,

	// Toggle to provide variables for the REPL variable view for the native REPL.
	"python.REPL.provideVariables": true,

	// Toggle to send code to Python REPL instead of the terminal on execution. Turning this on will change the behavior for both Smart Send and Run Selection/Line in the Context Menu.
	"python.REPL.sendToNativeREPL": false,

	// Activate Python Environment in the current Terminal on load of the Extension.
	"python.terminal.activateEnvInCurrentTerminal": false,

	// Activate Python Environment in all Terminals created.
	"python.terminal.activateEnvironment": true,

	// When executing a file in the terminal, whether to use execute in the file's directory, instead of the current open folder.
	"python.terminal.executeInFileDir": false,

	// When launching a python terminal, whether to focus the cursor on the terminal.
	"python.terminal.focusAfterLaunch": false,

	// Python launch arguments to use when executing a file in the terminal.
	"python.terminal.launchArgs": [],

	// Enable [shell integration](https://code.visualstudio.com/docs/terminal/shell-integration) for the terminals running python. Shell integration enhances the terminal experience by enabling command decorations, run recent command, improving accessibility among other things.
	"python.terminal.shellIntegration.enabled": false,

	// Enable auto run test discovery when saving a test file.
	"python.testing.autoTestDiscoverOnSaveEnabled": true,

	// Glob pattern used to determine which files are used by autoTestDiscoverOnSaveEnabled.
	"python.testing.autoTestDiscoverOnSavePattern": "**/*.py",

	// Optional working directory for tests.
	"python.testing.cwd": null,

	// Port number used for debugging of tests.
	"python.testing.debugPort": 3000,

	// Prompt to configure a test framework if potential tests directories are discovered.
	"python.testing.promptToConfigure": true,

	// Arguments passed in. Each argument is a separate item in the array.
	"python.testing.pytestArgs": [],

	// Enable testing using pytest.
	"python.testing.pytestEnabled": false,

	// Path to pytest. You can use a custom version of pytest by modifying this setting to include the full path.
	"python.testing.pytestPath": "pytest",

	// Arguments passed in. Each argument is a separate item in the array.
	"python.testing.unittestArgs": [
		"-v",
		"-s",
		".",
		"-p",
		"*test*.py"
	],

	// Enable testing using unittest.
	"python.testing.unittestEnabled": false,

	// Folders in your home directory to look into for virtual environments (supports pyenv, direnv and virtualenvwrapper by default).
	"python.venvFolders": [],

	// Path to folder with a list of Virtual Environments (e.g. ~/.pyenv, ~/Envs, ~/.virtualenvs).
	"python.venvPath": "",

	// Enable/disable AI-assisted code actions. Requires the Copilot Chat extension to be enabled.
	"python.analysis.aiCodeActions": {},

	// When typing a `{` in a string, automatically prefix the string with an `f`.
	"python.analysis.autoFormatStrings": false,

	// Enable auto-import completions.
	"python.analysis.autoImportCompletions": false,

	// Automatically adjust indentation based on language semantics when typing Python code.
	"python.analysis.autoIndent": true,

	// Automatically add common search paths like `src`.
	"python.analysis.autoSearchPaths": true,

	// Cache LSP data for faster completions. 
	// 
	// [Experimental] may cause Pylance to stop working.
	"python.analysis.cacheLSPData": false,

	// Add parentheses to function completions.
	"python.analysis.completeFunctionParens": false,

	// Analysis scope for showing diagnostics.
	//  - openFilesOnly: Analyzes and reports errors on only open files.
	//  - workspace: Analyzes and reports errors on all files in the workspace.
	"python.analysis.diagnosticMode": "openFilesOnly",

	// Allows a user to override the severity levels for individual diagnostics. 
	// 
	// Use the rule name as a key and one of `error`, `warning`, `information`, `none`, `true` (alias for `error`) or `false` (alias for `none`) as value. The default value shown for each diagnostic is the default when #python.analysis.typeCheckingMode# is set to `off`. See [here](https://github.com/microsoft/pyright/blob/main/docs/configuration.md#diagnostic-rule-defaults) for defaults for each type checking mode (`off`, `basic` and `strict`).
	"python.analysis.diagnosticSeverityOverrides": {},

	// Disable hint diagnostics with special hints for grayed-out or strike-through text.
	"python.analysis.disableTaggedHints": false,

	// Display diagnostics in English regardless of VS Code's display language.
	"python.analysis.displayEnglishDiagnostics": false,

	// Enable support for editable installs of packages as described in [PEP 660](https://peps.python.org/pep-0660/) when using Python 3.13 and higher. 
	// 
	// [Experimental]. For internal use only, may cause Pylance to stop working.
	"python.analysis.enableEditableInstalls": false,

	// Enable/disable experimental server. For internal use only, may cause Pylance to stop working.
	"python.analysis.enableExperimentalServer": false,

	// Enables internal perf telemetry if telemetry is enabled in VS Code.
	"python.analysis.enablePerfTelemetry": false,

	// Enables pytest support in Pylance.
	"python.analysis.enablePytestSupport": true,

	// Use sync server mode [Experimental]. For internal use only, may cause Pylance to stop working.
	"python.analysis.enableSyncServer": false,

	// Paths of directories or files that should not be included. These override the include directories, allowing specific subdirectories to be excluded. 
	// 
	// Note that files in the exclude paths may still be included in the analysis if they are referenced (imported) by source files that are not excluded. 
	// 
	// Paths may contain wildcard characters `**` (a directory or multiple levels of directories), `*` (a sequence of zero or more characters), or `?` (a single character). 
	// 
	// If no exclude paths are specified, Pylance automatically excludes the following: `**/node_modules`, `**/__pycache__`, `.git` and any virtual environment directories. If the path contains a `${workspaceFolder:<workspaceName>}` variable, the glob pattern will only apply to the corresponding workspace in a multi-root workspace environment.
	"python.analysis.exclude": [],

	// Allow using '.', '(' as commit characters when applicable.
	"python.analysis.extraCommitChars": false,

	// Additional import search resolution paths
	"python.analysis.extraPaths": [],

	// source fixes to run in fix all.
	"python.analysis.fixAll": [],

	// Add type annotations when generating code. Defaults to `false` for type checking mode `off`, and `true` for other modes.
	"python.analysis.generateWithTypeAnnotation": false,

	// For string literals that look like module names, enables go to definition to go to the module.
	"python.analysis.gotoDefinitionInStringLiteral": true,

	// Paths of directories or files whose diagnostic output (errors and warnings) should be suppressed even if they are an included file or within the transitive closure of an included file. 
	// 
	// Paths may contain wildcard characters `**` (a directory or multiple levels of directories), `*` (a sequence of zero or more characters), or `?` (a single character). 
	// 
	// If the path contains a `${workspaceFolder:<workspaceName>}` variable, the glob pattern will only apply to the corresponding workspace in a multi-root workspace environment.
	"python.analysis.ignore": [],

	// Defines the default format for importing modules.
	//  - absolute: Use absolute import format when creating new import statement.
	//  - relative: Use relative import format when creating new import statement.
	"python.analysis.importFormat": "absolute",

	// Paths of directories or files that should be included. If no paths are specified, Pylance defaults to the workspace root directory. 
	// 
	// Paths may contain wildcard characters `**` (a directory or multiple levels of directories), `*` (a sequence of zero or more characters), or `?` (a single character). 
	// 
	// If the path contains a `${workspaceFolder:<workspaceName>}` variable, the glob pattern will only apply to the corresponding workspace in a multi-root workspace environment.
	"python.analysis.include": [],

	// Include alias symbols from user files. This will make alias symbols to show up in features such as `add import`, `auto import`
	"python.analysis.includeAliasesFromUserFiles": false,

	// Enable indexing of installed third party libraries and user files for language features such as auto-import, add import, workspace symbols and etc.
	"python.analysis.indexing": true,

	// Enable/disable inlay hints for call argument names:
	// ```python
	// datetime('year='2019, 'month='10, 'day='27)
	// ```
	// 
	//  - off: Disable inlay hints for call argument names.
	//  - partial: Enable inlay hints for positional-or-keyword arguments while ignoring positional-only and keyword-only.
	//  - all: Enable inlay hints for positional-or-keyword and positional-only arguments while ignoring keyword-only.
	"python.analysis.inlayHints.callArgumentNames": "off",

	// Enable/disable inlay hints for function return types:
	// ```python
	// def foo(x:int) '-> int':
	// 	return x
	// ```
	// 
	"python.analysis.inlayHints.functionReturnTypes": false,

	// Enable/disable inlay hints for pytest function parameter types:
	// ```python
	// def test_foo(my_fixture: 'str'):
	// 	assert(my_fixture == 'foo')
	// ```
	// 
	"python.analysis.inlayHints.pytestParameters": false,

	// Enable/disable inlay hints for variable types. Hints are not displayed for assignments of literals or constants:
	// ```python
	// foo':list[str]' = ["a"]
	//  
	// ```
	// 
	"python.analysis.inlayHints.variableTypes": false,

	// Select a predefined set of values for settings. Please check [this link](https://aka.ms/languageserver-mode) for more details.
	//  - light: Set Pylance to do only essential work to make it light weight. See the link at the description to find out exactly what settings are set to what value.
	//  - default: Leave Pylance with default settings.
	//  - full: Enable most Pylance features by default. See the link at the description to find out exactly what settings are set to what value.
	"python.analysis.languageServerMode": "default",

	// Specifies the level of logging for the Output panel
	"python.analysis.logLevel": "Information",

	// Path to a Node.js executable to use for running the language server. If not specified, the language server will use the Node.js executable that ships with VS Code. Set this option if you're having trouble with Pylance running out of memory. See [here](https://aka.ms/AApf7ox) for more information.
	"python.analysis.nodeExecutable": "",

	// Used to override how many levels under installed packages to index on a per package basis. By default, only top-level modules are indexed (depth = 1). To index submodules, increase depth by 1 for each level of submodule you want to index. Accepted values are:
	// ```JSON
	// {"name": "package name (str)",
	//  "depth": "depth to scan (int)",
	//  "includeAllSymbols": "whether to include all symbols (bool)"}
	// 
	// ```
	// If `includeAllSymbols` is set to `false`, only symbols in each package's `__all__` are included. When it's set to `true`, Pylance will index every module/top level symbol declarations in the file.  
	//   
	// Usage example: 
	// ```JSON
	// [
	// 	{"name": "sklearn", "depth": 2, "includeAllSymbols": true},
	// 	{"name": "matplotlib", "depth": 3, "includeAllSymbols": false}
	// ]
	// 
	// ```
	// 
	"python.analysis.packageIndexDepths": [
		{
			"name": "sklearn",
			"depth": 2
		},
		{
			"name": "matplotlib",
			"depth": 2
		},
		{
			"name": "scipy",
			"depth": 2
		},
		{
			"name": "django",
			"depth": 2
		},
		{
			"name": "flask",
			"depth": 2
		},
		{
			"name": "fastapi",
			"depth": 2
		}
	],

	// Indices for all third party libraries will be persisted to disk.
	"python.analysis.persistAllIndices": true,

	// Instead of relying on the shared stdlib.json indices for all Python versions, generate unique indices tailored to each workspace's specific Python version and platform. This regeneration process will affect performance, unlike using the prebuilt stdlib indices.
	"python.analysis.regenerateStdLibIndices": false,

	// Report extra telemetry [Experimental]. For internal use only, may cause Pylance to slow down.
	"python.analysis.reportExtraTelemetry": false,

	// Show only direct dependencies declared in `requirements.txt` or `pyproject.toml` in `auto import` suggestions, if they exist. This only affects `auto import` for completions. The `add import` code action will continue to show all possible imports.
	"python.analysis.showOnlyDirectDependenciesInAutoImport": false,

	// Path to directory containing custom type stub files.
	"python.analysis.stubPath": "typings",

	// Enable/disable support for docstring generation. In a blank docstring, use `Ctrl+Space` to generate a docstring.
	"python.analysis.supportDocstringTemplate": false,

	// Enable/disable support for reStructuredText in docstrings.
	"python.analysis.supportRestructuredText": true,

	// Type checking modes Basic, Standard, and Strict :
	// 
	// | Feature                                  | Basic | Standard | Strict |
	// |------------------------------------------|:-----:|:--------:|:------:|
	// | Variable type mismatches                 |   ✅   |    ✅     |   ✅   |
	// | Function return type checks              |   ✅   |    ✅     |   ✅   |
	// | Type narrowing enforcement               |       |    ✅     |   ✅   |
	// | Checking of `Any` type                   |       |    ✅     |   ✅   |
	// | Private/protected access checks          |       |    ✅     |   ✅   |
	// | Enforces stricter generics usage         |       |    ✅     |   ✅   |
	// | Reports missing type annotations         |       |          |   ✅   |
	// | Disallows `Any` type usage               |       |          |   ✅   |
	// | Requires strict type compatibility       |       |          |   ✅   |
	// | Enforces complete type coverage          |       |          |   ✅   |
	// 
	// For more details, check the [Pyright documentation](https://microsoft.github.io/pyright/#/configuration?id=type-check-diagnostics-settings).
	//  - off: Show diagnostics for invalid syntax, unresolved imports, undefined variables.
	//  - basic: All rules from `off` + `basic` type checking rules.
	//  - standard: All rules from `basic` + `standard` type checking rules.
	//  - strict: All rules from `standard` + `strict` type checking rules.
	"python.analysis.typeCheckingMode": "off",

	// Analyze and report errors for functions and methods that have no type annotations for input parameters or return types. The default value for this setting is `true`.
	"python.analysis.typeEvaluation.analyzeUnannotatedFunctions": true,

	// [PEP 585](https://peps.python.org/pep-0585) indicates that aliases to types in standard collections that were introduced solely to support generics are deprecated as of Python 3.9. This switch controls whether these are treated as deprecated. This applies only when pythonVersion is 3.9 or newer. The default value for this setting is `false` but may be switched to `true` in the future.
	"python.analysis.typeEvaluation.deprecateTypingAliases": false,

	// Disables legacy behavior where `bytearray` and `memoryview` are considered subtypes of `bytes`. [PEP 688](https://peps.python.org/pep-0688/#no-special-meaning-for-bytes) deprecates this behavior, but this switch is provided to restore the older behavior. The default value for this setting is `false`.
	"python.analysis.typeEvaluation.disableBytesTypePromotions": false,

	// Enables a set of experimental (mostly undocumented) features that correspond to proposed or exploratory changes to the Python typing standard. These features will likely change or be removed, so they should not be used except for experimentation purposes. The default value for this setting is `false`.
	"python.analysis.typeEvaluation.enableExperimentalFeatures": false,

	// If enabled, code that is determined to be unreachable by type analysis is reported using a tagged hint. This setting does not affect code that is determined to be unreachable regardless of type analysis; such code is always reported as unreachable. This setting also has no effect when when using the command-line version of pyright because it never emits tagged hints for unreachable code.
	"python.analysis.typeEvaluation.enableReachabilityAnalysis": false,

	// [PEP 484](https://peps.python.org/pep-0484) defines support for `# type: ignore` comments. This switch enables or disables support for these comments. The default value for this setting is `true`. This does not affect `# pyright: ignore` comments.
	"python.analysis.typeEvaluation.enableTypeIgnoreComments": true,

	// When inferring the type of a dictionary’s keys and values, use strict type assumptions. For example, the expression 
	// 
	// ```python
	// {'a': 1, 'b': 'a'}
	// ```
	//  could be inferred to be of type `dict[str, Any]` or `dict[str, int | str]`. If this setting is true, it will use the latter (stricter) type. The default value for this setting is `false`.
	"python.analysis.typeEvaluation.strictDictionaryInference": false,

	// When inferring the type of a list, use strict type assumptions. For example, the expression 
	// 
	// ```python
	// [1, 'a', 3.4]
	// ```
	//  could be inferred to be of type `list[Any]` or `list[int | str | float]`. If this setting is true, it will use the latter (stricter) type. The default value for this setting is `false`.
	"python.analysis.typeEvaluation.strictListInference": false,

	// [PEP 484](https://peps.python.org/pep-0484) indicates that when a function parameter is assigned a default value of None, its type should implicitly be Optional even if the explicit type is not. When enabled, this rule requires that parameter type annotations use Optional explicitly in this case. The default value for this setting is `true`.
	"python.analysis.typeEvaluation.strictParameterNoneValue": true,

	// When inferring the type of a set, use strict type assumptions. For example, the expression 
	// 
	// ```python
	// {1, 'a', 3.4}
	// ```
	//  could be inferred to be of type `set[Any]` or `set[int | str | float]`. If this setting is true, it will use the latter (stricter) type. The default value for this setting is `false`.
	"python.analysis.typeEvaluation.strictSetInference": false,

	// Paths to look for typeshed modules.
	"python.analysis.typeshedPaths": [],

	// Use library implementations to extract type information when type stub is not present.
	"python.analysis.useLibraryCodeForTypes": true,

	// Enable/disable support for pulling diagnostics from Pylance (instead of Pylance pushing them). 
	// 
	// [Experimental], may cause diagnostics to not appear. 
	// 
	// Requires restarting VS Code when changed.
	"python.analysis.usePullDiagnostics": false,

	// Maximum number of user files to index in the workspace. Indexing files is a performance-intensive task. Please use this setting to limit the number of files you want us to index. If you enter -1, we will index all files.
	"python.analysis.userFileIndexingLimit": 2000,

	// Note: If it is not Null, It will override CustomBrowser and ChromeDebuggingAttachment settings.
	// 
	//  Examples : 
	// chrome --incognito --headless --remote-debugging-port=9222 
	//  C:\\Program Files\\Firefox Developer Edition\\firefox.exe --private-window
	"liveServer.settings.AdvanceCustomBrowserCmdLine": null,

	// Enable Chrome Debugging Attachment to Live Server at Debuging Port 9222.
	//  NOTE: You have to install 'Debugger for Chrome' 
	// If the value is true, Select 'Attach to Chrome' from Debug Window to start debugging. 
	// 
	//  CAUTION: If it is true, 'Launch Chrome against localhost' may not work.
	"liveServer.settings.ChromeDebuggingAttachment": false,

	// Specify custom browser settings for Live Server. 
	// By Default it will open your default favorite browser.
	"liveServer.settings.CustomBrowser": null,

	// To disable information pop up messages.
	"liveServer.settings.donotShowInfoMsg": false,

	// To turn off prompt warning message if body or head or other supporting tag is missing in your HTML.
	"liveServer.settings.donotVerifyTags": false,

	// When set, serve this file (server root relative) for every 404 (useful for single-page applications)
	"liveServer.settings.file": "",

	// By Default Live Server inject CSS changes without full reloading of browser. You can change this behavior by making this setting as `true`
	"liveServer.settings.fullReload": false,

	// To switch between localhost or 127.0.0.1 or anything else. Default is 127.0.0.1
	"liveServer.settings.host": "127.0.0.1",

	// Setup https configuration
	"liveServer.settings.https": {
		"enable": false,
		"cert": "",
		"key": "",
		"passphrase": ""
	},

	// To ignore specific file changes
	"liveServer.settings.ignoreFiles": [
		".vscode/**",
		"**/*.scss",
		"**/*.sass",
		"**/*.ts"
	],

	// Mount a directory to a route. Such as [['/components', './node_modules']]
	"liveServer.settings.mount": [],

	// This the entry point of server when you're in multiroot workspace
	"liveServer.settings.multiRootWorkspaceName": null,

	// If it is true live server will start without browser opened.
	"liveServer.settings.NoBrowser": false,

	// Set Custom Port Number of Live Server. Set 0 if you want random port.
	"liveServer.settings.port": 5500,

	// To Setup Proxy
	"liveServer.settings.proxy": {
		"enable": false,
		"baseUri": "/",
		"proxyUri": "http://127.0.0.1:80"
	},

	// Set Custom root of Live Server. 
	// To change root the the server to sub folder of workspace, use '/' and relative path from workspace. 
	// Example: /subfolder1/subfolder2
	"liveServer.settings.root": "/",

	// Change this to false if you don't want the button to show in the statusbar
	"liveServer.settings.showOnStatusbar": true,

	// Use local IP as host
	"liveServer.settings.useLocalIp": false,

	// You have to install a browser extension. That will be works for your dynamic pages (like PHP).
	"liveServer.settings.useWebExt": false,

	// Delay before live reloading. Value in milliseconds. Default is 100
	"liveServer.settings.wait": 100,

	// Defines scopes for extension to work with.
	// multi-root: all selectors found within all root folders will be visible to all stylesheets.
	// workspace: all selectors found within particular workspace folder/project will be visible to stylesheets within that workspace folder.
	// linked files: selectors will be provided only for linked stylesheets.
	// Default: "multi-root"
	"html-to-css-autocompletion.autocompletionFilesScope": "multi-root",

	// Set custom glob pattern to exclude search on pattern matches. E.g.: **/{folderName1,folderName2,...}/**
	"html-to-css-autocompletion.excludePattern": "",

	// Defines folder names to be excluded from being searched. Default: ["node_modules"]
	"html-to-css-autocompletion.folderNamesToBeExcluded": [
		"node_modules"
	],

	// Defines only specific folder names to be searched. Default: [""]
	"html-to-css-autocompletion.folderNamesToBeIncluded": [
		""
	],

	// Defines file types to be searched for classes/ids.
	// Defaults: ["html", "php"]
	"html-to-css-autocompletion.getSelectorsFromFileTypes": [
		"html",
		"php"
	],

	// Set custom glob pattern to get classes/ids from matched files. E.g.: **/{folderName1,folderName2,...}/*.{fileType1,fileType2,...}
	"html-to-css-autocompletion.includePattern": "",

	// Set true to populate Intellisense with selectors only when '#' or '.' characters are typed. Default: false
	"html-to-css-autocompletion.triggerCharacters": false,

	// Uses the legacy module resolving.
	"standard._legacyModuleResolve": false,

	// Turns auto fix on save on or off.
	"standard.autoFixOnSave": false,

	// Controls whether JavaScript Standard Style is enabled for JavaScript files or not.
	"standard.enable": true,

	// Controls whether JavaScript Standard Style is enabled globally for JavaScript files or not.
	"standard.enableGlobally": false,

	// Controls whether VSCode should use an alternate Standard engine, like semistandard, standardx or ts-standard.
	"standard.engine": "standard",

	// A path added to NODE_PATH when resolving the standard module.
	"standard.nodePath": null,

	// The standard options object to provide args normally passed to JavaScript Standard Style when executed from a command line.
	"standard.options": {},

	// Run the linter on save (onSave) or on type (onType)
	"standard.run": "onType",

	// Traces the communication between VSCode and the JavaScript Standard Style linter service.
	"standard.trace.server": "off",

	// Any linting error reported by Standard will instead be displayed as a warning within VS Code.
	"standard.treatErrorsAsWarnings": false,

	// Activate JavaScript Standard Style based on project's package.json settings, use globally installed standard module if set to "false"
	"standard.usePackageJson": true,

	// An array of language ids which should be validated by JavaScript Standard Style
	"standard.validate": [
		"javascript",
		"javascriptreact",
		"typescript",
		"typescriptreact"
	],

	// 
	"standard.workingDirectories": [],

	// Set default browser
	"open-in-browser.default": "",

	// Open a preview to the side automatically
	"svg.preview.autoOpen": false,

	// Show a bounding box around the preview image
	"svg.preview.boundingBox": false,

	// Show transparency grid
	"svg.preview.transparencyGrid": false,

}
