+++
title = "Hello, world"
date = 2026-08-21
description = "A first post to make sure the pipeline works end to end."
[taxonomies]
tags = ["meta", "zola"]
+++

This is a placeholder post so the templates have something to render.[^1]

[^1]: Footnotes render at the bottom of the post, with a link back to where
they were referenced. Set by `bottom_footnotes` in `zola.toml`.

## A code block

```rust
fn main() {
    let greeting = "hello, world";
    println!("{greeting}");
}
```

And some `inline code`, a [link](https://www.getzola.org/), and a quote:

> Premature optimization is the root of all evil.

## A table

| Column | Type | Notes |
|---|---|---|
| `id` | uuid | primary key, generated |
| `created_at` | timestamptz | indexed, defaults to `now()` |
| `payload` | jsonb | unconstrained, can get large |
| `status` | text | one of `queued`, `running`, `done` |
