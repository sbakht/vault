---
id: e7697034-b9b2-489f-9206-f1e27154405b
title: Refactor
desc: ''
updated: 1640113363496
created: 1640113094725
---

function getPrice(pricing) {
	if(pricing.priceObj.flags.isSale === true) {
		return pricing.priceObj.price.sale.value;
	}else if(pricing.priceObj.flags.isSale === false && pricing.priceObj.flags.isPromo === true) {
		return pricing.priceObj.price.regular.value - pricing.priceObj.saved;
	}else if(pricing.priceObj.flags.isSale === false && pricing.priceObj.flags.isRegular === true) {
		return pricing.priceObj.price.regular.value;
	}

	return 0;
}