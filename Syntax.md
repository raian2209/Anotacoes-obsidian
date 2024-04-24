In computer science, the syntax of a computer language is the rules that define the combinations of symbols that are considered to be correctly structured statements or expressions in that language.

## levels of syntax

Computer language syntax is generally distinguished into three levels:

* Words – the lexical level, determining how characters form tokens;
* Phrases – the grammar level, narrowly speaking, determining how tokens form phrases;
* Context – determining what objects or variables names refer to, if types are valid, etc.

Distinguishing in this way yields modularity, allowing each level to be described and processed separately and often independently.

First, a [[lexer]] turns the linear sequence of characters into a linear sequence of tokens; this is known as "lexical analysis" or "lexing".

Second, the [[parser]] turns the linear sequence of tokens into a hierarchical syntax tree; this is known as "parsing" narrowly speaking. This ensures that the line of tokens conform to the formal grammars of the programming language. The parsing stage itself can be divided into two parts: the parse tree, or "concrete syntax tree", which is determined by the grammar, but is generally far too detailed for practical use, and the abstract syntax tree (AST), which simplifies this into a usable form. The AST and contextual analysis steps can be considered a form of semantic analysis, as they are adding meaning and interpretation to the syntax, or alternatively as informal, manual implementations of syntactical rules that would be difficult or awkward to describe or implement formally.

Thirdly, the contextual analysis resolves names and checks types. This modularity is sometimes possible, but in many real-world languages an earlier step depends on a later step – for example, the lexer hack in C is because tokenization depends on context. Even in these cases, syntactical analysis is often seen as approximating this ideal model.