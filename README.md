# Goodbit Policies

Run `bundle install` to install dependencies.

## To run locally

1. In the Gemfile, comment out line 18: `gem "github-pages", group: :jekyll_plugins` and un-comment out line 11: `gem "jekyll", "~> 3.9.0"`

2. Run `bundle exec jekyll serve` to run the site locally.

When you commit to the github repo, reverse `step 1`.

## To add a new page

1. Create a new markdown file (`.md`) in the `pages` directory.
2. The header should include the following:

```
---
layout: page
title: Small trivia, big challenge!
permalink: /stbu-pp/
exclude: true
---
```

- Layout: Which layout to use; the options are `home` or `page`. `page` is used for Terms of Use and Privacy Policy pages.
- Title: The title that will be shown in the browser.
- Permalink: This is where you define what link the page should use. All links have `/policies` as a subpage before the permalink.
- Exclude: Choose `true` if you don't want this page to show up in the navbar on the home page. Choose `false` if you want it in the header - i.e. if it's an important page that is relevant to the organization as whole.

3. The pages will automatically be built into `html` using the `markdown` file. Here is a guide for how to use styling in markdown: [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/).
4. To add your new page to the home screen, go to `index.md` and add it as a link using the following syntax:

```
[Privacy Policy](/policies/stbu-pp)
```

## Build and Deployment

When you commit and push a change to Github, it will automatically build the new pages. You can view the progress of the build here:

[Github Actions](https://github.com/madebygoodbit/policies/actions)
