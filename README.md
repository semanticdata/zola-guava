# 🍈 Guava

<p align="">
  <img src="https://img.shields.io/github/languages/code-size/semanticdata/zola-guava" />
  <img src="https://img.shields.io/github/repo-size/semanticdata/zola-guava" />
  <img src="https://img.shields.io/github/commit-activity/t/semanticdata/zola-guava" />
  <img src="https://img.shields.io/github/last-commit/semanticdata/zola-guava" />
  <img src="https://img.shields.io/website/https/semanticdata.github.io/zola-guava.svg" />
</p>

Zola Guava is based on [rust-br/dinkleberg](https://github.com/rust-br/dinkleberg). The aim of the project is to revive what is a beautiful theme.

Checkout the live [demo](https://miguelpimentel.do/zola-guava/) of the theme.

## Features and Improvements

* Refactored color styles. Makes it easier to cusotmize the site.
* Made different Typography choices. Big change to `line height`.
* Justified post contents without affecting titles.
* Fixed codeblocks line height and border issues.
* Changed code highlighting theme to `zenburn`.
* Added additional nav section for external *Links* alongside *Social* links.
* Addressed Issue [#2](https://github.com/rust-br/dinkleberg/issues/2). Fixed mobile version. No longer broken.
* Addressed Issue [#12](https://github.com/rust-br/dinkleberg/issues/12). Fixed `config.toml` by adding `label_minutes`. Would not build before.
* Addressed Issue [#13](https://github.com/rust-br/dinkleberg/issues/13). Fixed code padding.

## Screenshots

![website screenshot](screenshot.png)

## Configurations

```toml
[extra]
blog_logo="/imgs/common/logo.png" #will appear on top header
blog_title="My Blog" #will appear on top header after logo

## i18n words
label_tags = "Tags"
label_tag = "Tag"
label_categories = "Categorias"
label_category = "Categoria"
label_relative_posts = "Postagens Relacionadas"
label_next = "Próxima"
label_previous = "Anterior"
label_page = "Página"
label_of = "de"
label_minutes = "minutos"

og_image="" # Image that will appear on social media
og_alt_image="" # Alt for og_image
og_site_name="" # Site Name for Open Graphic
keywords="" # Keywords for SEO

educational_use="knowledge share" # OPTIONAL
copyright_year="2018" # OPTIONAL

fb_app_id="???" # OPTIONAL, Facebook App Id to help in metrics
twitter_username="@???" # OPTIONAL, Twitter User to help with metrics

## Sidebar automatic links
sidebar = [
    {name = "Social", urls=[
        {name="Telegram", url="https://t.me/rustlangbr"},
        {name="Github", url="https://github.com/rust-br"},
    ]},
    {name = "Divida Conhecimento!", urls=[
        {name="Contribuir!", url="https://rust-br.github.io/blog/hello-world"}
    ]}
]

```

## Running the Site Locally

Tips that will help you develop and preview the site locally.

### Requirements

Before using the theme, you need to install [Zola](https://www.getzola.org/documentation/getting-started/installation/) ≥ 0.18.0.

### Quick Start

```bash
# clone the repo
git clone git@github.com:semanticdata/zola-guava.git
# change directory into the cloned folder
cd zola-guava
# serve the site locally
zola serve
# open http://127.0.0.1:1111/ in the browser
```

For more detailed instructions, visit the [Documentation](https://www.getzola.org/documentation/themes/installing-and-using-themes/) page about installing and using themes.

### Useful Commands

A short list of commands that will help you develop your own version of the theme.

| Command                    | Description                |
| -------------------------- | -------------------------- |
| `zola init <my-repo>`      | Initiate new Zola site     |
| `zola build`               | Build only                 |
| `zola serve`               | Build and Serve            |

## Customization

You can changed the configuration, templates and content yourself. Refer to the `config.toml`, and templates files for ideas. In most cases you only need to modify the contents of `config.toml` to customize the appearance of your blog. Make sure to visit tyhe [Zola Documentation](https://www.getzola.org/documentation/getting-started/overview/).

### Custom CSS Styles

Adding custom CSS is as easy as adding your styles to `sass/_custom.scss`. This is made possible because SCSS files are backwards compatible with CSS. This means you can type normal CSS code into a SCSS file and it will be valid.

## Acknowledgements and Attributions

The icons used throughout the site are kindly provided by [UXWing](https://uxwing.com/license/). Read their [license](https://uxwing.com/license/).

Other icons used come from [Remix Icon](https://remixicon.com/). Check out their [license](https://remixicon.com/license).

## License

Source code in this repository is available under the [MIT License](LICENSE).
