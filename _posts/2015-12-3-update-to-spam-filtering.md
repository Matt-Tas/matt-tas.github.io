---
layout: post
title: Update to spam filtering
published: true
---

Using segments to filter out referral spam has been great... however I have noticed a down side, preventing segments from being used as an analysis tool.

Using a master segment to filter means you can't create segments without having to duplicate all of the filters each time.. not easy. 

##Review of methods

I had used an .htaccess update, which is usually the easiest way to do this as it is file based and manual. The problem with this was that it was still registering as direct traffic. If you had 100 visits, 50 of which were spam bots than you would see a high bounce rate on your referral traffic. The .htaccess adjustment would fling the bots off into the web, but they seem to still be registering as direct traffic by analytics if the settings were wrong.

##Now to testing

I've setup a two new views in analytics. One view filters out office traffic and only allows my hostname, the other view filters out office, not my hostname and referrals from adf.ly.  This will allow me to see if that works. I expect it will block adf.ly. I will then attempt to block it with the .htaccess file and then look at the results. 

###Questions to answer
1. Does the .htaccess method work?
2. Does the .htaccess method slow down web traffic?
3. What are the limits to the .htaccess method?
3. Can the .htaccess method be automated?