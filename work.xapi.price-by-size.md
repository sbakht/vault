---
id: 2d93b7a1-50f0-48df-9d9e-81ab4fd5fa90
title: Price By Size Products
desc: ''
updated: 1635960714032
created: 1635960460582
---

## TLDR
Masters product can (must?) be the same product as one of the product ids. So the master IS a member. On PDP the master/member id will render the same product + default size. On discovery the master product id will show the master collection + price range, but the member id will show that given member product.

**These are called Price By Size products**

## Conversation

[12:19 PM] Saad Bakht
these are the responses to pdp xapi, small version gives the master product for some reason

[12:20 PM] Saad Bakht
look at this

[12:20 PM] Saad Bakht
https://www.mcom-182.tbe.zeus.fds.com/xapi/digital/v1/product/166248

[12:20 PM] Saad Bakht
https://www.mcom-182.tbe.zeus.fds.com/xapi/digital/v1/product/170830

[12:20 PM] Saad Bakht
2 different ids, both return same product

[12:25 PM] Saad Bakht
so 170830 is the master product, but it looks like master products arent unique, so 1 member can be the same as the master

![](/assets/images/2021-11-03-12-28-11.png)
