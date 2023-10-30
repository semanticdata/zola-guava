<!-- ![753986_1](https://user-images.githubusercontent.com/10289071/40806112-dd79ae78-64f6-11e8-8f24-63f387d5bb8f.jpg)  -->

# Zola Test via Dinkleberg

## Features

Zola Dinkleberg is based on [rust-br/dinkleberg](https://github.com/rust-br/dinkleberg). The aim of the project is to revive what is a beautiful theme. That said, I have added the following:

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

<img alt="Website Screenshot" src="screenshot.png" width="720px" />

## Configurations

```toml
[extra]
blog_logo="/imgs/common/logo.png" #will appear on top header
blog_title="rust::br::Blog" #will appear on top header after logo

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

This configuration was the same configuration that we use on [RustBR Blog](https://rust-br.github.io/blog)

### Favicons and other stuff

By default Dinkleberg wait that you have all icons on root of your static, for it you can use the site [https://www.favicon-generator.org/](https://www.favicon-generator.org/) to generate that bundle and put it inside you `/static` :D
