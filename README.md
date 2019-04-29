# Docuss

Docuss allows to integrate your website (or web app) with your Discourse forum.

![Schema](schema.jpg)

Benefits :

- Smoother user experience
- Website/forum interactions: discuss a page, discuss parts of a page, etc.

Docuss is in prototype phase. Please report ideas and issues in the above
`Issues` tab.

# Demos

## Main Showcase

> <a href="http://www.docuss.org" target="_blank" title="Click top open the demo">
> <img src="https://sylque.github.io/dcs-client/demos/mustacchio/images/logo.jpg" alt="Mustacchio" width="130" />
> </a>
>
> [Mustacchio](http://www.docuss.org) is a fake website demonstrating most
> Docuss features. The original website (i.e. before its integration with
> Discourse) is hosted
> [here](https://sylque.github.io/dcs-client/demos/mustacchio/).

## Other demos

> <a href="http://www.docuss.org/docuss/d_home" target="_blank" title="Click top open the demo">
> <img src="https://sylque.github.io/discuss-the-web/public/logo.png" alt="Discuss The Web" width="130" />
> </a>
>
> Sample Meteor+React web app. See the repo
> [here](https://github.com/sylque/discuss-the-web).

> <a href="http://www.docuss.org/docuss/openst" target="_blank" title="Click top open the demo">
> <img src="https://www.openstack.org/themes/openstack/images/openstack-logo-full.svg" alt="Discuss The Web" width="120" />
> </a>
>
> Open source project governance document. Single page of a live\* website, with
> discussions added to each heading. The original website is
> [here](https://docs.openstack.org/contributors/common/governance.html).

\* _Demos targeting live websites use a specific proxy server to inject a Docuss
client library into pages. This proxy is not available yet._

# How to use it

## "I just want to see if it works"

1. Set up your [Discourse](https://www.discourse.org/) instance (see the
   installation manual
   [here](https://github.com/discourse/discourse/blob/master/docs/INSTALL.md)).
2. Install the [Docuss plugin](https://github.com/sylque/dcs-discourse-plugin2)
   in your Discourse instance and set it up with this JSON description file:
   `https://sylque.github.io/dcs-client/demos/mustacchio/dcs-website.json`
3. Check that the Mustacchio demo runs correctly within your Discourse instance
   (however, you won't see the main menu, as explained
   [here](https://github.com/sylque/dcs-discourse-plugin2#website-navigation))

## "I really want to integrate my website or web app"

You will need:

- A server running a [Discourse](https://www.discourse.org/) instance (see the
  installation manual
  [here](https://github.com/discourse/discourse/blob/master/docs/INSTALL.md)).
- A server hosting your website or web app.

Docuss installation:

1. Add a [Docuss client librarie](https://github.com/sylque/dcs-client) to your
   website pages.
2. Create a
   [JSON description file](https://github.com/sylque/dcs-website-schema) and
   host it alongside your website.
3. Install the [Docuss plugin](https://github.com/sylque/dcs-discourse-plugin2)
   in your Discourse instance and set it up with your JSON description file.

# License

Docuss components are released under the
[Fair Source 30 license](https://github.com/sylque/docuss/blob/master/LICENSE)
(additional information [here](https://fair.io/)).

Notice that dcs-discourse-plugin2 is released with minified source code only.
This may or may not change in the future.
