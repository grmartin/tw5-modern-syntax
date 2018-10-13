# TW5 Modern Syntax

A drop in replacement for the Highlight.js plugin with an updated JS package and additional contemporary language types.

## Installation (for Node.js)

The following procedure relies on the fact that TW5 will always prefer a local tiddler to a global one and thus a plugin in your server's base path will always take priority.

1. Start up server (`tiddlywiki <path> --server`)
1. In Wiki Web enable the stock Highlight.js Plugin
1. Shutdown Server
1. Create a `plugins` folder at the root of your wiki path (same location as your `tiddlywiki.info` file)
1. Clone or Export this repo in to a folder named `highlight` under `plugins`
1. Restart your server

## From `readme.tid`

title: $:/plugins/tiddlywiki/highlight/readme

This plugin provides syntax highlighting of code blocks using v9.12.0 of [highlight.js](https://github.com/isagalaev/highlight.js) from Ivan Sagalaev.

### Usage

When the plugin is installed it automatically applies highlighting to all codeblocks defined with triple backticks or with the CodeBlockWidget.

The language can optionally be specified after the opening triple braces:

```css
 * { margin: 0; padding: 0; } /* micro reset */

html { font-size: 62.5%; }
body { font-size: 14px; font-size: 1.4rem; } /* =14px */
h1   { font-size: 24px; font-size: 2.4rem; } /* =24px */
```

If no language is specified highlight.js will attempt to automatically detect the language.

### Built-in Language Brushes

The plugin includes support for the following languages (referred to as "brushes" by highlight.js):

* ActionScript - as `actionscript`
* Apache - as `apache`
* AppleScript - as `applescript`
* ARM Assembly - as `armasm`
* Augmented Bacus-Naur - as `abnf`
* (Standard) Bacus-Naur - as `bnf`
* Bash - as `bash`
* C# - as `cs`
* C++ - as `cpp`
* CMake - as `cmake`
* CoffeeScript - as `coffeescript`
* CSS - as `css`
* D - as `d`
* Diff - as `diff`
* DNS Zone File - as `dns`
* DOS Batch - as `dos`
* Extended Bacus-Naur - as `ebnf`
* F# - as `fsharp`
* Go - as `go`
* Gradle - as `gradle`
* Handlebars - as `handlebars`
* Haxe - as `haxe`
* HTML, XML - as `xml`
* HTTP - as `http`
* Ini - as `ini`
* Intel x86 Assembly - as `x86asm`
* Java - as `java`
* JavaScript - as `javascript`
* JSON - as `json`
* Kotlin - as `kotlin`
* Lisp - as `lisp`
* LLVM IR - as `llvm`
* Lua - as `lua`
* Makefile - as `makefile`
* Markdown - as `markdown`
* Nginx - as `nginx`
* NSIS - as `nsis`
* Objective-C - as `objectivec`
* OCaml - as `ocaml`
* Perl - as `perl`
* PHP - as `php`
* PowerShell - as `powershell`
* Protocol Buffers - as `protobuf`
* Python - as `python`
* R - as `r`
* Ruby - as `ruby`
* Shell Session - as `shell`
* SQL - as `sql`
* Swift - as `swift`
* Twig - as `twig`
* TypeScript - as `typescript`
* Vim Script - as `vim`
* YAML - as `yaml`

You can also specify the language as a MIME content type (eg `text/html` or `text/css`). The mapping is accomplished via mapping tiddlers whose titles start with `$:/config/HighlightPlugin/TypeMappings/`.
