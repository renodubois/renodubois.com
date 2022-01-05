I'm gonna forgot how this directory works, so here's the quick rundown.

## _defaults

The "default" folder. Defines two different types of templates - `page` and `list`.
`page is a regular content page - a blog post, a note, etc. A `list` is a page that
displays a list of posts, generally. This would be something like `/posts` or `/notes`.
That template will display a list of the files in whatever path we're looking at
(i.e. all blog posts when in `posts/`) and it can also display info before
that - that info is sourced via the directory's `_index.md` file.
See `notes/_index.md` for a good example of this.

## partials

Partial templates - ones that are included in larger templates via calls to
`{{ partial "partialname.html" . }}`. In my case, I have a header and a footer.

## notes

Templates specific to the notes directory.
