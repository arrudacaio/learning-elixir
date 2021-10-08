# About List Collections in Elixir

Elixir implements list collections as linked lists. This mean that accessing the list length is an operation **that will run in linear time O(n)**. For this reason, it is typically faster to prepend thant to append, because prefixing is basically changing the HEAD reference of the linked list.