# HUGO Podcasts

*Podcast publishing for [hugo static site generator]([https://gohugo.io/](https://github.com/gohugoio/hugo))*

## SETUP

This module is a good add-on to my minimalistic HUGO theme module [energye](https://github.com/frankrenold/energye).

### As a HUGO module ([preferred](https://www.hugofordevelopers.com/articles/master-hugo-modules-managing-themes-as-modules/))

#### Install

Make your project a HUGO module

```
hugo mod init your-project-repo
```

Add this theme as a HUGO module and make sure taxonomy configuration is merged from it

```
#config.yaml
module:
  imports:
  - path: github.com/frankrenold/hugo-podcasts
taxonomies:
  _merge: shallow
```

[Read more](https://www.hugofordevelopers.com/articles/master-hugo-modules-managing-themes-as-modules/)

#### Update after installation
```
hugo mod get
```

## MANAGING PODCAST CONTENT

You find a folder "sample-content" in the repository. Add the content of this folder to your projects content folder to start off.

### Content folder structure

- episodes (contains all episodes for all podcasts)
- podcasts (contains the podcasts)

### Unique audio file names

Every podcast episode needs a unique id. Please make sure, all your episodes of a podcast have unique audio file names as long as you do not change anything in the content of the file. The module uses a hash of the filename as unique id of the episode in the feed.
