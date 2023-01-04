# 🧞 Klaviyo-Specific Activities

**Overview**

**Activities** are automated issuance events that you set up in your Merchant Portal.  Klaviyo is a dream platform to set up 3 different types of automated activities:&#x20;

* Newsletter Sign up
* Sharing your birthday
* Giving feedback

**How to**&#x20;

To create an activity, go to **Reward** on the left menu and then click on **Activities.** Go ahead and click on **Create a new activity** to get started.&#x20;

After choosing naming the activity, choosing the integration and choosing form submission, things get tricky.&#x20;

{% embed url="https://www.loom.com/share/3321370cddc342a5ac84e3891c7e223a" %}

First off, you are going to need to go back into your Klaviyo account to fill out the ‘Form ID’ section. The form ID can be found in the domain as the six digit code within the form you have created in Klaviyo. Copy this code and put in the form submit.&#x20;

Second, you are going to want to make sure that you have set up the button **Action** on the final step to **Submit Form** and then **After Submit** to **Close Form.**

Lastly, when you go back to your Merchant Portal you are going to need to fill out the Token Claim Path. This should link to the claim page you have set up (or if you haven't go here to set it up now). This should not include the entire domain, just the final words after the last forward slash (i.e. /claims-page)

**Keep in mind**

1. You can edit an activity at any time.
2. If you do edit an activity or create a new one, you do need to turn the Status on. When the Status is on, it will be orange.

