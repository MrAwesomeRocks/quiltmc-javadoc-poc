---
layout: post
title:  "First javadocs are added!"
date:   2021-06-21 19:31:20 -0500
categories: jekyll update
---

The first Javadocs have been added to the site! 🎉

The listing for the Javadocs can be found on the [homepage]({{ site.baseurl }}{% link index.markdown %}), and will dynamically generate based on the javadocs listed in `_config.yml`.

To add new Javadocs, there are three steps:
1. Create a new entry in `_config.yml` with a formatted name of the artifact.
2. Add the lowercase name of the artifact to the Github Action.
3. Generate the initial Javadoc using the following commands:
    ```sh
    $> cd docs
    $> curl https://maven.quiltmc.org/service/rest/v1/search/assets/download?repository=release&group=GROUP_ID&name=AFTIFACT_ID&maven.classifier=javadoc&sort=version -o javadoc.jar
    $> unzip javadoc.jar -d AFTIFACT_ID  # ARTIFACT_ID should be lowercase
    $> rm javadoc.jar
    $> git add .
    $> git commit
    $> git push
    ```
