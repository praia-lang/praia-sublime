# Praia Syntax Highlighting

Sublime Text syntax highlighting for the [Praia](https://praia.sh) programming language.

## Installation

### Package Control

1. Open the Command Palette (`Cmd+Shift+P` / `Ctrl+Shift+P`)
2. Select **Package Control: Install Package**
3. Search for **Praia Syntax Highlighting**

### Manual

Clone this repo into your Sublime Text `Packages` directory:

```
git clone https://github.com/praia-lang/praia-sublime.git "Praia Syntax Highlighting"
```

## Features

- Full syntax highlighting for `.praia` files
- String interpolation (`%{expr}`)
- Triple-quoted multiline strings
- Nested block comments
- Shebang detection
- Comment toggling (`Cmd+/` / `Ctrl+/`)

## Recommended Settings

These settings work well with Praia. To use them, open a `.praia` file and choose
**Preferences → Settings - Syntax Specific** from the menu, then paste:

```json
{
    "tab_size": 4,
    "translate_tabs_to_spaces": true,
    "auto_match_enabled": true,
    "word_separators": "./\\()\"'-:,.;<>~!@#$%^&*|+=[]{}`~?"
}
```

## Tests

Syntax tests live in [`tests/`](./tests). Open a test file in Sublime Text and run
**Build With: Syntax Tests** (`Cmd+B` / `Ctrl+B`) to verify the syntax. See the
[Sublime docs](https://www.sublimetext.com/docs/syntax.html#testing) for details.

## License

[MIT](./LICENSE)
