# vncnt-hugo

This is a simple theme for [**hugo**](https://gohugo.io/) which can serve as a template for personal landing pages.

## Installation

Clone this repo into your `themes` directory of your **hugo** website:
```
git clone https://github.com/fncnt/vncnt-hugo themes/vncnt-hugo
```
Or even better, add this repository as a submodule of your **hugo** website, if you are using `git` for it:
```
git add submodule https://github.com/fncnt/vncnt-hugo themes/vncnt-hugo
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
However, those are trade-offs I'm willing to accept for simplicity.

## Third-party Components

This theme relies on fontawesome. The included files in `static/webfonts` are used under the SIL Open Font License 1.1 as described in `static/css/all.min.css`. The latter file is licensed under the MIT License.

The Raleway font files in `static/fonts` are licensed under the SIL Open Font License 1.1 (see `static/fonts/OFL.txt`)

Both `normalize.css` and `skeleton.css` are licensed unter the MIT License.

## Roadmap

- possibly get rid of skeleton.css
- add support for including blog-like content

