---
id: f59202ed-be39-46b5-a4f8-b53c4ae63543
title: API
desc: ''
updated: 1639520408240
created: 1639084402381
---

https://app.tvpage.com/api/docs/#/


## User page

https://www.macys.com/style-crew/a/noura-barnes/213627
user id = 213627

## User generated product page 
GET /v2/api/entity/{clientId}/entity/{videoId}/products
clientId = 1759121 

- https://www.macys.com/style-crew/p/tie-dye-for-the-trevor-project/227205039
- https://app.tvpage.com/v2/api/entity/1759121/entity/227205039/products
- https://app.tvpage.com/api/videos/227205039?X-login-id=1759121 
- https://api.tvpage.com/api/channels/155524390/contents?user_id=213627&X-login-id=1759121&n=24 
	- i dont know where 155524390 comes from
	- n specifies the number of related products
- https://api.tvpage.com/api/accountUser/ambassador/213627?X-login-id=1759121

https://api.tvpage.com/api/channels/155524389/contents?X-login-id=1759121&p=0&n=24&status=approved&_=1639087607159 this is the homepage call, where is the id determined from?

**ID comes from the page source, it is hardcoded based on page type**

Additionally, I wanted to include our documentation on hub customization so that you can see how this comes together to create the experience, and what the possibilities are for customization.

https://tvpage-support.zendesk.com/hc/en-us/articles/4415841959447-TV-Page-Configuration-Guide