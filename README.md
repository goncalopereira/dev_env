# Gem install
bundle install

# Install Atom plugins
chmod +x Atom.sh
./Atom.sh

# Modify ~/.atom/config.cson based on local file

Use
''' $ rbenv which $gem '''
To find gem location

Example:

'''

"linter-foodcritic":
  executablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/foodcritic"
"linter-rubocop":
  command: "/usr/local/opt/rbenv/versions/2.3.1/bin/rubocop"
"linter-ruby":
  rubyExecutablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/ruby"
"rubocop-auto-correct":
  rubocopCommandPath: "/usr/local/opt/rbenv/versions/2.3.1/bin/rubocop"
'linter-reek':
  reekExecutablePath: "/usr/local/opt/rbenv/versions/2.3.1/bin/reek"


'''

# Modify ~/.atom/keymap.cson based on local file
'''

'atom-text-editor[data-grammar~="ruby"]':
  'alt-r': 'rubocop-auto-correct:current-file'

'''
