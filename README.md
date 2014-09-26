## Synopsis

Ultisnips snippet for bootstrap 3

## Process

### Original Source

These snippets were converted from Snipmate snippets created and shared by https://github.com/colbydehart

Original snipmate snippet can be found at https://github.com/colbydehart/Bootstrap-3-snippets-html

### Conversion

Conversion was performed thanks to subl2ultisnips https://github.com/rendom/Sublimetext-snippets-to-Ultisnips

### Process

The following commands were run to create the snippets

```bash
npm install -g subl2ultisnips
git clone https://github.com/colbydehart/Bootstrap-3-snippets-html.git
find . -type file -iname '*-snippet' -exec subl2ultisnips {} html_bootstrap_3.snippets \;
```

For some reason regulary expression transforms are not correctly converted, you will need to do a search and replace on the resulting snipets file using the following expression

```
s/\\1/$0/g
```

Using sed to fix the output

```bash
sed 's/\\1/$0/g' html_bootstrap_3.snippets
```


## Code Example

To create a login form simply perform the following actions

```
bs3-hello<tab>Ultisnips Is Awseome<tab>Login Form<tab>
bs3-container<tab>bs3-row<tab>bs3-col:12<tab>
bs3-form:horizontal<tab>login<tab><tab>Login<tab>
bs3-input:email:h<tab>email<tab><tab><tabe>Username<tab>
bs3-input:password:h<tab>password<tab><tab><tabe>Password<tab>

```

Output; see example.html

## Motivation

Provide an easy to use snippets library for UltiSnips

## Installation

Copy html_bootstrap_3.snippets to your personal snippets folder

## Tests

TBC


## License

A short snippet describing the license (MIT, Apache, etc.)
