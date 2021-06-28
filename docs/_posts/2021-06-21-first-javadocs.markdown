---
layout: post
title:  "First javadocs are added!"
date:   2021-06-28 10:19:12 -0500
categories: jekyll update
---

The first Javadocs have been added to the site! 🎉

The listing for the Javadocs can be found on the [homepage]({{ site.baseurl }}{% link index.markdown %}), and will dynamically generate based on the javadocs listed in `_config.yml`.

To add new Javadocs, there are three steps:
1. Create a new entry in `_config.yml` with a formatted name of the artifact.
2. Add the lowercase name of the artifact to the Github Action.
3. Push your changes to Github
4. Run the `Update Docs` Github Action through the manual trigger.
5. Check if your new docs appear on the site!
