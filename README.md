# Hyde
This is my fork of the [Hyde](https://github.com/Keats/hyde) theme for the [Gutenberg](getgutenberg.io) static site generator. I've made a few style tweaks here and there and optimized for page size (my homepage weighs in at ~4kB).

Here are the tweaks I've made:

* Theming is more consistent.
* Headers and bold text in posts are now the same color as the headers in the list of posts.
* Print styles are removed (`print.scss` is still there, but not linked).
* Import `poole.scss` in `hyde.scss` to reduce the number of requests on page load.
* The native font stack is used instead of web fonts to increase page speed.
* You can hide a page by setting `hidden = true` in the `[extra]` section of the page frontmatter.

Other than that the theme is identical to the official [Hyde](https://github.com/Keats/hyde) from Gutenberg. As such, I'll direct you there for a description of all the options.

## Installation
First download this theme to your `themes` directory:

```bash
$ cd themes
$ git clone https://github.com/Keats/hyde.git
```
and then enable it in your `config.toml`:

```toml
theme = "hyde"
```

## Contributions
Since this is my personal blog theme, I'm only really looking for bugfixes at this time. If anyone wants to take a stab at merging `print.scss`, `poole.scss`, and `hyde.scss`, that would be more than welcome though.
