# blog

## Quick start development

Make sure you have `yarn` and the latest version of [hugo](https://gohugo.io/getting-started/installing/) installed on your local machine.

```bash
yarn install
yarn serve
```

## Recommended VS code plugins

* Spellchecker by Michael Vernier
* Markdown All in One by Yu Zhang
* Eslint by Microsoft

## Check for broken links

In one terminal start the server on `localhost:1313`

```bash
yarn serve
```

Then run the check in another terminal:

```bash
make buildscripts && ./bin/linkcheck
```

It will print any issues.

## Shortcodes

Use the following scripts to manage global shortcodes.

### Build the scripts

```bash
make buildscripts
```

### Add a SHORTCODE to all posts at the end of SECTION_NUMBER

```bash
./bin/addshorts SHORTCODE SECTION_NUMBER
```

### Remove SHORTCODE from all posts

```bash
./bin/rmshorts SHORTCODE
```
