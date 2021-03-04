+++
title = "Markdown features"
description = "All features of Markdown"
date = 2021-03-01T15:00:00Z
updated = 2021-03-04
+++

This is post about markdown features. 

## Lists

- List
- Without numbers

or

1. Ordered list
    1. One
    2. Two
2. Come back to first level.

# Headers (H1)

## H2

### H3

#### H4

##### H5

###### H6

You can make text *italic* or **bold**.

# Code

Example of Rust code:

```rust

// `vst` uses macros, so we'll need to specify that we're using them!
#[macro_use]
extern crate vst;

// We're implementing a trait `Plugin` that does all the VST-y stuff for us.
impl Plugin for Whisper {
    fn get_info(&self) -> Info {
        Info {
            name: "Whisper".to_string()
        }
    }
}

```

You can also specify file name that convenient for tutorials:

<div class='filename'>
  <div>www/index.html</div>
</div>

```html
<div class='filename'>
  <div>src/lib.rs</div>
</div>
```

## Page separator

How it looks:

---

Syntax:

```html
---
```

## Quotes
{% quote(author="Richard Feynman") %}
The first principle is that you must not fool yourself and you are the easiest person to fool.
{% end %}

## Youtube

С вставкой `yt(id="the_id_here")`
{{ yt(id="ogEjvM-v_-s") }}

## Vimeo
`vm(id="id_here")`

{{ vm(id="115189988") }}

## Urls

[Example](https://tinyops.ru)

## Tables

Example:

Header 1  | Header 2
------------- | -------------
Content  | Content
Content  | Content

## Folding content

<details>
    <summary>Title 1</summary>
    <p>Content</p>
</details>

<details>
    <summary>Title 2</summary>
    <p>Content</p>
</details>

Syntax:

```html
<details>
    <summary>Title 1</summary>
    <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
```
