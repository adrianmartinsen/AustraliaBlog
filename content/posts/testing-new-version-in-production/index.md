---
title: Testing new version in production
date: 2024-12-31T18:06:00+01:00
---
Changed the build version to 125.7 which is the lowest possible version that PaperMod theme will work with. Let's see if this post shows up.

So it would seem the version was not the issue. After pulling this commit to my local repo it still wouldn't show even on a local server. After noticing the datetime format being slightly different from the manually created posts I changed the datetime (specifically the timezone) to match what the "hugo new content" command makes. After that it showed locally and when pushing the changes it showed on the Netlify site as well. 

I edited the datetime format in the config for the CMS to match what Hugo creates by default and voila! A new post created on the CMS immidiatly showed on the Netlify site.
