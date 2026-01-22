# Formatting & Layout Demo

This page shows common Markdown + MkDocs formatting options you can use.

---

## Headings, paragraphs, emphasis

Regular paragraph text goes here. Use *italics* for emphasis, **bold** for stronger emphasis,
and `inline code` for short code snippets.

You can also combine them, but keep it readable.

### Subheading

Another paragraph under a level-3 heading.

#### Level 4 heading

Short line of text.

---

## Lists

### Unordered list

- Bullet item one
- Bullet item two
  - Nested bullet
  - Another nested bullet
- Bullet item three

### Ordered list

1. First step
2. Second step
3. Third step

### Task list

- [ ] Open the model
- [x] Run baseline scenario
- [ ] Write up results

---

## Links and images

### Links

- Inline link: [MkDocs documentation](https://www.mkdocs.org/)
- Link to another page in the same site: [Run log](runs/index.md)

### Images

Below is an image reference. It will show if `img/model_schematic.png` exists in your `docs/img/` folder.

![Example schematic](img/model_schematic.png)

---

## Blockquotes

> This is a blockquote.  
> You can use it for short quotes or to visually separate important comments.

Nested blockquote:

> Outer quote
>
> > Inner quote


Ingredients:
- VSCode
- Github
- python, jupyter and flopy

!!! note "Tip"
    Useful information here.

??? note "Details"
    This text is initially folded.


## Code blocks

```python
print("hello")
```

```bash
echo "hello"
```

```md
Use `foo()` to process values.
```

This is ==important text== you want to highlight.