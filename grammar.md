# Grammar

- Var -> int | float

Initialize variables (Complete):
- DefinitionLine -> Initialize ; DefinitionLine
- DefinitionLine -> Empty
- Initialize -> Var name InitializeStart 
- InitializeStart -> = value InitializeList
- InitializeStart -> = Exp
- InitializeStart -> InitilializeList
- InitializeList -> , name InitializeList
- InitializeList -> , name = value InitializeList
- InitializeList -> Empty

Assign Values:
- AssignLine -> Assign ;
- Assign -> name = value

Expression

ExpressionAssign -> Expression ; <!-- Não existem comunicações irrelevantes no SSL --->
Expression -> Value Op Expression
Expression -> ( Value Op Expression )
Expression -> ( Value )
Expression -> Value
Op -> \|\| | && | > | < | == | >= | <= | + | - | * | % | / | ^ | >> | << | & |
Value -> literal
Value -> variable 

Conditional
if $$
