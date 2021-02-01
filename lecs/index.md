//[lecs](../index.md)/[lecs](index.md)



# Package lecs  


## Types  
  
|  Name|  Summary| 
|---|---|
| <a name="lecs/LecsNode///PointingToDeclaration/"></a>[LecsNode](-lecs-node/index.md)| <a name="lecs/LecsNode///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>sealed class [LecsNode](-lecs-node/index.md)  <br><br><br>
| <a name="lecs/ListNode///PointingToDeclaration/"></a>[ListNode](-list-node/index.md)| <a name="lecs/ListNode///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [ListNode](-list-node/index.md)(**startToken**: [Token](-token/index.md), **nodes**: [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)<[LecsNode](-lecs-node/index.md)>, **endToken**: [Token](-token/index.md)) : [LecsNode](-lecs-node/index.md)  <br><br><br>
| <a name="lecs/MismatchedClosingBrace///PointingToDeclaration/"></a>[MismatchedClosingBrace](-mismatched-closing-brace/index.md)| <a name="lecs/MismatchedClosingBrace///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [MismatchedClosingBrace](-mismatched-closing-brace/index.md)(**openingBrace**: [Token](-token/index.md), **closingBrace**: [Token](-token/index.md)) : [ParseError](-parse-error/index.md)  <br><br><br>
| <a name="lecs/ParseError///PointingToDeclaration/"></a>[ParseError](-parse-error/index.md)| <a name="lecs/ParseError///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>sealed class [ParseError](-parse-error/index.md)  <br><br><br>
| <a name="lecs/SetNode///PointingToDeclaration/"></a>[SetNode](-set-node/index.md)| <a name="lecs/SetNode///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [SetNode](-set-node/index.md)(**startToken**: [Token](-token/index.md), **nodes**: [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)<[LecsNode](-lecs-node/index.md)>, **endToken**: [Token](-token/index.md)) : [LecsNode](-lecs-node/index.md)  <br><br><br>
| <a name="lecs/SymbolNode///PointingToDeclaration/"></a>[SymbolNode](-symbol-node/index.md)| <a name="lecs/SymbolNode///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [SymbolNode](-symbol-node/index.md)(**token**: [Token](-token/index.md)) : [LecsNode](-lecs-node/index.md)  <br><br><br>
| <a name="lecs/Token///PointingToDeclaration/"></a>[Token](-token/index.md)| <a name="lecs/Token///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [Token](-token/index.md)(**value**: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), **location**: [IntRange](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.ranges/-int-range/index.html)) : [TokenizerTypes](-tokenizer-types/index.md)  <br><br><br>
| <a name="lecs/TokenizerTypes///PointingToDeclaration/"></a>[TokenizerTypes](-tokenizer-types/index.md)| <a name="lecs/TokenizerTypes///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>sealed class [TokenizerTypes](-tokenizer-types/index.md)  <br><br><br>
| <a name="lecs/UnmatchedClosingBrace///PointingToDeclaration/"></a>[UnmatchedClosingBrace](-unmatched-closing-brace/index.md)| <a name="lecs/UnmatchedClosingBrace///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [UnmatchedClosingBrace](-unmatched-closing-brace/index.md)(**closingBrace**: [Token](-token/index.md)) : [ParseError](-parse-error/index.md)  <br><br><br>
| <a name="lecs/UnmatchedOpeningBraces///PointingToDeclaration/"></a>[UnmatchedOpeningBraces](-unmatched-opening-braces/index.md)| <a name="lecs/UnmatchedOpeningBraces///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [UnmatchedOpeningBraces](-unmatched-opening-braces/index.md)(**openingBraces**: [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)<[Token](-token/index.md)>) : [ParseError](-parse-error/index.md)  <br><br><br>
| <a name="lecs/VectorNode///PointingToDeclaration/"></a>[VectorNode](-vector-node/index.md)| <a name="lecs/VectorNode///PointingToDeclaration/"></a>[jvm]  <br>Content  <br>data class [VectorNode](-vector-node/index.md)(**startToken**: [Token](-token/index.md), **nodes**: [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)<[LecsNode](-lecs-node/index.md)>, **endToken**: [Token](-token/index.md)) : [LecsNode](-lecs-node/index.md)  <br><br><br>


## Functions  
  
|  Name|  Summary| 
|---|---|
| <a name="lecs//parse/#kotlin.collections.List[lecs.Token]/PointingToDeclaration/"></a>[parse](parse.md)| <a name="lecs//parse/#kotlin.collections.List[lecs.Token]/PointingToDeclaration/"></a>[jvm]  <br>Content  <br>fun [parse](parse.md)(tokens: [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)<[Token](-token/index.md)>): Either<[ParseError](-parse-error/index.md), [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)<[LecsNode](-lecs-node/index.md)>>  <br><br><br>
| <a name="lecs//tokenize/#kotlin.String/PointingToDeclaration/"></a>[tokenize](tokenize.md)| <a name="lecs//tokenize/#kotlin.String/PointingToDeclaration/"></a>[jvm]  <br>Content  <br>fun [tokenize](tokenize.md)(input: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)): [List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)<[Token](-token/index.md)>  <br><br><br>

