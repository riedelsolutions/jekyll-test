# Root

Root is a modern, minimal, tag-based Jekyll blog theme designed to be simple and not distract from the actual content of the site &mdash; your posts. Coded for you to focus on your blog posts and content only.


## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "root"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: root
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install root

## Usage

### Tag System

Simply put the tags you wish to have on the tag menu in the front matter of your posts, they will be automatically generated and not repeated.

### Tag Pages

For the tag pages/sections, do the following

1. Create your html file, e.g. `example.html`

2. Add the following front matter and expression:

```
---
layout: default
---

{% include tagPagesLoop.html tagName='TAG_NAME_HERE' %}

```

### Styling

Every style is under /assets/main.scss

### Assets

All images go under /images


## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/riedelsolutions/root. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `root.gemspec` accordingly.
