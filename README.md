# Microsite Thing

This is a simple microsite-making package. It combines some of the little helpers
I like to use when building a microsite: Jekyll, a Bootstrap theme from Bootswatch,
straightforward SASS, concatenated static assets, and easy-to-steal Jekyll template
logic throughout.

## Before You Begin

1. Clone this repo locally.
1. Install Jekyll and SASS.
1. Run `sass --watch scss/site.scss:static/styles.css` and then `jekyll serve`

## Start Styling

* You can replace `_variables.scss` and `_darkly.scss` with another Bootswatch theme,
or just override the variables right there at the top of `site.scss`.
* The Bootswatch theme is totally optional; I just like it. It's nice to have a
little package with some colors and typography and some spacing / padding decisions
that all seem to work together.
* The rest of `site.scss` is mostly to center the navbar and make some specific
things work with the logo and text I was using.
