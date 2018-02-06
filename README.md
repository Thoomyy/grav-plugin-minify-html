# Minify Html Plugin

**Minify Html** is for [Grav CMS](http://github.com/getgrav/grav). Minify HTML output.

## Installation

Installing the Minify Html plugin can be done in two ways. The GPM (Grav Package Manager) installation method enables you to quickly and easily install the plugin with a simple terminal command, while the manual method enables you to do so via a zip file.

### GPM Installation (Preferred)

The simplest way to install this plugin is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's terminal (also called the command line). From the root of your Grav install type:

    bin/gpm install minify-html

This will install the Minify Html plugin into your `/user/plugins` directory within Grav. Its files can be found under `/your/site/grav/user/plugins/minify-html`.

### Manual Installation

To install this plugin, just download the zip version of this repository and unzip it under `/your/site/grav/user/plugins`. Then, rename the folder to `minify-html`. You can find these files on [GitHub](https://github.com/jimblue/grav-plugin-minify-html) or via [GetGrav.org](http://getgrav.org/downloads/plugins#extras).

You should now have all the plugin files under

    /your/site/grav/user/plugins/minify-html

> NOTE: This plugin is a modular component for Grav which requires [Grav](http://github.com/getgrav/grav) and the [Error](https://github.com/getgrav/grav-plugin-error) and [Problems](https://github.com/getgrav/grav-plugin-problems) to operate.

## Configuration

Before configuring this plugin, you should copy the `user/plugins/minify-html/minify-html.yaml` to `user/config/plugins/minify-html.yaml` and only edit that copy.

Here is the default configuration and an explanation of available options:

```yaml
enabled: true
```

## Usage

You just have to enable the plugin to minify the HTML content.
You can see the result by looking at the source in the browser console.

## Compression mode

You can choose between 3 compression mode:

* default compress JS and CSS but doesn't do it aggressively to get the smallest size.
* Fastest only compresses HTML and ignores the rest.
* Smallest compress everything aggressively to get the smallest size.
