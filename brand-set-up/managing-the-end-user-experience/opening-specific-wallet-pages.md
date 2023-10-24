---
description: How to drive users to a specific wallet page.
---

# 😆 Opening Specific Wallet Pages

Looking to drive users to a specific wallet page? Look no further..&#x20;



**Steps for structuring:**

1. Use the following template\
   `{{your-link-with-toki-wallet}}?toki-owp-{{path}}`\
   \
   `toki-owp`- this parameter sets the initial page on which the wallet will be opened when someone opens it
2. Replace `{{your-link-with-toki-wallet}}`- with the link where you placed the wallet
3. Replace `{{path}}` to the path inside the wallet on which page you want to open the wallet

For example (if you want this to open on a new page):

[https://peakskis.com/pages/thank-you-for-purchasing-peak-skis?toki-owp=/home/activity/9a60de6f-8f25-4f7e-a4ce-a1cfd46f1e21\&with\_toki\_wallet=1](https://peakskis.com/pages/thank-you-for-purchasing-peak-skis?toki-owp=/home/activity/9a60de6f-8f25-4f7e-a4ce-a1cfd46f1e21\&with\_toki\_wallet=1)

For example (if you want this to open on the same page):

\#toki-open?toki-owp=/home/activity/e64ff0f6-59c9-402e-8790-72277b4e9760\


**Here are a list of available paths:**

* `/home`- home page (the first tab)
* `/home/earn`- Ways To Earn page
* `/home/activiies` - will open the wallet on the activity list
* `/home/activity/{{activity_id}}` - will open the wallet on a specific activity
  * You can find your Activity ID on the Rewards Activities page as the third column from the right
* `/home/challenges`- Challenges page
* `/home/voting-activities`- Voting Activities page
* `/home/voting-activity/{{id}}`- specific voting activity
* `/profile` - Profile page (the fourth tab)
* `/profile/edit` - the fifth tab
* `/reward-overview` - the second tab
* `/transactions` - the third tab
* `/credits/spend` - the fourth tab
