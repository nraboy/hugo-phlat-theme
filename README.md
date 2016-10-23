# Hugo Phlat Theme

A flat bootstrap theme for the Hugo static website engine.

![Hugo Phlat Theme Screenshot](https://raw.githubusercontent.com/nraboy/hugo-phlat-theme/master/images/screenshot.png)

A functional sample of this theme can be seen in action via [Own the Web](https://www.owntheweb.net).

## Installation

Use an existing Hugo project or create a fresh one before trying to install this theme.  Within the Hugo project, execute the following command from your Command Prompt (Windows) or Terminal (Mac and Linux):

```
mkdir themes
cd themes
git clone https://github.com/nraboy/hugo-phlat-theme
```

See the [official Hugo themes documentation](http://gohugo.io/themes/installing) for more info.

## Usage

This theme expects the standard Hugo site layout.

```
.
└── content
    ├── post
    |   ├── post1.md
    |   └── post2.md
    ├── page
    |   ├── about.md
    |   ├── contact.md
```

Run `hugo --theme=hugo-phlat-theme` to generate your site!

## Configuration

This theme relies heavily on a well crafted `config.toml` file.  It will consist of both optional and required parameters.

### Required Parameters

These parameters are required for the theme to compile and function correctly.

```toml
baseurl = "https://www.example.com/"
languageCode = "en-us"
title = "Own the Web"

[permalinks]
    post = "/:year/:month/:slug/"
    page = "/:slug/"

[taxonomies]
    tag = "tags"
    category = "categories"

[params]
    keywords = ["default", "keywords", "if", "no", "front", "matter"]
    description = "A description that will appear as a default if front matter does not exist"
```

### Optional Parameters

These parameters are optional, but including them will make your static website look nicer and take advantage of what the theme offers.

#### Header Menu

These menu items appear in the top right of the screen or within the drop list on mobile or smaller screen devices.

```toml
[[menu.header]]
    name = "Home"
    weight = 1
    url = "/"

[[menu.header]]
    name = "Resources"
    weight = 2
    url = "/resources/"

[[menu.header]]
    name = "Contact"
    weight = 3
    url = "/contact/"
```

#### Footer Menu

These menu items appear in the bottom left of the screen.

```toml
[[menu.footer]]
    name = "Privacy Policy"
    weight = 1
    url = "/privacy-policy/"

[[menu.footer]]
    name = "Sponsors"
    weight = 2
    url = "/sponsors/"
```

#### Other Parameters

Many of these parameters are social media links that appear at the bottom right of the screen in the footer.  Other parameters include Adsense identification numbers, Google Analytics, and similar.

```toml
[params]
    google_analytics = "UA-XXXXXXX-YY"
    google_adsense = "ca-pub-XXXXXXXX"
    disqus = "site_name_here"
    google_webmaster = ""
    bing_webmaster = ""
    alexa = ""
    twitter = "https://www.twitter.com/nraboy"
    googleplus = ""
    linkedin = ""
    youtube = ""
    paypal = ""
```

## About the Author

Phlat was designed and built by [Nic Raboy](https://www.nraboy.com) in San Francisco, California.

If you like this theme let me know!  You can reach me easiest on Twitter at [@nraboy](https://www.twitter.com).

## License

This theme is released under the MIT license.  For more information read the [License](LICENSE.md).
