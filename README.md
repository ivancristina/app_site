# Jekyll App Site

The Jekyll App Site is a small Jekyll template to present an iPhone app with a static site, made by **JP Simard**.

There are indeed very few differences between my fork and his project, which are:

* Ready to use `assets`, no need to build in **rake** (removed from `.gitignore`)
* Updated with Jet Black **iPhone 7** frame
* Added Gold **iPhone 5S** frame *(not used)*
* Updated jquery from `2.0.3` up to `3.3.1`
* Updated the date, from static *`2014`* to Jekyll dynamic year
* Added an entry in `_config.yml` to choose the icon path
* Switched from `redcarpet` to `kramdown` **markdown** language
* Added `rouge` highlight method *(not needed though)*
* Added `rake` and `rsync` as **`plugins`** in `_config.yml`

## Running Locally

Even though I already compiled all the assets, if you want to do that yourself, I kept a copy of the `_assets` path.

Make sure you have all the [requirements](#requirements) installed.

There are 4 rake tasks:

* `rake`: same as running `rake:serve`
* `rake serve`: compile and run the site with changes reloaded automatically
* `rake build`: compile the site without running it. Useful for deploying.
* `rake clean`: deletes the `_site` and `assets` directories

To deploy, upload the `_site` directory to your static HTML server (i.e. [AWS S3](http://aws.amazon.com/s3)).

## Requirements

* [Jekyll](http://jekyllrb.com): `gem install jekyll`
* [Sass](http://sass-lang.com): `gem install sass`
* [rsync](http://rsync.samba.org)

## Modifying

You'll probably want to modify the following files for your project:

* `_config.yml` for site constants (name, tagline, etc.)
* `favicon.ico` for the site's favicon
* `index.md` for content
* `press/index.md` for content
* `support/index.md` for content
* `_assets/stylesheets/globals/variables.scss` for colors
* `_assets/images/*` for images

## Credits

* Entirely based on  [JP Simard](https://github.com/jpsim)'s Project. Take a look at his [Demo](http://jpsim.com/jekyll_app_site)
* HTML/Sass for this template was originally written for Sinatra by [Sam Soffes](https://github.com/nothingmagical/getcoinsapp.com)
* [Grater](https://github.com/soffes/grater)
* [Bourbon](http://bourbon.io)

## License

MIT licensed.
