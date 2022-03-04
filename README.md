# Docuss

A comment/discussion/collaboration system for websites and web apps.

> ### **This project is not active anymore**. 
> You might want to check [DiscPage](https://github.com/sylque/discpage), which shares a lot of features with Docuss.
 
## Features

- Add comments **or full discussion topics** to your web pages
- Create **menus or buttons with attached comments/discussions**
- Supports Wordpress out of the box

## Live Demo

- ~~**Mustacchio**: a fake website demonstrating most Docuss features~~

<p align="center"><a href="http://www.docuss.org">
  <img src="mustacchio.png">
</a></p>

## Other Demos

- ~~**WorDPress**: a fake Wordpress blog, with comments added to Post headings and discussions added to Pages.~~
- ~~**OpenStack**: a single page from a live\* website, with discussions added to each heading~~
- ~~**Discuss The Web**: a sample Meteor+React web app.~~

## How It Works

Docuss allows to integrate your website (or web app) with
[Discourse](https://www.discourse.org/), the popular open-source discussion
platform. Docuss is composed of a plugin running in your Discourse forum and a
JavaScript library running in your web pages.

## Project Status

Docuss is in prototype phase. Please report any idea or issue in the above
`Issues` tab.

# How To Use It

## "I just want to see if it really works"

1. Set up your [Discourse](https://www.discourse.org/) instance (see the
   installation manual
   [here](https://github.com/discourse/discourse/blob/master/docs/INSTALL.md))
   with SSL (see SSL setup [here](https://meta.discourse.org/t/how-to-set-up-ssl-in-discourse/56577)).
2. Install the [Docuss plugin](https://github.com/sylque/dcs-discourse-plugin)
   in your Discourse instance, and set it up with this JSON description file:
   `https://sylque.github.io/dcs-client/demos/mustacchio/dcs-website.json`
3. You should see the _Mustacchio_ demo running smoothly within your Discourse
   instance (with the exception of the menu bar, as explained
   [here](https://github.com/sylque/dcs-discourse-plugin#website-navigation))

## "I'm convinced, I want to integrate my website"

You will need:

- A server running a [Discourse](https://www.discourse.org/) instance (see the
  installation manual
  [here](https://github.com/discourse/discourse/blob/master/docs/INSTALL.md)).
- A server hosting your website or web app.

Docuss installation:

1. Add a [Docuss client library](https://github.com/sylque/dcs-client) to your
   website pages (if your website is a Wordpress blog, this can be done
   automatically for you by the
   [dcs-wordpress-plugin](https://github.com/sylque/dcs-wordpress-plugin)).
2. Create a
   [JSON description file](https://github.com/sylque/dcs-website-schema) and
   host it alongside your website.
3. Install the [Docuss plugin](https://github.com/sylque/dcs-discourse-plugin)
   in your Discourse instance and set it up with your JSON description file.

# License

All Docuss components are released under the [MIT](LICENSE) license.



<br /><br /><br /> ---<br /> \* _Demos targeting live websites use a specific
proxy server to inject a Docuss client library into pages. This proxy is not
available yet._
