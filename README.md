# Sublime Text 3 Note

## Edit

#### Split selection
ctrl + shift + L

#### Warp selection in HTML tag
alt + shift + W

#### Move Line up/down
ctrl + shift + up / down

#### Copy line
ctrl + shift + D

#### Delete line
ctrl + shift + K

#### Indentation left/right
ctrl + [ / ]

#### Indentation paste
ctrl + shift + V

#### Console log command
ctrl + ` ; sublime.log_commands(True) + enter ; sublime.log_input(True)


## Search

#### Go to line
ctrl + G ; line-number + enter

#### Open/Close side file bar
ctrl + K + B;

#### Open go anything panel [anything-panel]
ctrl + P

#### Open file
[anything-panel] ; file-name + enter

#### Search Class in Javascript or CSS
[anything-panel] ; @class=name + enter

#### Search symbol in files
[anything-panel] ; #symbol + enter


## Command palette

#### Command palette
ctrl + shift + P

#### Usage
* selected context and do some edit, like uppercase and sort , reverse etc.
* encode in HTML file to make symbol safe encode.
* set syntax to set plain text style


## Add-ons

#### install packages
[command-palette] ; package control : install package ; package-name + enter

## Snippets

#### Usages
* Tool->Snippets -- show all available snippets in current language
* HTML can use Emmet package (it's magic)

###### Warp selection in HTML tag use Emmet
shift + ctrl + G ; sample in command line "li.day-$$>span"

###### Use Emmet create HTML fast way
sample snippet "(header.site-header>h1+nav>ul>li*5)+(div.site-body>div.main+aside.sidebar)+(footer.site-footer)"

* Use Emmet create CSS efficiently
###### Use snippet to finish code
sample "db" => "display: block;"; "tda" => "text-decoration: none;"; "mr10" => "margin-right: 10px;";
"mb15" => "margin-bottom: 15px;"; "p10" => "padding: 10px;"; "p10-20" = "padding: 10px 20px;";
"w85p" => "width: 85%;"

* Create a snippet
Tools->Developer->New Snippets... ; make your own snippet with template, this is a sample
```
<snippet>
	<content><![CDATA[
<div class="$1">
	Hello ${2:World}!
</div><!-- ${1/\*//} "/\*\\"is a Regular Expression to make mirror cursor disappear -->
]]></content>
	<tabTrigger>hello</tabTrigger>
	//whole valid scope in https://gist.github.com/iambibhas/4705378
	<scope>text.html</scope>
	<discription>Hello World</discription>
</snippet>
```

## Key bindings
Preferences->Key Bindings ; write shortcut in user file like bellow
```
[
	{"keys": ["ctrl+shift+f"], "command": "reindent"}
]
```

## Macros

#### Recording
ctrl + Q ; ctrl + Q ; Tools->Save Macro... ; Key Bindings =>
```
[
	{"keys": ["ctrl+alt+f"], "command": "reindent"},
	{"keys": ["alt+enter"], "command": "run_macro_file", "args": {"file": "Packages/User/auto_barcket.sublime-macro"}}
]
```

## Themes
* Use Material Theme in Package Control

#### Hide / Show menu bar
alt

#### Find setting in [command-palette]
[command-palette] ; "vmen" => "view: Toggle Menu" // Show / Hide menu bar

## User Setting
Preferences->Settings ; add lines
```
	"highlight_line": true,
	"caret_extra_width": 2,
	"caret_extra_top": 1,
	"caret_extra_bottom": 1,
	"line_padding_top": 1,
	"line_padding_bottom": 1,
 ```

## Add-ons list
* Trailing Spaces
* Material Theme
* Git
* GitGutter
* Color Highlighter
* Alignment
* Emmet
* SublimeLinter + jshint
* HTML/CSS/JS Prettify
* JavaScript Completions
* Webgl Completions
* BracketHighlighter


## Relate videos
[Youtube Video](https://www.youtube.com/watch?v=SVkR1ZkNusI&index=1&list=PLpcSpRrAaOaqQMDlCzE_Y6IUUzaSfYocK)
