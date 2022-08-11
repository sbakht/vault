---
id: vu6fxzr1qp8dnsuaiqxa2to
title: Orderconfirmation
desc: ''
updated: 1660233867287
created: 1660233772609
---

# how to debug order confirmation data

checkoutable products: https://confluence.federated.fds/display/Productivity/TDM+Data#TDMData-PayPalPayment: 

https://www.mcom-121.tbe.zeus.fds.com/shop/product/villeroy-boch-french-garden-dinner-plate?ID=1494&CategoryID=53629&cm_kws=1494

American Express    	 341111597242000  	12/22	1154

put debugger on OrderConfirmationView.js

Example data:
{
    "bag_shipping_eligibility": "standard:premium:express",
    "bag_shipping_selected": "standard",
    "customer_loyalty_id": "",
    "customer_loyalty_tier": "",
    "free_ship_threshold": "24.99",
    "free_ship_threshold_met": false,
    "holiday_eligibility": [],
    "impression_data": [],
    "is_big_ticket": [
        "false"
    ],
    "is_order_gift": "false",
    "opt_in_sdd_sms": "false",
    "order_ccfpEligible": [
        "false"
    ],
    "order_currency": "USD",
    "order_cvv_flag": "false",
    "order_discount": "28.01",
    "order_email": "rotk13@gmail.com",
    "order_id": "698347670064",
    "order_money_earned": "0",
    "order_money_spent": "0.00",
    "order_payment_amounts": [
        "30.30"
    ],
    "order_payment_types": [
        "American Express"
    ],
    "order_pickup_type": "",
    "order_promocode": "",
    "order_sub_total": "27.99",
    "order_tax": "2.31",
    "order_total": "30.3",
    "order_total_items": "1",
    "order_total_primary": "30.30",
    "order_total_secondary": "",
    "page_name": "",
    "page_type": "order confirmation",
    "pdd_availability_message": [],
    "pickup_eligibility": [
        "NA"
    ],
    "product_bops_flag": [
        "false"
    ],
    "product_boss_flag": [
        "false"
    ],
    "product_brand_id": [
        "1327"
    ],
    "product_brand_name": [
        "Villeroy and Boch"
    ],
    "product_category_id": [
        "53629"
    ],
    "product_category_name": [
        "Dining - Dinnerware"
    ],
    "product_color": [
        "Orange"
    ],
    "product_discount": [
        "28.01"
    ],
    "product_fulfillment_method": [
        "ship"
    ],
    "product_gwp_flag": [
        "false"
    ],
    "product_id": [
        "1494"
    ],
    "product_insurance_fee": [
        ""
    ],
    "product_name": [
        "Villeroy & Boch  French Garden Dinner Plate"
    ],
    "product_original_price": [
        "56.0"
    ],
    "product_price": [
        "27.99"
    ],
    "product_promo_discount": [
        ""
    ],
    "product_pwp_flag": [
        "false"
    ],
    "product_quantity": [
        "1"
    ],
    "product_recycling_fee": [
        ""
    ],
    "product_registry_flag": [
        "false"
    ],
    "product_registry_number": [
        ""
    ],
    "product_removal_fee": [
        ""
    ],
    "product_shipping": [
        "0"
    ],
    "product_shipping_eligibility": [
        "standard:premium:express"
    ],
    "product_shipping_method": [
        "standard"
    ],
    "product_shipping_selected": [
        "standard"
    ],
    "product_shipping_surcharge": [
        ""
    ],
    "product_size": [
        ""
    ],
    "product_sub_total": [
        "27.99"
    ],
    "product_upc": [
        "5450102345397"
    ],
    "protection_plan_purchased": [
        ""
    ],
    "sdd_instructions_entered": "false",
    "secondary_order_id": "",
    "shipping_options_available": "",
    "shipping_options_select": "",
    "shipping_value": "0.0",
    "subscription_product_flag": []
}