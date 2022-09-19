# HUGO Podcasts

*Podcast publishing for [hugo static site generator]([https://gohugo.io/](https://github.com/gohugoio/hugo))*

## SETUP

### As a HUGO module ([preferred](https://www.hugofordevelopers.com/articles/master-hugo-modules-managing-themes-as-modules/))

#### Install

Make your project a HUGO module

```
hugo mod init your-project-repo
```

Add this theme as a HUGO module

```
#config.yaml
module:
  imports:
  - path: github.com/frankrenold/hugo-podcasts
```

[Read more](https://www.hugofordevelopers.com/articles/master-hugo-modules-managing-themes-as-modules/)

#### Update after installation
```
hugo mod get
```
