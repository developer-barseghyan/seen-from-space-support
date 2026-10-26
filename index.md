---
layout: default
title: Seen from Space Support
permalink: /
---

# Support

**Seen from Space: Satellite Map** shows a fresh satellite image of any place on Earth every few days, tells you when the next one will be taken, and puts two dates side by side so you can see what changed. For places in the United States it adds sharp aerial photos, year by year back to 2010.

There is no account and no server of mine. Predictions are computed on your iPhone, and your points are stored only on it.

---

## Contact

**developer.barseghyan@gmail.com**

I usually reply within about two business days. If a prediction or an image looks wrong, please read *"A prediction or an image looks wrong"* below before writing, and include what it asks for. It makes the fix much faster.

---

## Before anything else

**Pass times are predictions, and an expected image is not a promised one.** The app computes where each satellite will be from public orbital data and judges each pass against a model of the satellite's sensor. It does not read the operators' real acquisition plans and it does not know about clouds. Images, aerial photos, the vegetation view and reports are for information only: **not a survey, an inspection or a valuation.** Please do not use the app for navigation, safety or any decision where an error could cause harm.

---

## Frequently asked questions

### What is on the Home screen?

The newest clear image of the point you selected, when the next image is expected, and the cloud cover of the latest one. Below it: **Compare**, **Timelapse**, **Vegetation** and **Share**, the aerial photo card for US points, and your recent images. Switch points with the menu at the top left.

The full list of satellite passes lives in the **Passes** tab, and the satellite catalog opens from the button at the top of Passes or from **Settings → Data → Satellite catalog**.

### What do WILL IMAGE, CAN IMAGE and PASS mean?

<span class="tag will">WILL IMAGE</span> The satellite belongs to a mission that images systematically (Sentinel-2, Landsat 8 and 9, Sentinel-1, Sentinel-3, MODIS on Terra and Aqua, VIIRS on Suomi NPP and NOAA-20/21), your point is inside its swath and, for a camera, the sun is high enough. An image is expected.

<span class="tag can">CAN IMAGE</span> A commercial satellite (Maxar, Airbus, Planet, ICEYE, Capella and others) could point at your location on this pass. These satellites image only when a customer orders it. The app never claims that they will, and it cannot tell whether they did.

<span class="tag pass">PASS</span> The satellite flies by, but your point is outside its swath or pointing range, or a camera passes at night. These are hidden by default; **Settings → Passes → Show passes without imaging** lists them.

### The app said WILL IMAGE, but there is no image.

Four usual reasons:

1. **It is too early.** Sentinel-2 images are usually published 3 to 12 hours after the pass, sometimes later. The app keeps looking for 48 hours.
2. **The mission is not Sentinel-2.** In-app satellite images exist for Sentinel-2 only. For Landsat, MODIS, VIIRS and Sentinel-1 or -3, the pass page links to the mission's public browser, preset to your point and day.
3. **The satellite did not acquire.** Outages, manoeuvres and regional exceptions happen, and the app cannot see them.
4. **Your point is in open ocean.** Sentinel-2 covers land and coastal waters. The app checks the archive and labels such passes "Outside Sentinel-2 coverage".

### The image is white or grey.

That is cloud. The satellite photographs whatever is there. Each image shows its cloud percentage, measured over the whole scene (about 110 km across), not over your small window, so a "20 % cloud" image can still be cloudy exactly over your point, and the reverse. Home always shows the newest **clear** image, so a cloudy one may be newer than what you see there.

Clouds are not predicted. A <span class="tag will">WILL IMAGE</span> pass on an overcast day produces an image of clouds.

### Why can't I see my house in the satellite image?

Sentinel-2 records 10 metres of ground per pixel. That shows roads, rivers, fields, city blocks, stadiums and large buildings, and how they change from one pass to the next. A house, a car or a tree is smaller than a pixel. What you get instead of sharpness is **freshness**: the satellite layer in map apps is typically one to three years old, while Sentinel-2 returns every few days.

For points in the United States, the **aerial photo** (below) does show houses, cars and trees.

### What are the aerial photos, and why only in the US?

