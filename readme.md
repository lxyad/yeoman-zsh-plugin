# Yeoman plugin for (Oh My) ZSH

This is a [Yeoman](http://yeoman.io/) plugin for [Oh My ZSH](https://github.com/robbyrussell/oh-my-zsh), **compatible with _yeoman_ version `≥1.0`**.

It provides:
* aliases ;
* **zsh autocomplete** functions and options.

---

## Installation

### oh-my-zsh

If you're using [oh-my-zsh](github.com/robbyrussell/oh-my-zsh):

1. In the command line, change to _oh-my-zsh_'s custom plugin directory :

    ```
    cd ~/.oh-my-zsh/custom/plugins/
    ```
2. Clone the repository into a new `yo` directory:

    ```
    git clone https://github.com/lxyad/yo-zsh-plugin yo
    ```
3. Edit your `~/.zshrc` and add `yo` to the list of plugins:

    ```
    plugins=( ... yo )
    ```
4. Source your current shell configuration:

    ```
    source ~/.zshrc
    ```

---

### `yo` completion

The list of generators is built using the native [`--generators` option](https://github.com/yeoman/yo#options)  

#### List installed generators

```bash
$ yo<tab>
angular                          -- angular's generator
gulp-webapp                      -- gulp-webapp's generator
karma                            -- karma's generator
leaflet                          -- leaflet's generator
mocha                            -- mocha's generator
webapp                           -- Default Yeoman generator for scaffolding out a front-end web app
```

#### List of options

```bash
$ yo -<tab><tab>
--help             -- show the help message and quit
--version          -- show version information and quit
  --help         # Print this info and generator's options and usage
  -f, --force    # Overwrite files that already exist
  --version      # Print version
  --no-color     # Disable colors
  --[no-]insight # Toggle anonymous tracking
  --generators   # Print available generators

```

---

## Aliases (for _yeoman_)

Old aliases have been updated to *use new yeoman's `≥1.0` commands*, i.e. `yo`, `bower`, `grunt` :

* `ym...` prefix stand for `yeoman`:

    ```
    alias ymget='npm install -g yo grunt-cli bower'

    alias ym='yo help'
    alias ymv='yo --version'

    alias ymi='yo'
    alias ymb='grunt build'
    alias ymsv='grunt server'
    alias ymsd='grunt server:dist'
    alias ymst='grunt server:test'
    alias ymt='grunt test'
    alias ymii='bower install'
    alias ymui='bower uninstall'
    alias ymu='bower update'
    alias yml='bower list'
    alias yms='bower search'
    alias ymlu='bower lookup'
    ```
