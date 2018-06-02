OpenMRS Planet
==============

This repository is used to configure the [RSS](https://en.wikipedia.org/wiki/RSS) feeds for 
[planet.openmrs.org](http://planet.openmrs.org/). The OpenMRS Community uses a feed aggregagator 
hosted by [OSUOSL](https://osuosl.org/). When changes are pushed to the configuration in this
repository, they are automatically deployed by OSUOSL via Jenkins.

## Which feeds are included?

We include any RSS feeds within or outside the community with OpenMRS content. For blogs that may contain 
non-OpenMRS content, we prefer to filter to OpenMRS-related posts (e.g., only posts categorized or tagged 
as OpenMRS).

For example, we add blogs for [Google Summer of Code](https://summerofcode.withgoogle.com/) and blogs of 
community members to the aggregator.

## How do I add my blog or a relevated feed?

Submit a pull request to this repository including the feed. Add it to the bottom of the list following 
the same format – that is, the web addrsess of ATOM or RSS content in square braces followed by a line 
with `name = ` and the title for the feed (e.g., the name of the author):

```
[https://rss.example.com/]
name = Title for the feed here
```

If you aren't sure how to submit a pull request with your feed, then ask for help on 
[OpenMRS Talk](https://talk.openmrs.org) or within our [IRC channel](https://om.rs/irc).

## How to feeds get removed?

You can submit a pull request to remove a feed or ask someone in the community for help. Anyone may 
remove their own blog if they wish and we may occasionally pull out entries that are no longer functional, 
no longer active, or no longer relevant for the OpenMRS community.
