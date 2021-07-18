---
title: Merchant's Coupons Plugin
weight: 150
---

CM Coupon Listing Merchant's Coupons plugin helps you insert list of coupons from a specific merchant into Joomla! article, `Custom HTML` module or any extension which supports `onContentPrepare` event.

After installing the plugin, you need to enable it to make it working. You can find it in Plugin Manager with the name `Content - CM Coupon Listing Merchant's Coupons`.

In Joomla! article or in the editor of the extension, you insert the following tag:

{cmcouponlisting merchant=XX}

XX is the ID of the merchant in CM Coupon Listing. For example if merchant has ID 10, the tag should be:

{cmcouponlisting merchant=10}

The result is the list of coupons with coupon's name and coupon's short description.

![](/images/cmcouponlistingmerchantcoupon.jpg)