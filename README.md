# Economy of Effort

### Notes

SCSS building not functional from Octopress 2 import
Need to sort out how to use in pure Jekyll

Rename _sass/ to css/ to use Jekyll's built-in SASS compilation
but @import compass doesn't work (and probably other library-provided sheets after it)
Need to figure out how to replace these library imports with something jekyll likes
and not have it break existing styling

Currently using a scraped CSS file from the old site

When CSS building works, change layout to not use the scraped file anymore

Using YouTube plugin from: https://github.com/erossignon/jekyll-youtube-lazyloading
- copied into _plugins folder
- copied CSS to the end of my scraped CSS file
- edited the plugin to replace ratio-4-3 with ratio-16-9
- also edited the copy-pasted CSS to add margin underneath the video
- added fastimage gem, fetch YouTube thumbnails in descending quality order to find the 
  best quality, instead of just using the shit tier "0.jpg" (the Yt gem only returns default.jpg which is shit tier too)
