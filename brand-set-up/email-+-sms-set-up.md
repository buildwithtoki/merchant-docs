# 📩 Email + SMS Set Up

**There are six core events we recommend setting up first.**&#x20;

* Joined Program
* Program announcement
* Referral Completed&#x20;
  * Re-engage Social Activities
* Reward Tier Earned
  * Collected but didn’t redeem
* Redemption Created (aka coupon code from reward tier used)
  * Refer a friend
* Points Earned
  * Push to next highest tier
  * Send to a friend
  * Exchange Notification
* Points Reminder (Sent to inactive customers who have points but not enough to redeem a reward.)
* Redemption Reminder (Sent to inactive customers who have enough points sitting in their account to redeem a reward.)

**Properties we support:**

* Toki\_points\_earned: The customer's total historical points earned
* toki\_point\_balance (if you are using points-as-credit, see below): The customer's current available points balance that they can use now,
* Toki\_tier\_name: The name of the tier the customer is in now
* Toki\_loyalty\_nt\_points: The number of points the customer must earn in order to proceed to the next tier.
* Toki\_nt\_amount: The amount the customer must spend in order to proceed to the next tier. This property will show the default currency defined in your account settings.
* Toki\_referral\_link: The customer's unique referral link. If you are running a code-based referral program, see below for attributes for code-based referrals.
* Toki\_has\_account: True/False depending on if the customer has an account with the platform or not.
* Toki\_referrer\_email: The email of the customer to send the referral to the friend.
* toki\_referrer\_name: The first name + last name of the advocate (if that information is available).
* toki\_${CHALLENGE\_NAME}challenge\_completed\_at: The challenge that this customer has completed
* toki\_voting\_activity\_${ACTIVITY\_NAME}: The answer that the customer gave for the voting activity OR zero party data activity completed (we know this is a little confusing!)
* apple\_wallet\_download\_url: This will be replaced with a link to download the your users Apple Wallet pass



**Here is a view of what these properties look like on an Audience profile in Klaviyo.**

{% embed url="https://loom.com/share/98ddc3dcae444b5eb9517e8fea520034?sid=9f34b78c-32c1-46bb-ada7-0cdb25d65647" %}

&#x20;

**Events we support:**

* Toki Points Earned: This event is triggered any time a customer earns points; This event is commonly used for: keeping a customer's point balance up to date in your CRM or email marketing platform.&#x20;
* Toki Points Reminder: This event is triggered after a certain amount of days of inactivity. The Points Reminder events will be triggered each day at 5 pm UTC
* Toki Redemption Reminder: This event is triggered after a certain amount of days of inactivity. This event is commonly used for: sending an email to remind the customer that they have enough points for a reward.
* Toki Redemption Created: This event is triggered any time a customer redeems points and receives a coupon code. When the customer does not explicitly receive a coupon code, during redemption at checkout, for example, this event will not fire.
* Toki Referral Completed: This event is triggered any time a customer refers a friend that satisfies the referral program requirements. This event is commonly used for: sending an email thanking the customer for the referral.
* Toki Tier Earned: This event is triggered when a customer meets the requirement for a new tier.This event is commonly used for: letting a customer know they reached a certain status level.
* Toki Tier Lost: This event is triggered when a customer fails to meet the requirement for a tier after the specified period of time has passed. This event is commonly used for: sending a "warning" a set period of time to let the customer know they are about to lose their tier if they don't step up their participation.
* Toki Tier Status Changed: This event is triggered when a customer gets closer or farther from retaining their current tier, and from entering the next tier. This event is commonly used for creating incentives by notifying customers "You only need X more points to reach the next tier"
* Toki Account Created: The event is triggered when a reward was given to a customer for creating an account using the Create Account earning rule. This event is commonly used: if you want to do a Welcome Series for new users.
