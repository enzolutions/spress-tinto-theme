## Tinto theme for Spress

Tinto is a ported theme to Spress design by [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes).
[Live demo](https://mmistakes.github.io/minimal-mistakes/).

### License
Free for personal and commercial use under the [MIT license](http://opensource.org/licenses/MIT)

### Featured:

* Responsive templates. Looking good on mobile, tablet, and desktop.
* Gracefully degrading in older browsers. Compatible with Internet Explorer 8+ and all modern browsers.
* Minimal embellishments -- content first.
* Optional large feature images for posts and pages.
* Simple and clear permalink structure.
* Custom 404 page to get you started.
* Support for Disqus Comments

### How to install?

Go to your [Spress](http://spress.yosymfony.com/) installation folder i.e  **~/Spress** and add the following depencency to your `composer.json` file

```
"require": {
    "enzolutions/spress-tinto-theme": "~1.0-dev"
}
```

and then run the following command to install the dependency.

```
$ composer update
```

### How to use?

**Create a new site**:

```bash
$ spress site:new /your-site-dir tinto
$ cd /your-site-dir tinto
$ spress site:build --server --watch
```

#### Menus

Spresso support top and bottom menus. To configure, you can edit
`top_menu` and `bottom_menu` options from the `config.yml`:

```yaml
# Menus
menu:
    top:
       - { name: "Home", url: / }
       - { name: "About", url: /about }
    bottom:
       - { name: "Spress add-ons", url: http://spress.yosymfony.com/add-ons , target: '_blank'}
       - { name: "Spress Docs", url: http://spress.yosymfony.com/docs, target: '_blank' }

bottom_menu:
    - { name: Go to Tinto theme web, url: https://github.com/enzoltions/Spress-theme-tinto }

```

#### Comments

Comments are powered by [Disqus](disqus.com) and it need your
**disqus shortname**. To get it, you need create a account at this service.
It's free.

##### Disable comments

By default, Disqus comments are enabled. If you want a post without comments, set
the `comments` variable to `false` at the Front-matter of the post:
```
---
comments: false
---
```
