# Semicolons

Like C, Go's formal grammar uses semicolons to terminate statements, but unlike in C, those semicolons do not appear in the source. Instead the lexer uses a simple rule to insert semicolons automatically as it scans, so the input text is mostly free of them.

The formal syntax uses semicolons ";" as terminators in a number of productions. Go programs may omit most of these semicolons using the following two rules:

1. When the input is broken into tokens, a semicolon is automatically inserted into the token stream immediately after a line's final token if that token is
    - an identifier
    - an integer, floating-point, imaginary, rune, or string literal
    - one of the keywords break, continue, fallthrough, or return
    - one of the operators and punctuation ++, --, ), ], or }
2. To allow complex statements to occupy a single line, a semicolon may be omitted before a closing ")" or "}".

### Explanation:

In the Go programming language, semicolons are also used to terminate statements, similar to C. However, unlike C, where you must include semicolons explicitly in the source code, Go allows you to omit semicolons in many cases. Instead, Go's lexer (the component responsible for breaking the input source code into tokens for further processing) automatically inserts semicolons as needed during the lexical analysis phase.

This means that while semicolons are still used to terminate statements in Go, developers often don't need to explicitly include them in their source code. The lexer inserts semicolons based on simple rules, such as placing a semicolon at the end of a line if the line is the end of a statement and doesn't end with certain tokens like ), }, or an operator.

This design choice aims to reduce visual clutter and make the source code cleaner and more readable, as developers can focus on writing the logic of their programs without worrying about inserting semicolons at the end of each line. However, it's important for developers to understand the rules governing automatic semicolon insertion to avoid unexpected behavior in their code.