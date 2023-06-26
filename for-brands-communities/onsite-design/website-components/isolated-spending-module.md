---
description: What is a token shop, and how do you set it up?
---

# 🍭 Token Shop + Isolated Spending

**Overview**

Setting up a Token Shop is a way for your customers to buy products _exclusively_ with their tokens or store credit - no cash needed. There's a few things needed to set this up.&#x20;

1. Isolated Spending Rule - learn how to set up here
2. Isolated Spending Module
3. Token Shop&#x20;



**How to Design the Spending**

After setting up your Isolated Spending Rule, design the module in the Merchant Portal&#x20;

1.

    **How to Design the Spending Module**

    1. From the merchant portal, Click Design from the sidebar
    2. Click "Create Design"
    3. Write the name of the module you are creating - "Global Spending"
    4. Select "Global Spending Module" from the list
    5. Use the settings in the designer to customize what this looks like - text, colors, images, shape of the buttons, etc!

\*We suggest actually creating product duplicates so you can keep track of the inventory for free products\*&#x20;

As you will see in the below video, our original product "Chill Feelings" is in the regular "Shop" collection; however, we made a duplicate called "Chill Feelings - Special" which is in the "Exclusive Members Shop", the latter both of which have Isolated Rules applied to them.

{% embed url="https://www.loom.com/share/3747e1938943413584386af35fa8f867" %}

Once the duplicates have been created, you must add them to their own collection. This is the collection that you have attached to your rule in your merchant portal.&#x20;

You want to make sure that you have a separate template for product pages and collection pages that relate to an Isolated Rule. We have created a new product template here called "isolated-product" and a new collection template called "isolated- collection".&#x20;

We then specifically add the Isolated Spending Module to the isolated-product page.

We then add the Price Mask to the isolated-product page and the isolated-collection page.

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

Customize both however you see fit!&#x20;

And voila!





