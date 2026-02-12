# Policies

## What This Is
Jekyll static site hosted on GitHub Pages. Legal documents: Terms of Use, Privacy Policy, and related pages.

## Development
```bash
bundle install

# Run locally (requires Gemfile modification)
# Comment out: gem "github-pages"
# Uncomment: gem "jekyll", "~> 3.9.0"
bundle exec jekyll serve

# When committing, reverse the Gemfile changes
```

## Adding Pages
1. Create `.md` file in `pages/` directory
2. Front matter:
   ```yaml
   ---
   layout: page
   title: Page Title
   permalink: /custom-path/
   exclude: true  # Set false to show in navbar
   ---
   ```
3. Add link in `index.md` if not excluded

## Deployment
- **Platform:** GitHub Pages
- **Auto-deploy:** On push to main branch
- **Build status:** [GitHub Actions](https://github.com/madebygoodbit/policies/actions)

## Future
May be merged into `goodbitco` marketing site eventually.

## Related Systems
- **Goodbitco** — Marketing site (eventual merge target)
- **Fireball** — Community platform (links to these policies)
