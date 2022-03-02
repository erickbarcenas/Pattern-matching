# Pattern-matching

{a, b, [1, 2, c]} = {5, 6, [1, 2, 3]}
lista = ["tania", "erick"]
["tania", "erick"] = lista 
[_, _, _, x] = [1, 2, 3, 4, 5]
{suma} = {3+5+6}
["uno", x, {:atomo, x}] = ["uno", "dos",{:atomos, 12}] 
[h | [a, b, c, 5]] = [1, 2, 3, 4, 5]
x = :ok 
{_, _, [valor, {:ok, a, [5, _,]}]} = {1, 2, ["valor", {:ok, 3, [5, 6]}]}