For points in the United States (the 48 contiguous states, Hawaii and Puerto Rico; not Alaska), the app adds aerial photos from the US Department of Agriculture's National Agriculture Imagery Program (NAIP): 0.6 m per pixel, and 0.3 m in states with newer flights. Each state is flown every two to three years, and the app shows every year back to 2010.

These photos are sharp but not fresh: the newest one may be two or three years old. That is why the app shows them next to the newest Sentinel-2 image, so you can see both what is there and what changed. NAIP is public-domain US government data; there is no equivalent free source for other countries, so outside the US the aerial card does not appear.

### How do I compare two dates?

Tap **Compare** on Home, on an image, on an aerial photo, or in the full-screen viewer. Drag the divider across the picture; tap a date at the top to change it. Both sides are drawn at the same scale around the same point, so streets and shorelines line up. On US points you can also compare an aerial photo with this week's satellite image, or two aerial years.

### What is Timelapse?

All the images of your point played as a short sequence with their dates. Cloudy images are left out unless you turn on **Include cloudy**. You can export it as a video or a GIF to share.

### What does the vegetation view show?

It colours the image by a vegetation index (NDVI) computed from Sentinel-2's red and near-infrared bands: brown is bare ground, yellow is sparse, green is growing vegetation; water and cloud are marked separately. The chip shows the average for the 5 km window, and the trend chart shows how that average moved over the last 30 days. In **Compare → Change**, green areas got greener between the two dates and red areas got browner.

It is a general indicator at 10 m per pixel. It does not identify crops or species, does not diagnose plant health, and is affected by cloud, haze and season.

### What is in a PDF report?

One page with the image or the two compared images, their dates and sources, the scale, and for the vegetation view its legend, averages and change. It carries the line "Not a survey, inspection or valuation". Share it from Compare, from an image, or from the vegetation trend.

### How do I zoom and move around an image?

Pinch, or use the **+** and **−** buttons at the bottom right. Double-tap zooms in where you tap; a two-finger tap zooms out. The target button centres the picture on your point; touch and hold it to return to the whole view. Touch and hold the picture to hide the overlays. In full screen, swipe left or right to move between dates and years at the same place and zoom.

### Is this a live view?

No. No satellite provides live video of the Earth to the public, and no app can show one. Seen from Space shows real photographs, each with its date, normally a few hours to a few days old for satellite images and up to a few years old for aerial photos.

### Why are there no images from WorldView, Pleiades, SkySat or the radar satellites?

Their images are sold by their operators and are not public. The app shows when those satellites could image your point, and never shows or claims an image from them. In-app satellite images come from Sentinel-2, whose data the European Union's Copernicus programme publishes free of charge.

### How accurate are the pass times?

With orbital data younger than two days, usually within about a minute. The data ages: the app shows how old it is and refreshes it on its own about once a day when it has a connection. You can also refresh by hand in **Settings → Data → Orbital data**.

### Settings shows fewer than 90 satellites, or "No orbital data" on a satellite.

The last refresh did not bring data for every satellite. The app keeps what it had and tries again later, so this normally clears by itself. Open **Settings → Data → Orbital data** and tap **Refresh** if you want to retry now (a retry is allowed every two hours). Predictions for the satellites that do have data are not affected.

### I am not getting notifications.

There are two kinds:

- **New image alerts** (free): a notification when a new Sentinel-2 image of a saved point is published. Turn them on in **Settings → Notifications → New image alerts**, or from the card on Home.
- **Pass alerts** (Pro): a reminder a set time before a satellite passes over your point, from the bell on a pass. The lead time is 5 to 60 minutes, 10 by default (**Settings → Notifications → Pass alert lead time**).

If neither arrives, check that notifications are allowed for Seen from Space on your iPhone (**Settings → Notifications** in the app shows a **Permission** row with **Open Settings** if they are not), and that no Focus mode is silencing them.

Notifications are scheduled or posted on the device itself, not sent from a server. New image alerts depend on iOS letting the app check in the background, which it does at its own discretion; opening the app from time to time helps.

