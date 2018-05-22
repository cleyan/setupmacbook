# Configuraciones Iniciales


# Configurar /Users/usuario/.config/fish/config.fish

set -g -x PATH /usr/local/bin $HOME/.composer/vendor/bin /usr/local/sbin $PATH

set -x GOPATH $HOME/Dropbox/Proyectos/go
set -xg PATH $PATH /usr/local/go/bin $GOPATH/bin

test -e {$HOME}/.iterm2_shell_integration.fish ; and source {$HOME}/.iterm2_shell_integration.fish
set -g fish_user_paths "/usr/local/opt/node/bin" $fish_user_paths
set -g fish_user_paths "/usr/local/opt/php@7.0/bin" $fish_user_paths
set -g fish_user_paths "/usr/local/opt/php@7.0/sbin" $fish_user_paths
set -g fish_user_paths "/usr/local/opt/php@7.1/bin" $fish_user_paths
set -g fish_user_paths "/usr/local/opt/php@7.1/sbin" $fish_user_paths

# The next line updates PATH for the Google Cloud SDK.
if [ -f '/Users/usuario/carpeta/google-cloud-sdk/path.fish.inc' ]; if type source > /dev/null; source '/Users/usuario/carpeta/google-cloud-sdk/path.fish.inc'; else; . '/Users/usuario/carpeta/google-cloud-sdk/path.fish.inc'; end; end

