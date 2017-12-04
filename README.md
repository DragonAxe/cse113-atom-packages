# cse113-atom-packages

Programming - Why Haskell is Great - 10 minutes
https://www.youtube.com/watch?v=RqvCNb7fKsg

To get rid of those pesky pop-up dock toggle buttons you can do this:
```
Settings -> Themes
Under "UI Theme" click the gear.
"Hide dock toggle buttons"
```

Here are the packages I use:

|Package:|From:|Purpose:|
|--------|-----|--------|
|advanced-open-file|Osmose|Open files with Ctrl+Alt+o|
|atom-beautify|Glavin001|Beautify code with uncrustify.cfg file|
|atom-overtype-mode|brunetton|Makes the insert button actually work|
|auto-indent-file|lucbu|Auto indent entire file|
|autocomplete-clang|yasuyuky|Autocompletions for C code|
|build|noseglid|Build your current project, directly from Atom|
|build-make|AtomBuild|Builds your makefile project. Requires 'build'.|
|chary-tree-view|h2so5|A better tree view side panel|
|docblockr|nikhilkalige|Doxygen helper|
|file-icons|DanBrooker|Colorful file icons|
|fold-functions|robballou|Collapses code blocks, i.e. functions so they don't take up space.|
|git-log|nikhilkalige|Fancy git tree viewer|
|git-plus|akonwl|Run git commands from within atom|
|language-x86-64-assembly|13xforever|Useful for CSE221|
|intensions|steelbrain|Base package for showing code completions|
|linter-ui-default|steelbrain|Needed for other linter packages|
|linter|atom-community|"A Base Linter with Cow Powers"|
|linter-clang|AtomLinter|Lint C source code|
|minimap|atom-minimap|A little preview of your entire source file|
|minimap-bookmarks|atom-minimap|Displays Atom bookmarks in the minimap|
|multi-cursor|joseramonc|Multiple cursors with {define your own keybinding}|
|nuclide|facebook|A UI overhaul that add IDE-like features.|
|symbols-tree-view|xndcn|A side bar that lists all the symbols (functions/variables) defined in the current file.|
|trailing-semicolon|pimartin|Adds or removes a semicolon or comma at end of line with ctrl+;|
|remote-sync|yongkangchen|scp/sftp/ftp sync between local machine and CS server. (May be currently broken)|

My Keymap file:
```
'atom-workspace':
  'alt-up': 'multi-cursor:expandUp'
  'alt-down': 'multi-cursor:expandDown'
'atom-text-editor':
  'ctrl-;': 'trailing-semicolon:semicolon'
```

My Snippets file:
```
'.source.c':
  'common-name':
    'prefix': 'command-name'
    'body': 'the code snippet to insert'
  'common-name2':
    'prefix': 'cstart'
    'body': """
multiline
code
snippet
    """
````

Disabled Atom Packages (for faster startup):
```
background-tips
language-csharp
language-go
language-mustache
language-objective-c
language-perl
language-ruby
language-ruby-on-rails
language-sass
```
