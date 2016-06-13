# Microsite Thing

This is a simple microsite-making package. It combines some of the little helpers
I like to use when building a microsite: Jekyll, a Bootstrap theme from Bootswatch,
straightforward SASS, concatenated static assets, and easy-to-steal Jekyll template
logic throughout.

## Before You Begin

1. Clone this repo locally.
1. Install Ruby and Jekyll.
1. Run `jekyll serve`.

## Start Styling

* There are two themes here; the default is called "dark", and there's a
basically-blank bootstrap theme called "blank". That's set by the `theme`
variable in `_config.yml`.
* You can add new styling rules to `site.scss`, or if you're a stickler about
keeping a pretty file structure, go into `_site-theme.scss`
and `_layout.scss`.
* But it's best not to touch `_variables.scss` or `_darkly.scss` if you can
avoid it; those are Bootswatch theme files and if you ever choose to drop in
[a new Bootswatch theme](https://bootswatch.com/), you don't want to have to reapply any changes.
* Or remove the theme altogether! If you comment out `variables` and `darkly`, you end up
with a pretty nice version of a stock Bootstrap theme.
* For best effect, make styling changes by overriding Bootstrap SASS variables;
declare these at the top of `site.scss`.

## Idiosyncrasies

For reasons, I chose to use an inline for a logo in a few places. This means that
`static/images/logo.svg` actually just says `{% include logo.svg %}`. This is probably not a pattern
you'll repeat with your own microsite, so it was kind of silly for me to do it
in what was meant to be a template for future work.
