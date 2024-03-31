# kwceramics

My GitHub pages website for a personal hobby

## Website

Jekyll theme based on [Freelancer bootstrap theme](https://github.com/jeromelachaud/freelancer-theme)

### Layout

- `_includes` contains html templates
- `_layouts` contains the layout of the html for main page
- `_posts` contains the posts featured in the "Gallery"
  - must begin with a YYYY-MM-DD date and then title
  - must be `.markdown` files that start and end with `---` blocks
  - ordered by `date` property _inside_ the files
- `css` defines the css styles for html elements
- `img` contains the images referenced by `_posts`
  - `/gallery` for ones featured by gallery
  - `/raw` for raw images not featured (can still be linked to)
  - `favicon.ico` the icon for tab view, search engine, etc
  - `profile.png` the main image for page header
- `js` defines some (simple) code for navigation, email, etc on the page
- `_config.yml` defines some configuration that is referenced in `_html`

### Run locally

#### Setup (one-time)

On Mac (requires `ruby>=3`)

```shell
brew update ruby
sudo gem install bundler jekyll
```

#### Serve (each-time)

```shell
bundle exec jekyll serve
```

App runs on `http://localhost:4000`
