iex で次のプログラムを試してみよう。

``` elixir
iex(6)> ['cat' | 'dog']
['cat', 100, 111, 103]
```

なぜ、iex は 'cat' を文字列として表示しているのに、'dog' を文字コードで表示しているのだろう?

- cat は文字リストになっている
- しかし ['cat' | 'dog']の場合, あるリストの先頭の要素が 'cat' になっており, 'dog' が末尾のリストになる
- Elixr が文字列を表示する条件としてはすべての文字として印字可能と判断するため('cat' は文字ではなく文字のリスト)
