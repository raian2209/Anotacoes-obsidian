* lexing: It's the same as [[tokenising]], scanning or lexical analysis.
**is a programming that have breaking down a string  
into meaningful units, indepdendent of context**
## lexical grammar:
in computer science, a lexical grammar or lexical structure is a formal grammar defining the syntax of tokens. The program is written using characters that are defined by the lexical structure of the language used. The character set is equivalent to the alphabet used by any written language.


## Types:

### natural language
 In case of a natural language, those categories include nouns, verbs, adjectives, ponctuations etc.

### programming language

the categories include identifiers, operators, grouping symbols and data types. Lexical tokenization is related to the type of tokenization used in [[Large language models]] (LLMs), but with two differences. First, lexical tokenization is usually based on a lexical grammar, whereas LLM tokenizers are usually probability-based. Second, LLM tokenizers perform a second step that converts the tokens into numerical values

lexing a command in elixir:

`number += sqrt(16)` 

```elixir
[
    {"number", :identifier},
    {"+=", :operator},
    {"sqrt", :identifier},
    {"(", :separetor},
    {"16", :literal},
    {")", :separetor}
]
```
