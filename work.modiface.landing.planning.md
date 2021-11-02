---
id: b3ad1436-3241-4841-adf7-74938abf9c4a
title: Planning
desc: ''
updated: 1635860727276
created: 1635860034636
---

## Modiface things we need to add


### Ajax call

Ajax parameters:

	1. Pagination
	2. Sort by
	3. Facets


#### Pagination

&pageIndex=1
&pageIndex=2

&productsPerPage=60
&productsPerPage=120

#### Sort By

&sortBy=ORIGINAL (featured items)
&sortBy=PRICE_LOW_TO_HIGH
&sortBy=PRICE_HIGH_TO_LOW
&sortBy=TOP_RATED
&sortBy=BEST_SELLERS
&sortBy=NEW_ITEMS (new arrivals

#### Facets

pathname=/shop/search/COLOR_NORMAL,PRODUCT_DEPARTMENT/Blue,Boots|Mules

	comma separates facet group
	| separates items within a group


- [ ] keyword
- [ ] region code
- [ ] device type
- [ ] application
- [ ] navigation type
- [ ] shopping mode

#### keyword

#### _regionCode

#### _deviceType

#### _application

#### _navigationType

#### _shoppingMode




https://www.macys.com/xapi/discover/v1/page?pathname=/shop/search/COLOR_NORMAL/Blue&keyword=shoes&_application=SITE&_navigationType=SEARCH&_deviceType=DESKTOP&_shoppingMode=SITE&_regionCode=US&_customerExperiment=565-20,601-23,730-21,752-21,775-21,799-21&currencyCode=USD&_customerState=GUEST&pageIndex=1&productsPerPage=60&sortBy=PRICE_LOW_TO_HIGH&_additionalStoreLocations=5419&_shipFromLocations=10&sessionId=017cb88d208c00180635a660c1d80507800160700093c&visitorId=59418712652014288716973226189909931660&size=medium

https://www.macys.com/xapi/discover/v1/page?pathname=/shop/search/COLOR_NORMAL/Blue&keyword=shoes&_application=SITE&_navigationType=SEARCH&_deviceType=DESKTOP&_shoppingMode=SITE&_regionCode=US&_customerExperiment=565-20,601-23,730-21,752-21,775-21,799-21&currencyCode=USD&_customerState=GUEST&pageIndex=2&productsPerPage=60&sortBy=PRICE_LOW_TO_HIGH&_additionalStoreLocations=5419&_shipFromLocations=10&sessionId=017cb88d208c00180635a660c1d80507800160700093c&visitorId=59418712652014288716973226189909931660&size=medium

https://www.macys.com/xapi/discover/v1/page?pathname=/shop/search/COLOR_NORMAL/Blue&keyword=shoes&_application=SITE&_navigationType=SEARCH&_deviceType=DESKTOP&_shoppingMode=SITE&_regionCode=US&_customerExperiment=565-20,601-23,730-21,752-21,775-21,799-21&currencyCode=USD&_customerState=GUEST&pageIndex=1&productsPerPage=120&sortBy=PRICE_LOW_TO_HIGH&_additionalStoreLocations=5419&_shipFromLocations=10&sessionId=017cb88d208c00180635a660c1d80507800160700093c&visitorId=59418712652014288716973226189909931660&size=medium

https://www.macys.com/xapi/discover/v1/page?pathname=/shop/search/COLOR_NORMAL,PRODUCT_DEPARTMENT/Blue,Boots|Mules&keyword=shoes&_application=SITE&_navigationType=SEARCH&_deviceType=DESKTOP&_shoppingMode=SITE&_regionCode=US&_customerExperiment=565-20,601-23,730-21,752-21,775-21,799-21&currencyCode=USD&_customerState=GUEST&pageIndex=1&productsPerPage=120&sortBy=NEW_ITEMS&_additionalStoreLocations=5419&_shipFromLocations=10&sessionId=017cb88d208c00180635a660c1d80507800160700093c&visitorId=59418712652014288716973226189909931660&size=medium