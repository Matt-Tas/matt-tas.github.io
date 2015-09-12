---
layout: post
title: Eliminate bad data with extreme prejudice - referral spam
published: true
---

A good way that most people can block Spam Referrals using a Segment. For power users they can use [Simo Ahava's spam filter insertion tool](http://www.simoahava.com/analytics/spam-filter-insertion-tool/)

[Analytics edge post on creating a filtered segment](http://www.analyticsedge.com/2015/01/advanced-segment-eliminate-spam-referrals/)

The rough guide: 
1. Create a new segment named *company name* Referral Filter
2. Filter > sessions > include > Hostname + matches regex + "companywebsite.com.au"
3. Filter > sessions > exclude > Medium + exactly matches + referral - AND - Source - matches regex > spamreferralwebsite.com|spamreferralwebsite.com
4. Limit domain listing to 4 before creating a new (or) then source + matches regex + domain|domain