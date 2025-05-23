# Tutorial: marked

The `marked` project is a **Markdown** *compiler*. It takes Markdown-formatted text as input and transforms it into **HTML**, which can be displayed in a web browser.  It provides options and extensions to customize the conversion process.


**Source Repository:** [https://github.com/markedjs/marked.git](https://github.com/markedjs/marked.git)

```mermaid
flowchart TD
    A0["Marked (Instance)
"]
    A1["Lexer
"]
    A2["Parser
"]
    A3["Renderer
"]
    A4["Tokenizer
"]
    A5["Tokens
"]
    A6["Marked Options
"]
    A7["Hooks
"]
    A0 -- "Uses" --> A1
    A0 -- "Uses" --> A2
    A0 -- "Uses" --> A3
    A0 -- "Configures" --> A6
    A0 -- "Uses" --> A7
    A1 -- "Delegates to" --> A4
    A1 -- "Generates" --> A5
    A2 -- "Uses" --> A3
    A3 -- "Uses" --> A2
    A4 -- "Uses" --> A6
    A6 -- "Configures" --> A1
    A6 -- "Configures" --> A2
    A6 -- "Configures" --> A3
    A6 -- "Configures" --> A4
    A7 -- "Modifies" --> A1
    A7 -- "Modifies" --> A2
    A0 -- "Walks" --> A5
```

## Chapters

1. [Marked (Instance)
](01_marked__instance__.md)
2. [Marked Options
](02_marked_options_.md)
3. [Lexer
](03_lexer_.md)
4. [Tokenizer
](04_tokenizer_.md)
5. [Tokens
](05_tokens_.md)
6. [Parser
](06_parser_.md)
7. [Renderer
](07_renderer_.md)
8. [Hooks
](08_hooks_.md)


---

Generated by [AI Codebase Knowledge Builder](https://github.com/The-Pocket/Tutorial-Codebase-Knowledge)