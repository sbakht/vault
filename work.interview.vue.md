---
id: ef0e22b0-2252-4539-bf2c-127bdf021f7a
title: Vue
desc: ''
updated: 1640112569217
created: 1640111304757
---

<img
	v-if="responsePdp && responsePdp.id"
	style="max-width:328px"
	:src="require(`@images/disco-${responsePdp && responsePdp.id}.png`).default"
>


<div
	v-for="(product, i) in products"
	:key="i + '-' + product.id"
	class="cell small-6 medium-4"
>
	<a
		v-if="product"
		:href="product.identifier.productUrl"
	>
		<ProductThumbnail
			class="product"
			:product="product"
			:swatch-url-template="swatchUrlTemplate"
		/>
	</a>
</div>


function formatedListOfSelectedItems() {
	return this.listOfSelectedItems.map(item => ({ id: item.id, title: item.name }));
}



function setAttributes() {
  screen.width = window.innerWidth;
  screen.height = window.innerHeight;
  screen.isMobile = screen.width < 600;
  screen.isTablet = screen.width >= 600 && screen.width < 1024;
  screen.isDesktop = screen.width >= 1024;
}

export default function useDisplay() {
  onMounted(() => {
    if (!screen.width) {
      setAttributes();
      window.onresize = setAttributes;
    }
  });

  return { ...toRefs(screen) };
}


player.on(player.EVENT.ADD_TO_CART, (addedItem, callback) => {
	addToBag({
		item: addedItem,
		callback,
		cookies,
		cookieDomain,
	})
		.then((response) => {
			currentBagGuid = response.bag.meta.bagGuid;
			callback(true);
		})
		.catch(() => {
			callback(false);
		});
});

export const parsePricing = ({ price } = {}) => {
  const { tieredPrice, priceType, finalPrice } = price || {};

  if (!tieredPrice || !priceType) {
    return {};
  }

  const saleMap = getSaleMap(tieredPrice);
  const regularMap = getRegularMap(tieredPrice, priceType);
  const promoMap = getPromoMap(finalPrice);

  const priceBreakdown = {};

  priceBreakdown.flags = priceType;
  priceBreakdown.sale = saleMap;
  priceBreakdown.regular = regularMap;
  priceBreakdown.promo = promoMap;

  return priceBreakdown;
};