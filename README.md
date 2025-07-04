# gel-ast
GEL AST node entities definitions

Examples:
$.len == 100

len($) == 100

$scores.map((@elem int) -> { @elem*@elem })
 .reduce((@elem int, @result int) -> {@elem + @result}, 0) < 200

 abortIfFalse($ > 100, "Value is too small")

 abortIfTrue($ > 100, "Value is too big")
 
 throwIfFalse($ > 100, "Value is too small")
 
 errorIfFalse($ > 100, "Value is too small")
 
 stopIfFalse($ > 100, "Value is too small")

$scores.map({ @0 * @0 })
  .reduce({@0 + @1}, 0) < 200

