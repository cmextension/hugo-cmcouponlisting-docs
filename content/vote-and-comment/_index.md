---
title: Vote and Comment
weight: 110
---

User can vote if a coupon works (good coupon) or doesn't work (bad coupon). While voting, user can also provide information about how much user saves when use the coupon (if coupon is good), or why coupon doesn't work (if coupon is a bad coupon).

You can enable/disable vote and comment, or configure some options of them in `Configuration` section.

## Manage currencies

You only need to use currencies if you enable voting and asking questions in `Configuration` section. If user votes coupon as a good coupon, then user is asked how much user has saved and what item user has bought, this is when currencies is used.

![](/images/coupon_vote_good.jpg)

In your back-end, navigate to `Components` -> `CM Coupon Listing` -> `Currencies` to access the list of currencies.

![](/images/backend_currency_list.jpg)

Click `New` button on the toolbar to create a new currency.

![](/images/backend_currency_form.jpg)

* **Currency name**: You can use currency name, eg. USD, or currency sign, eg. $. This name is only for internal use, it is not visible in front-end.
* **Currency sign**: Your currency's sign/symbol, eg. $.
* **Currency sign's position**: The position of your currency's sign, before or after the amount.
* **Status**: Only published currencies are displayed in front-end.
* **Ordering**: The position of the currency in the currency list.
* **ID**: Record number in the database.

## Manage reasons of bad coupon

If you enable voting and asking questions in :ref:`Configuration <ref-configuration-vote-comment>` section and user votes for a bad coupon, then user is asked why the coupon is bad. You can create some reasons for user to choose.

![](/images/coupon_vote_bad.jpg)

Go to to `Components` -> `CM Coupon Listing` -> `Bad coupon's reasons` in your back-end to access the list of reasons.

![](/images/backend_reason_list.jpg)

Click `New` button on the toolbar to create a new reason.

![](/images/backend_reason_form.jpg)

* **Reason**: The reason.
* **Status**: Only published reasons are displayed in front-end.
* **Ordering**: The position of the reason in the reason list.
* **ID**: Record number in the database.

## Manage votes

Go to to `Components` -> `CM Coupon Listing` -> `Votes` in your back-end to access the list of votes submitted by users.

![](/images/backend_vote_list.jpg)

You can click on the ID of the vote to edit it. You can also create a vote by yourself by clicking `New` button.

![](/images/backend_vote_form.jpg)

* **Coupon**: The coupon which the vote is for.
* **User**: The user who makes the vote. If no user is selected, user is considered as a guest.
* **Vote**: Vote (good or bad coupon).
* **Voted date**: The date when user makes the vote.
* **Status**: Published status.
* **Currency**: The currency that user uses to pay for product/service with the coupon. Only used if the vote is good.
* **Saved amount**: The amount that user saves by using this coupon. Only used if the vote is good.
* **Items**: The items that users pay for by using this coupon. Only used if the vote is good.
* **Reason of bad coupon**: The reason why user votes this coupon bad. Only used if the vote is bad.

## Manage comments

In back-end, to access to comment list you navigate to `Components` -> `CM Coupon Listing` -> `Comments`.

![](/images/backend_comment_list.jpg)

You can edit a comment by clicking its ID. In comment form, we have the following options.

![](/images/backend_comment_form.jpg)

* **Comment**: The content of the comment.
* **Posted date**: The date when the comment is posted.
* **Status**: Published status.
* **User**: The Joomla! user who posts the comment, if commenter is a registered user.
* **Guest's name**: The name of the guest who makes the comment. This value is not used if user is a registered user. If no value given, the word `Anonymous` is used.

## Vote in front-end

If you enable vote in the component's configuration, you can see the vote option for every deal in front-end.

![](/images/coupon_vote.jpg)

If coupon works, you click `Yes`, otherwise you click `No`.

Depending on your configuration, there could be another step asking for how much you save, what items you purchase if coupon is good or why you think the coupon is bad.

After your vote is submitted, you receive the message.

![](/images/coupon_vote_success.jpg)

## Comment in front-end

If you enable comment in the component's configuration, below every deal's detail there is a form for submitting new comment and the list of submitted comments.

![](/images/coupon_comment.jpg)

In the comment list, comments and votes are showed, they are sorted by submitted date, newer comments/votes are displayed first.
