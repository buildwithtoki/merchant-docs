# 🍭 Isolated Spending Module

**Overview**

The Isolated Spending Module is a way for your users to actually spend their tokens to get free products. This is super cool because you can basically set up a whole collection or area of your store where customers can specifically purchase products with loyalty tokens!&#x20;

To set this up, you will need to set up a Isolated Spending Rule within your merchant portal (as described before here) and then you will need to set up a Global Spending Module on the product pages + collection page you would like to allow this on.&#x20;

**How to**

After setting up your rule in the merchant portal, you will need to make sure you are reading to set up the module. We suggest actually creating product duplicates so you can keep track of the inventory for free products. As you will see in the below video, our original product "Chill Feelings" is in the regular "Shop" collection; however, we made a duplicate called "Chill Feelings - Special" which is in the "Exclusive Members Shop", the latter both of which have Isolated Rules applied to them.

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

We customize both to our liking.&#x20;

And voila!





