# MoMedia Theme for Felix Felicis

This is the latest version of the momedia theme for Felix Felicis.
Inspired by the original moment theme


## Installation

Requires Felix Felicis 3.0+


### Install with liquidluck

```
$ liquidluck install systemizer/momedia
$ liquidlcuk install systemizer/momedia -g
```

### Install by yourself

Git clone this repo, and place it in your blog:

```
your_blog/
    settings.py
    content/
    _themes/
        momedia/
```

### Install with git submodule

You can use git submodule for convience:

```
$ git submodule add git://github.com/lepture/liquidluck-theme-momedia.git _themes/momedia
```

## Configuration

Edit your settings, change your theme to ``momedia``.

## Customize

You can customize your theme with ``theme.vars``.

+ Google Analytics

```python
theme = {
    'vars': {
        'analytics': 'UA-xxxx',
    }
}
```

+ Tagcloud support, active tagcloud:


## 404

You can create a file in your source directory (``content``) named ``404.md``.

```
# 404

- template: 404.html

----------------

You content here.
```

Configure your nginx, add:

```
error_page 404 /404.html;
```