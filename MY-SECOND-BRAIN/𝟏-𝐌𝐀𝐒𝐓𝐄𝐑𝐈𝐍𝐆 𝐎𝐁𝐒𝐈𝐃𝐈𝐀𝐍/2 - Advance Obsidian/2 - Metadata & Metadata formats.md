## Metadata

While most of the text in a note is meant to be read by a human, _metadata_ is text that's meant to be easily readable by a program, for example a [community plugin](https://help.obsidian.md/Extending+Obsidian/Community+plugins) or Obsidian itself.

You can add metadata to your notes by adding a block on the first line of your note. The block must start and end with three hyphens (`---`).

For example, the following note contains two pieces of metadata, `tag` and `publish`:

```yaml
---
tag: journal
publish: false
---

# Daily note

Today I learned about front matter.
```

## Metadata format (YAML)

Metadata uses a markup called YAML which stands for “Yet another markup language”.

[YAML](https://yaml.org/) is a widely used configuration format that's readable by both humans and machines. 

Each piece of metadata consists of a _key_ and a corresponding _value_.

```yaml
---
key: value
---
```

While the order of each key-value pair doesn't matter, each key must be unique within a note. For example, you can't have more than one `tag` key.

Values can be text, numbers, true or false, or even collections of values (arrays).

```yaml
---
title: A New Hope
year: 1977
favorite: true
cast:
  - Mark Hamill
  - Harrison Ford
  - Carrie Fisher
---
```


While we recommend using YAML to define metadata, you can also define metadata using [JSON](https://www.json.org/):

```md
---
{
  "tag": "journal",
  "publish": false
}
---
```

## Predefined metadata

Obsidian comes with of a set of predefined keys:

| Key        | Description                                                                                                                                                                                                                                                     |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `tag`      | See [Working with tags](https://help.obsidian.md/How+to/Working+with+tags).                                                                                                                                                                                     |
| `tags`     | Alias for `tag`.                                                                                                                                                                                                                                                |
| `alias`    | See [Aliases](https://help.obsidian.md/Linking+notes+and+files/Aliases).                                                                                                                                                                                        |
| `aliases`  | Alias for `alias`.                                                                                                                                                                                                                                              |
| `publish`  | Used by [Obsidian Publish](https://help.obsidian.md/Obsidian+Publish/Introduction+to+Obsidian+Publish) to [automatically select notes to publish](https://help.obsidian.md/Obsidian+Publish/Publish+and+unpublish+notes#Automatically select notes to publish). |
| `cssclass` | Allows you to style individual notes using [CSS snippets](https://help.obsidian.md/Extending+Obsidian/CSS+snippets).                                                                                                                                            |



