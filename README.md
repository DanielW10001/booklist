# booklist

Structured publish info for CS and EE books.

Structure: "TITLE", "AUTHOR", "PUBLISHER"

Notice: 

- Chinese and English publishes are included.
- For publishes with multiple authors, only one author is included.
- Publisher may be not included.
- May include empty line or comment line led with '#'.

Work with Python 3:

```python3
with open('./book.txt', 'r', encoding='utf-8') as file:
    for line in file:
        if line[0] != '\n' and line[0] != '#':
            title, author, publisher = eval(line)
```

Issues and PRs are more than welcomed.

Licensed under `LICENSE.md`.

