---
title: Merchants
weight: 80
---

## Create merchant

In your Joomla! back-end, go to `Components` -> `CM Coupon Listing` -> `Merchants` to access the list of merchants on the site

![](/images/backend_merchant_list.jpg)

Click `New` button on the toolbar to create a new merchant.

![](/images/backend_merchant_form.jpg)

A merchant has the following data:

* **Name**: Merchant's name.
* **Alias**: Merchant's alias for search engine friendly URL. An alias is created automatically if you don't provide any alias when you create or edit merchant.
* **Manager**: A Joomla! user who manages merchant. This Joomla! user has ability to edit merchant's profile and coupons in front-end.
* **Categories**: Categories of products/services that merchant provides.
* **Overview**: A short overview of merchant.
* **Logo**: Merchant's logo.
* **Address**: Merchant's address.
* **Website**: Merchant's website.
* **Phone**: Merchant's phone number.
* **Featured**: Merchant is featured. Coupons of featured merchants could be displayed on the top of coupon lists, you can configure this in the component's configuration.
* **Published**: Merchant and merchant's coupons are displayed in front-end if merchant is published.
* **Active**: If merchant is inactive, Joomla! user who manages merchant can't manage profile and coupons in front-end any more. Inactive merchant and his/her coupons are still displayed in front-end.
* **ID**: Record number in database.

## Merchant registration

User can register as a merchant on your site via Merchant Registration menu item.

![](/images/merchant_registration_form.jpg)

### Guest

A guest can register as a merchant and as a Joomla! user at the same time.

When a guest registers, Joomla! notification and activation mails could be sent to user and administrators, this depends on your configuration for Users component. Go to your back-end, User Manager, click Options button on toolbar to configure Users component.

### Registered user

Registered user can login and then register as a merchant.

A user can only manage 1 merchant. If a user who already manages a merchant access registration form, he/she receives an error message.

### Send activated notification mail

When a user registers as a merchant, a merchant is created automatically in CM Coupon Listing, however this merchant is inactive. You can edit inactive merchant, set it to `Active`, then press `Send activated notification mail` button on merchant edit page, an email is sent to merchant to notify him/her that his/her merchant account is now active and he/she can submit coupon now.

You can customize the content of activated notification mail in the language file of CM Coupon Listing component.

### Edit profile

You need to create a menu item for `Merchant management area` page, this is where merchant manage his/her coupons and the profile information.

![](/images/merchant_dashboard.jpg)

Access the page, merchant can see an overview of the merchant's profile and coupons. To edit the profile merchant click `Edit profile` button.

![](/images/merchant_profile_form.jpg)
