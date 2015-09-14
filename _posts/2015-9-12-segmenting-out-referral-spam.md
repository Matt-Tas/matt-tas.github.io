---
layout: post
title: Eliminate bad data with extreme prejudice - referral spam
published: true
---

Spam bots be like, "Hey I'm just going increase my search ranking by having this code visit your site." It doesn't hurt, except it does, by injecting a lot of confusion to those unaware of their site stats.

##IF you don't block this you'll see increasing traffic + increasing bounce rate.

A lot of small business sites probably see this often. It is the first thing a decent SEO does when setting up your Google analytics stuff.

##How to get rid of it 

A good way that most people can block spam referrals is by using a Segment. 

[Analytics edge post on creating a filtered segment](http://www.analyticsedge.com/2015/01/advanced-segment-eliminate-spam-referrals/)

Here is how to do it.

1. Create a new segment named *company name* Referral Filter

2. Filter > sessions > include > Hostname + matches regex + "companywebsite.com.au"

3. Filter > sessions > exclude > Medium + exactly matches + referral - AND - Source - matches regex > spamreferralwebsite.com|spamreferralwebsite.com

4. Limit domain listing to 4 before creating a new (or) then source + matches regex + domain|domain

5. test

For power users they can try using [Simo Ahava's spam filter insertion tool](http://www.simoahava.com/analytics/spam-filter-insertion-tool/)