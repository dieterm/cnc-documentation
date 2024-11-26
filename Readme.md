# CNC Documentation (hugo website)

## How to use

To start the hugo server, run:

```sh
$ hugo server
```

Then surf to:

http://localhost:1313/

## To deploy on Netlify

Make sure environment variables are set correctly in `\netlify.toml`

```toml
[build.environment]
  HUGO_VERSION = "0.139.0"
  HUGO_BASEURL = "https://gleaming-frangollo-9ef787.netlify.app/"
```

Also make sure to deploy `package.json` to netlify in order to be able to build.

Commit & push code changes to git.</br>
Deploy will start automatically.

https://gleaming-frangollo-9ef787.netlify.app/

## To setup Hugo environment

Hugo & Docsy theme require a number of npm packages.</br>
These dependancies are defined in package.json.</br>
Make sure to deploy `package.json` to netlify in order to be able to build.</br>
Install npm packages locally:

```sh
$ npm install
```

## To build hugo files

First run this command (without arguments):

```sh
$ hugo
```

The output is generated in folder `\public`

## Clean hugo Cache

Sometimes the cache prevents changes from being visible.
To clear the cache files, execute:

```
$ hugo mod clean
```

## Theme "docsy"

The theme 'docsy' is used from https://themes.gohugo.io/themes/docsy/ .

Theme is loaded as git-module from: https://github.com/google/docsy .</br>
See file: `\.gitmodules`

In order to fix the _unsafe html_ issue, add the following to `hugo.yaml`:

```yaml
markup:
  goldmark:
    renderer:
      unsafe: true
```

Some layout files are overwriten to include custom css.</br>
See files in folder: `\layouts\partials\head-css.html` and `\static\css\styles.css`
