# 俺流VSCode Settings

VScodeには「Japanese Language Pack」のように便利な拡張機能がたくさんあります。

そこで個人的なおすすめの拡張機能や設定ファイルを紹介します。

これでかなり開発がはかどるはず。キーボードのショットかっとを指定するとなお便利だと思いますよ！！

## おすすめ拡張機能

入れておいて損はないと思うオススメの拡張機能。

サイドバー（左に縦に並んでるアイコンたち）にある「拡張機能」のボタンから下記を検索してインストールしてみてください。

- Japanese Language Pack for Visual Studio Code
- Auto Rename Tag
- Autoprefixer
- CSS Peek
- Prettier - Code formatter
- stylelint
- Highlight Matching Tag
- Markuplint 
- IntelliSense for CSS class names in HTML
- Live Sass Compiler ****（作成者が「Glenn Marks」さんの方）****
- Live Server
- PostCSS Intellisense and Highlighting

## おすすめ設定

上記の拡張機能に関する設定を加えた設定ファイルです。

VSCodeの「settings」から右上の「設定（JSON）を開く」をクリックし、表示されるコードを全て消して下記のコードをコピー&ペーストしてください。

```json
{
  "files.autoSave": "onWindowChange",
  "files.autoGuessEncoding": true,
  "files.insertFinalNewline": true,
  "files.trimFinalNewlines": true,
  "files.trimTrailingWhitespace": true,
  "editor.fontSize": 16,
  "editor.wordWrap": "on",
  "editor.renderWhitespace": "all",
  "editor.fontFamily": "'SourceHanCodeJP-Medium','Source Han Code JP','Panic Sans', Menlo, Monaco, 'Courier New', monospace",
  "editor.formatOnSave": true,
  "editor.formatOnType": true,
  "editor.formatOnPaste": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[php]": {
    "editor.defaultFormatter": "bmewburn.vscode-intelephense-client"
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.stylelint": true,
    "source.fixAll": true
  },
  "editor.fontWeight": "500",
  "editor.tabSize": 2,
  "editor.renderLineHighlight": "all",
  "editor.renderControlCharacters": true,
  "editor.cursorBlinking": "smooth",
  "editor.snippetSuggestions": "top",
  "editor.suggestSelection": "first",
  "editor.smoothScrolling": true,
  "editor.minimap.showSlider": "always",
  "explorer.compactFolders": false,
  "window.openFoldersInNewWindow": "on",
  "window.title": "${activeEditorMedium}${separator}${rootName}",
  "window.commandCenter": true,
  "workbench.editor.untitled.hint": "hidden",
  "workbench.startupEditor": "none",
  "workbench.editor.labelFormat": "short",
  "workbench.editor.tabSizing": "shrink",
  "breadcrumbs.enabled": true,
  "html.autoClosingTags": false,
  "html.format.extraLiners": "",
  "html.format.maxPreserveNewLines": 2,
  "html.format.wrapLineLength": 0,
  "html.format.unformatted": null,
  "html.format.contentUnformatted": "pre, code, textarea, title, h1, h2, h3, h4, h5, h6, p",
  "git.ignoreMissingGitWarning": true,
  "emmet.showSuggestionsAsSnippets": true,
  "emmet.triggerExpansionOnTab": true,
  "emmet.variables": {
    "lang": "ja"
  },
  "emmet.includeLanguages": {
    "nunjucks": "html",
		"postcss": "css"
  },
  "files.associations": {
    "*.njk": "html"
  },
  "liveServer.settings.useLocalIp": true,
  "liveServer.settings.CustomBrowser": "chrome",
  "liveSassCompile.settings.generateMap": true,
  "liveSassCompile.settings.formats": [
    {
      "format": "expanded",
      "extensionName": ".css",
      "savePath": "~/../css"
    }
  ],
  "liveSassCompile.settings.autoprefix": ["> 0.5%", "last 2 versions", "Firefox ESR", "not dead"],
  "autoprefixer.options": {
    "overrideBrowserslist": ["> 0.5%", "last 2 versions", "Firefox ESR", "not dead"],
    "grid": "autoplace"
  },
  "diffEditor.ignoreTrimWhitespace": true,
  "html-css-class-completion.enableEmmetSupport": true,
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.lineHeight": 1.1,
  "scm.autoReveal": false,
  "less.validate": false,
  "scss.validate": false,
	"postcss.validate": false,
  "css.lint.important": "warning",
  "css.lint.zeroUnits": "warning",
  "css.validate": false,
  "stylelint.validate": ["css", "less", "postcss", "scss", "sass"],
  "prettier.printWidth": 200,
	// "php.validate.executablePath": "C:/xampp/php/php.exe", // XAMPP for Windows
	// "php.validate.executablePath": "/usr/bin/php", // Intel Mac
  "material-icon-theme.hidesExplorerArrows": true,
  "liveshare.launcherClient": "web",
  "intelephense.stubs": [
    "apache",
    "bcmath",
    "bz2",
    "calendar",
    "com_dotnet",
    "Core",
    "ctype",
    "curl",
    "date",
    "dba",
    "dom",
    "enchant",
    "exif",
    "FFI",
    "fileinfo",
    "filter",
    "fpm",
    "ftp",
    "gd",
    "gettext",
    "gmp",
    "hash",
    "iconv",
    "imap",
    "intl",
    "json",
    "ldap",
    "libxml",
    "mbstring",
    "meta",
    "mysqli",
    "oci8",
    "odbc",
    "openssl",
    "pcntl",
    "pcre",
    "PDO",
    "pdo_ibm",
    "pdo_mysql",
    "pdo_pgsql",
    "pdo_sqlite",
    "pgsql",
    "Phar",
    "posix",
    "pspell",
    "random",
    "readline",
    "Reflection",
    "session",
    "shmop",
    "SimpleXML",
    "snmp",
    "soap",
    "sockets",
    "sodium",
    "SPL",
    "sqlite3",
    "standard",
    "superglobals",
    "sysvmsg",
    "sysvsem",
    "sysvshm",
    "tidy",
    "tokenizer",
    "xml",
    "xmlreader",
    "xmlrpc",
    "xmlwriter",
    "xsl",
    "Zend OPcache",
    "zip",
    "zlib",
    "wordpress"
  ]
}
```

