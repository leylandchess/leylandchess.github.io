# Leyland Chess Web Site

This is the code repository for the [web site](https://leylandchess.github.io).

## Quick start for contributors

### Markdown

Page content is written in markdown for simplicity; there's a cheat sheet
[here](https://www.markdownguide.org/cheat-sheet).  The names of markdown
files end in .md - Github automatically generates the .html files for you.
(You can write in HTML if you prefer, and give your file the suffix .html).

### Layouts

Top level pages which don't inlude chess diagrams should start with

```
---
layout: with-nav
title: Your Title Here
---
```
This puts the navigation bar at the top.  Pages which include a chess diagram
should start with

```
---
layout: with-pgn
title: Your Title Here
---
```

### New pages

In addition, new top level pages need to be added to `_data/navigation.yml`
like this:

```
- title: Your Title Here
  url: /your_page.html
```
so that they appear in the navigation bar.  (Recall that Github generates
`your_page.html` from `your_page.md`).

### Blog posts

These **must** be created in the `_posts` directory with the date in the title
in the form `YYYY-MM-DD-your-subject.md`.  That way they get correctly recognized
by Github, and put in chrononlogical order on the blog page.

### Chess diagrams

These use [pgn4web](http://pgn4web.casaschi.net).  Currently we support fixed
FEN positions and navigable PGN games.  See the first two example blog posts
for how to embed them.  Remember to use the `with-pgn` layout.  There can be
at most one diagram per page at the moment.

## Note for developers

Github uses [Jekyll](https://jekyllrb.com) to build the site.  You can set Jekyll
up locally to render and test the site before pushing changes. There's a decent
tutorial at the Jekyll page - this site's navigation is lifted from it.
