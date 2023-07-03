---
description: What is a token shop, and how do you set it up?
---

# 🍭 Token Shop + Isolated Spending

**Overview**

Setting up a Token Shop is a way for your customers to buy products _exclusively_ with their tokens or store credit - no cash needed. There's a few things needed to set this up.&#x20;

1. Isolated Spending Rule - learn how to set up [here](../../onboarding-checklist/redemption-aka-redeem/spending-rules/isolated-spending.md)
2. Isolated Spending Module - learn how to design it [here](../../onboarding-checklist/redemption-aka-redeem/spending-rules/)
3. Token Shop - set up in Shopify



**How to set up a Token Shop**

1. Create a new collection, called "isolated" or "token shop". This is the name of the collection that you will attach to your rule in the merchant portal&#x20;
2. Add the products you want to this collection\
   \
   \*We suggest creating product duplicates so you can keep track of the inventory for free products\*&#x20;
3. Create a separate template for product pages and collection pages that relate to an Isolated Rule. We suggest calling it "isolated-product"/"isolated- collection or "token-shop-product"/"token-shop-collection"&#x20;
4. Add the Isolated Spending Module to the isolated-product page.
5. Add the Price Mask to the isolated-product page and the isolated-collection page.

```
//    <div class="toki-price-tag-mask">
    {% raw %}
{% for collection in product.collections %}
      <div
        data-collectionId="{{ collection.id }}"
        data-moneyPrice="{{ money_price }}"
        data-price="{{ price }}"
      >
      </div>
    {% endfor %}
{% endraw %}  
    </div>
```

See a video below:

{% embed url="https://www.loom.com/share/3747e1938943413584386af35fa8f867" %}

As you will see in the video, our original product "Chill Feelings" is in the regular "Shop" collection; however, we made a duplicate called "Chill Feelings - Special" which is in the "Exclusive Members Shop", the latter both of which have Isolated Rules applied to them.

Customize both however you see fit!&#x20;





