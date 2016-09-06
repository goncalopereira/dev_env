### Gem install
`bundle install`
# Install plugins

```
chmod +x Atom.sh
./Atom.sh

chmod +x NPM.sh
./NPM.sh

chmod +x Brew.sh
./Brew.sh
```

### Change ~/.atom/config.cson based on local file

Use `$ rbenv which $gem`
To find gem location

Example:

```
"linter-erb":
  erbExecutablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/erb"
  rubyExecutablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/ruby"
"linter-foodcritic":
  executablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/foodcritic"
  extraArgs: "-t correctness"
"linter-reek":
  reekExecutablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/reek"
"linter-rubocop":
  command: "/usr/local/opt/rbenv/versions/2.3.1/bin/rubocop"
"linter-ruby":
  ignoredExtensions: [
    "md"
  ]
  rubyExecutablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/ruby"
"linter-shellcheck": {}
"rubocop-auto-correct":
  rubocopCommandPath: "/usr/local/opt/rbenv/versions/2.3.1/bin/rubocop"
```

### Change ~/.atom/keymap.cson based on local file
```

'atom-text-editor[data-grammar~="ruby"]':
  'alt-r': 'rubocop-auto-correct:current-file'
'atom-text-editor[data-grammar~="ruby"]':
  'alt-e': 'ror-refactor:extract-code'

```

### Nice Theme
```
apm install atom-material-syntax
```
