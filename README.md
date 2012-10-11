



## HTML payment buttons

Integrating with our HTML payment buttons are as easy as including a snippet of code. We have two flavors of buttons for you to use:

### Buy Now
Buy Now buttons are for single item purchases.

```html
<script src="paypal.js?merchant=MERCHANT_ID"
    data-type="buy"
    data-item_name="Buy me now!"
    data-amount="1.00"
></script>
```


### Add To Cart
Add To Cart buttons lets users add multiple items to their PayPal cart.

```html
<script src="paypal.js?merchant=MERCHANT_ID"
    data-type="cart"
    data-item_name="Add to cart!"
    data-amount="1.00"
></script>
```

## Button parameters
You can pass additional data values to the button as well. The following are currently supported:

**Item details**
* `data-item_name` Description of the item
* `data-item_number` The number of the item
* `data-quantity` Number of items
* `data-shipping` The cost of shipping this item
* `data-shipping2` The cost of shipping each additional unit of this item
* `data-tax` Transaction-based tax override variable

**Discounts** 
* `data-discount_amount` Discount amount associated with an item
* `data-discount_amount2` Discount amount associated with each additional quantity of the item
* `data-discount_rate` Discount rate (percentage) for an item
* `data-discount_rate2` Discount rate (percentage) for each additional quantity of the item
* `data-discount_num` Number of additional quantities of the item to which the discount applies