### Does the app work without a signal?

Predictions do. The orbital data is stored on the device, so pass times, angles and the pass list work offline for days. Images you have already opened stay in the cache. New images, aerial photos, the vegetation view, the map background and place search need a connection.

### How much mobile data does it use?

Little. The app never downloads whole scenes; it asks for the small window around your point. A 5 km satellite image is about 100 to 150 KB, an aerial photo about 250 to 500 KB, a vegetation view a few hundred KB. On cellular it uses lighter versions first and fetches sharper detail when you zoom in. Images are kept in a cache of up to 200 MB that you can clear in **Settings → Data → Image cache**.

### Why does the app ask for my location?

Only if you tap **Use my location** while adding a point, and only to read one position for that point. The app does not follow you and works fully without the permission: you can add any point by searching for a place, tapping the map or typing coordinates. See the [Privacy Policy]({{ site.baseurl }}/privacy).

### Why does the app ask for access to Photos?

Only when you tap **Save** on an image or save a timelapse. The permission is "add only": the app can save that file and can never read your library.

### What is free, and what does Pro include?

**Free:**

- one saved point
- every pass of Sentinel-2 (A, B and C) and Landsat 8 and 9 for the next 14 days, and the last 7 days
- the three most recent images of your point, with zoom, full screen, timelapse and sharing
- new image alerts
- one free comparison of two dates
- for US points, the newest aerial photo
- the vegetation view of the newest clear image
- PDF reports of the images you can open

**Pro:**

- all 90 satellites, including commercial, radar and weather missions
- unlimited points
- pass alerts before a satellite passes over your point
- 30 days of history and every image of your point in that period
- compare any two dates, as often as you like
- every aerial year since 2010, and comparing aerial years
- the vegetation view for every image, its 30-day trend and the change map
- a larger image area (15 km instead of 5 km)
- timelapse and reports without the large wordmark
- export of passes to CSV

Pro is offered as a monthly subscription, an annual subscription, or a one-time lifetime purchase. Prices are shown in the app in your own currency before you buy.

### How do I cancel a subscription?

On your iPhone: **Settings → your name → Subscriptions → Seen from Space → Cancel Subscription**. Cancel at least 24 hours before the renewal date and you keep Pro until the end of the period you paid for. Deleting the app does not cancel a subscription. The lifetime purchase has nothing to cancel.

### How do I restore my purchase?

If you reinstall the app or move to a new iPhone, tap **Restore Purchases**. It is in **Settings → Pro** inside the app and on the Pro screen itself. You must be signed in with the same Apple Account that made the purchase.

### Can I get a refund?

Purchases are made from Apple, and refunds are decided by Apple. Request one at [reportaproblem.apple.com](https://reportaproblem.apple.com). I cannot issue refunds myself.

### Is there an iPad or Android version?

Not yet. The app is for iPhone and needs iOS 18 or later.

### A prediction or an image looks wrong.

Please tell me. Every confirmed error is added to the app's tests, so your report fixes it for everyone.

Send to **developer.barseghyan@gmail.com**:

1. the satellite and the date and time of the pass, or the image's date, ideally with a screenshot
2. roughly where the point is (the nearest town is enough; you do not need to send exact coordinates)
3. what you expected and what you saw instead

### Where does the data come from?

- **Orbital elements:** CelesTrak, through the public mirror tle.ivanstanojevic.me.
- **Satellite images and the vegetation view:** Copernicus Sentinel-2 Level-2A data, rendered by Microsoft Planetary Computer, with the AWS Open Data copy as a fallback.
- **Aerial photos (US):** USDA NAIP, through Microsoft Planetary Computer, with USGS The National Map as a fallback.
- **Sensor parameters:** each operator's published documentation, listed per satellite inside the app.

The full list is in **Settings → Data sources**.

Seen from Space is an independent app. It is not affiliated with or endorsed by ESA, the European Union, NASA, USGS, USDA, NOAA, Microsoft or any satellite operator.

---

[Privacy Policy]({{ site.baseurl }}/privacy) · [Terms of Use]({{ site.baseurl }}/terms)
