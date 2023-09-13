# Micro-site MIIA

Code source du [site](https://iid-ulaval.github.io/ppr-iidays/) de présentation de la journée IID des PPRs affiliés à l'ULaval.

## Development setup

To develop this site locally, you need to 
1. Install [rbenv](https://github.com/rbenv/rbenv)
   - `rbenv` is a [Ruby](https://www.ruby-lang.org/fr/) version manager
2. Run -> `rbenv install $(cat .ruby-version)`
   - This will install ruby version `3.1.0`
3. Run -> `gem install bundler`
   - `bundler` helps with managing _gems_
4. Run -> `bundle install`
   - This will install the project dependencies listed in the [Gemfile](./Gemfile)
5. Run -> `bundler exec jekyll serve`
   - This will run the server and fire the website at http://127.0.0.1:4000

## Pages

To add a new page to the webiste, simply create a Markdown file in the folder [pages](./pages/)

File in `pages` are in french and you should provide an english translation in the folder [pages/en/](./pages/en/).

> **<p style="color:red">Important : English Pages !</p>**

When you create an english page, you must add the following frontmatter to your Markdown at the beginning of your file:
```mardowm
---
lang: en
---
```
