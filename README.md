# Purecss

Pure (purecss.io) is a set of small, responsive CSS modules that you can use in every web project realized by the yahoo developer team.
This gem adds it to the Assets Pipeline of Rails 3.2.

I cite directly from [purecss.io](http://purecss.io)
 > CSS with a minimal footprint.
 >
 > Pure is ridiculously tiny. The entire set of modules clocks in at 5.7KB minified and gzipped, without forgoing responsive styles, design, or ease of use. Crafted with mobile devices in mind, it was important to us to keep our file sizes small, and every line of CSS was carefully considered. If you decide to only use a subset of these modules, you'll save even more bytes.

For the moment it is possible to use only the responsive library, but I will change this as soon as I learn how to properly make better gems.

In this alpha release (0.0.1alpha3) I added FontAwesome. But given that purecss is compatible with the Bootstrap toolkit and rails-bootstrap provides FontAwesome, I plan to remove it in a subsequent update.

## TODO

I liked the idea of the light and functional Pure CSS and I think it is worthwile to create a gem for it.
I'd like to make something like [twitter-bootstrap-rails](https://github.com/seyhunak/twitter-bootstrap-rails) (and compatible with it)

I'd like to add
- Helpers for navigation bars, menus, forms, grids, ...
- Toolkit to set up website palette in an easy way
- Integration wit Rails SCSS
- System to keep the css updated
- Any ideas?

## Installation

Add this line to your application's Gemfile:

    gem 'purecss'

And then execute:

    $ bundle


Then you can either run the generator (with optional parameter responsive/nonresponsive):

    $ rails generate purecss:install

or add the following directives to your css manifest file (application.css):

    //= require purecss

for the responsive bundle, or

    //= require purecss-nr

for the non-responsive one.

If you want to include just an individual module (see [purecss.io](http://purecss.io)) add

    //= require purecss/<module>.js

instead.


## Usage

After the installation you can simply go to [purecss.io](http://purecss.io) and use (or extend) their predefined styles.


Enjoy!


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
