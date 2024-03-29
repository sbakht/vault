---
id: 151659f1-419b-412e-ba42-3608058e5cc9
title: Tvpage
desc: ''
updated: 1639083645260
created: 1639080172744
---

https://www.tvpage.com/

https://app.tvpage.com/api/docs/

https://www.macys.com/style-crew/
https://www.macys.com/style-crew/p/clinique-holiday-value-lipstick-set/227703551
https://www.macys.com/style-crew/a/noura-barnes/213627

## Email chain

Architecture

**Can you share a little about the current Macy’s (landing page and influencer storefront integration)?
E.g. Is the sitelet an i-frame integration? …or API?**

There is a reverse proxy pointing to our CDN that allows us to host these pages on the Macy's domain (style-crew subdirectory). We pull in your header/footer.
 
**Also, curious to hear more about the storefronts (e.g. how we’re building and maintaining the individual pages for each creator)**

These pages are created as part of our publishing system. This system generates these pages and publishes contents to Google in the form of a sitemap, as well as generating embed codes, etc. Happy to talk more on our call about this.
 
 

### Data

**Can you share a little about the breakdown of traffic sources
How much is coming from each marketing surface (e.g. FB/IG, Twitter, Email/Text link, etc)**
Historically, traffic has been split about 60/40 social media/google search traffic. With the social media traffic being pretty evenly split between Facebook and Instagram.
 
**How much traffic goes to storefront pages vs the total MSC page
Also, if possible, would love to understand how much sales and conversion comes from the total MSC page vs what might be coming from the storefront pages.**

Conversion on a particular asset/page is a little tough to quantify as we're not looking at single touch sessions. On average we see multiple photo and video views per session. Usually these are for the same creator, as consumers are discovering their content through their storefront or the related content section. From a traffic perspective, I do not have that answer readily available but I should be able to get it pulled for you in the coming days. 

## Documentation

https://tvpage-support.zendesk.com/hc/en-us/articles/4407091516439-Implementing-3rd-party-analytics-events
https://tvpage-support.zendesk.com/hc/en-us/articles/4403030935575-Third-Party-Integrations
https://tvpage-support.zendesk.com/hc/en-us/articles/4403024392727-Reported-Metrics

## Another email

The primary way that we "send" data to our clients is through integration with your analytics system. With this method, we will be mapping the events that we capture to your system and firing them directly from the experiences in real-time.

### Landing page

The primary landing page can be configured/customized to show content and create content navigation in any way that you'd like. 
 
Here are some examples of what other clients are doing:
•	Advance Auto - https://shop.advanceautoparts.com/videos
•	Taylor Guitars - https://www.taylorguitars.com/videos/

### Storefront

Influencer Storefronts do follow a template, wherein much of what is populated in the experience (ie. cover photo, profile image, influencer info, etc.) is provided by the influencer facing app, the merchant back-office, or both. That being said, we're absolutely open to design input and would be willing to explore any customization requirements that Macy's has for these storefronts.

### Getting content onto PDP

Content push to places like the PDP are one of the biggest ways to take advantage of the great content generated by the Style Crew team and put it to work for you. Macy's is currently seeing over $4 in revenue generated from every video view ($4.21 YTD) on top of funnel traffic to this content, and this traffic is converting at 4.41% YTD. The opportunity to get this high-performing content in front of more eyeballs, lower in the funnel is tremendous. We're generating in excess of $100M in video attributed revenue annually for some of our larger clients, and are highly confident we could meet or exceed that for you.

#### Two ways

Using a TVP widget that can be customized to fit any experience you would like. Examples below.

- https://www.academy.com/shop/pdp/bowflex-selecttech-1090-adjustable-dumbbell	
-	https://www.autozone.com/filters-and-pcv/cabin-air-filter/p/stp-max-cabin-air-filter-caf90168m/1068799_0]
-	https://www.moon-audio.com/meze-liric-closed-back-headphone.html - 2 widgets on page

Here are some potential designs that our team created for what one of these widgets could look like on a Macy's PDP:

https://projects.invisionapp.com/share/H310PY1KUVJ2#/screens
https://projects.invisionapp.com/share/VN10RYTAHW7M#/screens/
https://projects.invisionapp.com/share/3N122C5EQ9KF#/screens/
https://projects.invisionapp.com/share/FVZWIQEJN6Q#/screens

Using our content feed to get the data you need to create any experience that you would like. Examples below.

- https://www.bedbathandbeyond.com/store/product/vitamix-reg-8-oz-blending-bowl-kit/5263019
- https://www.crutchfield.com/S-WsDuGZRBUUm/p_070XDM270/Dual-XDM270.html

## Api

As mentioned above, we have a feed of content data that can enable you to create any custom experience, for PDP or elsewhere. I've attached the documentation for that feed (XML, but could also be JSON). An additional non-PDP example of how this is used to create custom experiences and landing pages below:

https://www.bedbathandbeyond.com/store/static/beforethemove
