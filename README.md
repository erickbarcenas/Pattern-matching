# Pattern-matching

```elixir
{a, b, [1, 2, c]} = {5, 6, [1, 2, 3]}
```

```elixir
lista = ["tania", "erick"]
```

```elixir
["tania", "erick"] = lista 
```

```elixir
[_, _, _, x] = [1, 2, 3, 4, 5]
```

```elixir
{suma} = {3+5+6}
```

```elixir
["uno", x, {:atomo, x}] = ["uno", "dos",{:atomos, 12}] 
```


```elixir
[h | [a, b, c, 5]] = [1, 2, 3, 4, 5]
```

```elixir
x = :ok 
```


```elixir
{_, _, [valor, {:ok, a, [5, _,]}]} = {1, 2, ["valor", {:ok, 3, [5, 6]}]}
```


 ```elixir
defmodule Math do
  def sum_list(list, accumulator \\ 0)

  def sum_list([head | tail], accumulator) do
    sum_list(tail, head + accumulator)
  end

  def sum_list([], accumulator) do
    accumulator
  end
end


Math.sum_list([1, 2, 3])
6
Math.sum_list([1, 2, 3], 1)
7
```

