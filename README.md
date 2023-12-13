# Statamic Video


Custom video fieldset for Statamic 3.

## [Video Fieldset](https://statamic.dev/fieldtypes/video)

Extract embed URLs from Youtube, Vimeo, and HTML5 compatible video links and preview them right inline. Feel free watch the whole thing instead of working – we won't tell.

### Type

### Mute button

### Autoplay

### Loop

### Caption

## [Statamic Modifiers](https://statamic.dev/modifiers)

Modifiers manipulate the data of your variables on the fly in Antlers templates. They can modify strings, filter arrays and lists, perform comparisons, handle basic math, simplify your markup, and even help you debug.

This video fieldset includes 3 modifiers:

-  `app/Modifiers/GetVideoId.php`
-  `app/Modifiers/IsVimeo.php`
-  `app/Modifiers/IsYoutube.php`


## [What is a fieldset?](https://github.com/statamic/v2-docs/blob/master/content/collections/docs/fieldsets.md#what-is-a-fieldset-what-is-a-fieldset)

A _fieldset_ is YAML file that defines a list of fields used to create content. They're reusuable, highly configurable, and the cornerstone of a customized and tailor-fit Control Panel.

Your fieldsets are kept in the `site/settings/fieldsets` directory. The main section of a fieldset is the `fields` key which allows you to set and configure any number of fields utilizing any combination of the available [fieldtypes](https://github.com/statamic/v2-docs/blob/master/fieldtypes).

An example of what a fieldset might look like:

```
title: Blog Post
fields:
  content:                # The template tag, i.e. {{ content }}
    display: Content      # The CP field label
    type: markdown        # The fieldtype
    instructions: Write!  # Instructional text
    validate: required    # Validation rules
  author:
    display: Author
    type: users
    default: current
    max_items: 1

```

## Change Log
All notable changes to this project will be documented in the [changelog file](CHANGELOG.md).
 
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).
[Sample CHANGELOG ](https://gist.github.com/juampynr/4c18214a8eb554084e21d6e288a18a2c).