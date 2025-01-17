# Ellama

[![License GPL 3](https://img.shields.io/badge/license-GPL_3-green.svg)](http://www.gnu.org/licenses/gpl-3.0.txt)
[![MELPA](https://melpa.org/packages/ellama-badge.svg)](https://melpa.org/#/ellama)

Ellama lets you access LLMs locally using
[ollama](https://github.com/jmorganca/ollama)'s API from Emacs. It
offers a set of commands that allow you to inquire, define words,
translate text and more through the Emacs interface. Ellama natively
supports streaming output, making it effortless to use with your
preferred text editor.

## Installation

Firstly, you need to install
[ollama](https://github.com/jmorganca/ollama) and pull
[zephyr](https://ollama.ai/library/zephyr) (default model) or any
other model from [library](https://ollama.ai/library) (in that case
you should customize `ellama-model`)
You can now install the package `ellama` from
[MELPA](https://melpa.org/#/getting-started). Just `M-x`
`package-install`<kbd>Enter</kbd> `ellama` <kbd>Enter</kbd>.

## Commands

### ellama-ask

Ask Ellama about something by entering a prompt in an interactive
buffer.
![ellama-ask](imgs/ellama-ask.gif)

### ellama-ask-about

Ask Ellama about a selected region or the current buffer.
![ellama-ask-about](imgs/ellama-ask-about.gif)

### ellama-translate

Ask Ellama to translate a selected region or word at the point.
![ellama-translate](imgs/ellama-translate.gif)

### ellama-define-word

Find the definition of the current word using Ellama.
![ellama-define-word](imgs/ellama-define-word.gif)

### ellama-summarize

Summarize a selected region or the current buffer using Ellama.
![ellama-summarize](imgs/ellama-summarize.gif)

### ellama-code-review

Review code in a selected region or the current buffer using Ellama.
![ellama-code-review](imgs/ellama-code-review.gif)

### ellama-change

Change text in a selected region or the current buffer according to a provided change.

### ellama-enhance-grammar-spelling

Enhance the grammar and spelling in the currently selected region or
buffer using Ellama.
![ellama-enhance-grammar-spelling](imgs/ellama-enhance-grammar-spelling.gif)

### ellama-enhance-wording

Enhance the wording in the currently selected region or buffer using Ellama.

### ellama-make-concise

Make the text of the currently selected region or buffer concise and simple using Ellama.

### ellama-change-code

Change selected code or code in the current buffer according to a provided change using Ellama.

### ellama-enhance-code

Change selected code or code in the current buffer according to a provided change using Ellama.

### ellama-complete-code

Complete selected code or code in the current buffer according to a provided change using Ellama.

### ellama-add-code

Add new code according to a description, generating it with a provided context from the selected region or the current buffer using Ellama.

### ellama-render

Render the currently selected text or the text in the current buffer as a specified format using Ellama.

### ellama-make-list

Create a markdown list from the active region or the current buffer using Ellama.

### ellama-make-table

Create a markdown table from the active region or the current buffer using Ellama.

### ellama-summarize-webpage

Summarize a webpage fetched from a URL using Ellama.

## Configuration

The following variables can be customized for the Ellama client:

- `ellama-url`: The URL to call Ollama.
- `ellama-curl-executable`: The path to curl executable.
- `ellama-model`: The model to use Ollama with. Default model is
  [zephyr](https://ollama.ai/library/zephyr).
- `ellama-buffer`: The default Ellama buffer name.
- `ellama-always-show-buffer`: Whether to always show the Ellama buffer.
- `ellama-user-nick`: The user nick in logs.
- `ellama-assistant-nick`: The assistant nick in logs.
- `ellama-buffer-mode`: The major mode for the Ellama logs buffer.
  Default mode is `markdown-mode`.
- `ellama-language`: The language for Ollama translation. Default
  language is english.
- `ellama-template`: The template to use with Ollama instead of the default.

## Acknowledgments

Thanks [Jeffrey Morgan](https://github.com/jmorganca) for excellent
project [ollama](https://github.com/jmorganca/ollama). This project
cannot exist without it.

Thanks [zweifisch](https://github.com/zweifisch) - I got some ideas
from [ollama.el](https://github.com/zweifisch/ollama) what ollama
client in Emacs can do.

Thanks [Dr. David A. Kunz](https://github.com/David-Kunz) - I got more
ideas from [gen.nvim](https://github.com/David-Kunz/gen.nvim).
