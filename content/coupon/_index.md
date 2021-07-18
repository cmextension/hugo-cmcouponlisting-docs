---
title: Coupons
weight: 90
---

## Create coupon in back-end

In your Joomla! back-end, you navigate to `Components` -> `CM Coupon Listing` -> `Coupons`.

![](/images/backend_coupon_list.jpg)

On the toolbar, you click `New` button to create a new coupon.

![](/images/backend_coupon_form.jpg)

* **Name**: Coupon's name.
* **Alias**: Coupon's alias for search engine friendly URL. An alias is created automatically if you don't provide any alias when you create or edit coupon.
* **Short description**: A short description about coupon, it is displayed in coupon list and coupon detail pages.
* **Description**: A detailed description about coupon, it is only displayed in coupon detail page.
* **Type**: Coupon type. There are 4 types: coupon code, printable coupon, sale link and activation link. You can configure what types are used, what types are not used in the component's configuration.

  * **Coupon code**: Coupon is a code to enter when check out.
  * **Printable coupon**: Coupon is an image to print or save to smartphone and bring to merchant.
  * **Sale link**: Coupon is a deal or an offer from a third-party website.
  * **Activation link**: A link to merchant's website which automatically activates discount, no coupon code is required when checkout.

* **Merchant**: Merchant who owns coupon.
* **Categories**: Categories which coupon is in.
* **Starting date and Ending date**: The date when coupon starts valid and the date when coupon expires. Coupon is only displayed in front-end if current date is between these two dates.
* **Featured**: Featured coupons could be displayed on the top of coupon lists, you can configure this in the component's configuration.
* **Published**: Coupon is displayed in front-end if it is published.
* **Access**: Joomla!'s access level group. Only users in selected access level can see and get coupon. This is useful if you want to have some special coupons which are only available for registered users, or users who have already purchased for subscriptions on your site.
* **ID**: Record number in database.

## User submits coupon in front-end

To allow users to contribute coupons to the site, you need to configure some options in `Configuration` section. The most important options is `Access submission page`, it provides the options for access levels, only users in the selected access level can access the form. For example if you select `Public` then all users inluding guests can submit new coupon. If you want to limit access to the form you need to select a different access level, for example you select `Registered` to only allow logged-in users to access the form.

To create new new access level you can do it in your back-end (access Users -> Access Levels on the top menu).

You need to create a menu item for `Coupon submission` page. Visit the page in front-end with an account which is in the configured access level, you can see the form with less fields than the coupon form in back-end. After user submits coupon, you can receive an notification email if you enable it in the component's configuration, you need to log into your back-end, review the coupon, assign it to a correct category and publish it.

![](/images/frontend_coupon_user_form.jpg)

## Merchant manages coupon in front-end

`Merchant management area` menu item is required to allow merchant to manage coupons. To create a new coupon, merchant needs to click `New coupon` button. To delete coupons, merchant needs to select the coupons and click `Delete` button.

![](/images/merchant_dashboard.jpg)

Merchant needs to fill the required fields. After coupon is saved, it is published immediately. If email notification is enabled in the component's configuration, administrators will receive emails for new coupon submission.

![](/images/frontend_coupon_merchant_form.jpg)
