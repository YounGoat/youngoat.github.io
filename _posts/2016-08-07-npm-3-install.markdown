---
layout: post
title:  "Why npm 3 installation so slow?"
date:   2016-07-07
categories: diary
---

*What happens when command "npm install" invoked?*

The answer just lies in the manual page for npm install command. Run ```npm help install``` and see the "ALGORITHM" section.

```bash
npm help install
# ...
# load the existing node_modules tree from disk
# clone the tree
# fetch the package.json and assorted metadata and add it to the clone
# walk the clone and add any missing dependencies
#   dependencies will be added as close to the top as is possible
#   without breaking any other modules
# compare the original tree with the cloned tree and make a list of
# actions to take to convert one to the other
# execute all of the actions, deepest first
#   kinds of actions are install, update, remove and move
# ...
```
