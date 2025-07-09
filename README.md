# Run locally

## Preliminaries
1. Create `Gemfile` under the root folder:
    ```txt
    source 'https://rubygems.org'

    group :jekyll_plugins do
    gem 'jekyll'
    gem 'jekyll-feed'
    gem 'jekyll-sitemap'
    gem 'jekyll-redirect-from'
    gem 'jemoji'
    gem 'webrick', '~> 1.8'
    end

    gem 'github-pages'
    gem 'connection_pool', '2.5.0'
    ```

2. In WSL,
    ```bash
    sudo apt install ruby-dev ruby-bundler nodejs
    bundle config set --local path 'vendor/bundle'
    bundle install
    ```

## Run
1. Run 
    ```bash
    bundle exec jekyll serve -l -H localhost
    ```
    in the local terminal.

2. Open `localhost:4000` in the browser.