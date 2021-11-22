# About List Collections in Elixir

Elixir implements list collections as linked lists. This mean that accessing the list length is an operation **that will run in linear time O(n)**. For this reason, it is typically faster to prepend thant to append, because prefixing is basically changing the HEAD reference of the linked list.

<br>
<br>

## Prepend example (faster): 

```
lista = [1, 2, :that]
["Example" | lista ]

>> ["Example", 1, 2, :that]
```

## Append example (slow): 

```
lista = [1, 2, :that]
lista ++ ["Testando"]

>> [1, 2, :that, "Testando"]
```

Continue tomorrow with Head/Tail
https://elixirschool.com/en/lessons/basics/collections