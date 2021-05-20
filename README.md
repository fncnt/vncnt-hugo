# vncnt-hugo

This is a simple theme for [**hugo**](https://gohugo.io/) which can serve as a template for personal landing pages.

## Installation

Clone this repo into your `themes` directory of your **hugo** website:
```
git clone https://github.com/fncnt/vncnt-hugo themes/vncnt-hugo
```
Or even better, add this repository as a submodule of your **hugo** website, if you are using `git` for it:
```
git submodule add https://github.com/fncnt/vncnt-hugo themes/vncnt-hugo
```

## Configuration

Copy the `config.toml` file of the theme into the main directory of your **hugo** website.
You may want to adjust the value of `baseURL` as well as the parameters in the `[params]` section.

If you set `email` in `[params]`, the link to your email will appear in front of all keys set in `[params.contact].`

### Changing Contact Links

To add a link to a preferred service of your choice simply add a suitable key to `[params.contact]`, e.g.
```
linkedin = "https://www.linkedin.com/in/jdoe"
```
Please note that the key must correspond to a [fontawesome brands icon](https://fontawesome.com/icons?d=gallery&s=brands).
Also, regardless of the key order in your `config.toml` file, the links will be ordered lexicographically due to the usage of [`range`](https://golang.org/pkg/text/template/#hdr-Actions).

However, you may specify contact links more verbosely, as documented in [`config.toml`](config.toml).
This allows to use other fontawesome styles and manually sort contact links.

## Third-party Components

The spine (I'm so sorry) of this theme is made of [`Barebones`](https://github.com/acahir/Barebones).
Both `normalize.css` and `barebones.css` are licensed unter the MIT License.

This theme relies on fontawesome. The included files in `static/webfonts` are used under the SIL Open Font License 1.1 as described in `static/css/all.min.css`. The latter file is licensed under the MIT License.

The Raleway font files in `static/fonts` are licensed under the SIL Open Font License 1.1 (see `static/fonts/OFL.txt`)

### Tracking

The theme supports Google Analytics using Hugo's internal templates. To enable
tracking, set the [googleAnalytics](https://gohugo.io/templates/internal/#configure-google-analytics)
and (optionally) [privacy](https://gohugo.io/about/hugo-and-gdpr/#all-privacy-settings) configuration values.

## Dark Mode

On [supported browsers](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-color-scheme#Browser_compatibility), this theme applies a dark mode if the user's OS itself is set to dark.

## Roadmap

- add support for blog-like content