PHPを利用する場合は貼り付けたコードのコメント部分を自分のOSに合わせて、先頭にある「// （コメント）」を消す。

### Windows（XAMPP）

```json
// "php.validate.executablePath": "C:/xampp/php/php.exe", // Windows
```

 ↓

```json
"php.validate.executablePath": "C:/xampp/php/php.exe", // Windows
```

### Mac（Intel製）

```json
// "php.validate.executablePath": "/usr/bin/php", // Mac
```

↓ 

```json
"php.validate.executablePath": "/usr/bin/php", // Mac
```

詳細はブログにも書きました。

[https://shibajuku.net/vscode-plugin-settings/](https://l.facebook.com/l.php?u=https%3A%2F%2Fshibajuku.net%2Fvscode-plugin-settings%2F%3Ffbclid%3DIwAR0MCDnlWGcI5WTjpEV2SJxlr47SGIroLOKEJteTTPs4SbIwFv59nzhbNzk&h=AT3qN_lFPGc0yqX2fpchsNyJKPbzafrI3mTJhAE7A8oZP7ocuc-D-2weGGQdVLMcQM7D54G4qxSyuowhIJuDDWX1wxrqjsy1lM0YRC19LBCnxEgmPKoptk44AcWMp-GgGfaNLKzHB-A_pWV6nvpJY219-Iw)

## キーボードショートカットの設定

おすすめショートカットは、設定しておくと便利なおすすめのショートカットキーです。「左下の歯車」→「キーボードショートカット」から設定できます。

- Autoprefix CSS ： 自動でベンダープレフィックスをつけるctrl + shift + A （Macは ctrl を cmd に置換）
- 定義をここに表示：カーソルがあるHTMLの要素に指定されてるCSSをその場に表示 ctrl + E （Macは ctrl を cmd に置換）
- ラップ変換：Emmetで文章に対して要素をマークアップctrl + shift + W（Macは ctrl を cmd に置換）

