---
layout: default
title: Seen from Space Support
permalink: /
---

# Support

**Seen from Space: Satellite Map** shows fresh, free satellite images of any place on Earth and tells you when the next one will be taken. It predicts the passes of 90 Earth-imaging satellites over the points you save and shows the Sentinel-2 images of those points, usually within hours of the pass.

There is no account and no server of mine. Predictions are computed on your iPhone, and your points are stored only on it.

---

## Contact

**developer.barseghyan@gmail.com**

I usually reply within about two business days. If a prediction or an image looks wrong, please read *"A prediction or an image looks wrong"* below before writing, and include what it asks for. It makes the fix much faster.

---

## Before anything else

**Pass times are predictions, and an expected image is not a promised one.** The app computes where each satellite will be from public orbital data and judges each pass against a model of the satellite's sensor. It does not read the operators' real acquisition plans and it does not know about clouds. Please do not use it for navigation, safety or any decision where an error could cause harm.

---

## Frequently asked questions

### What do WILL IMAGE, CAN IMAGE and PASS mean?

<span class="tag will">WILL IMAGE</span> The satellite belongs to a mission that images systematically (Sentinel-2, Landsat 8 and 9, Sentinel-1, Sentinel-3, MODIS on Terra and Aqua, VIIRS on Suomi NPP and NOAA-20/21), your point is inside its swath and, for a camera, the sun is high enough. An image is expected.

<span class="tag can">CAN IMAGE</span> A commercial satellite (Maxar, Airbus, Planet, ICEYE, Capella and others) could point at your location on this pass. These satellites image only when a customer orders it. The app never claims that they will, and it cannot tell whether they did.

<span class="tag pass">PASS</span> The satellite flies by, but your point is outside its swath or pointing range, or a camera passes at night. These are hidden by default; **Settings → Show passes without imaging** lists them.

### The app said WILL IMAGE, but there is no image.

Four usual reasons:

1. **It is too early.** Sentinel-2 images are usually published 3 to 12 hours after the pass, sometimes later. The app keeps looking for 48 hours.
2. **The mission is not Sentinel-2.** In-app images exist for Sentinel-2 only. For Landsat, MODIS, VIIRS and Sentinel-1 or -3, the pass page links to the mission's public browser, preset to your point and day.
3. **The satellite did not acquire.** Outages, manoeuvres and regional exceptions happen, and the app cannot see them.
4. **Your point is in open ocean.** Sentinel-2 covers land and coastal waters. The app checks the archive and labels such passes "Outside Sentinel-2 coverage".

### The image is white or grey.

That is cloud. The satellite photographs whatever is there. Each image shows its cloud percentage, which is measured over the whole scene (about 110 km across), not over your small window, so a "20 % cloud" image can still be cloudy exactly over your point, and the reverse.

Clouds are not predicted. A <span class="tag will">WILL IMAGE</span> pass on an overcast day produces an image of clouds.

### Why can't I see my house or my car?

Sentinel-2 records 10 metres of ground per pixel. That shows roads, rivers, fields, city blocks, stadiums and large buildings, and how they change from one pass to the next. A house, a car or a tree is smaller than a pixel. Zooming further only makes the squares bigger, so the app stops zooming where it stops being useful.

What you get instead of sharpness is **freshness**: the satellite layer in map apps is typically one to three years old, while Sentinel-2 returns every few days.

### Is this a live view?

No. No satellite provides live video of the Earth to the public, and no app can show one. Seen from Space shows real photographs, each with its date and time, normally a few hours to a few days old.

### Why are there no images from WorldView, Pleiades, SkySat or the radar satellites?

Their images are sold by their operators and are not public. The app shows when those satellites could image your point, and never shows or claims an image from them. In-app images come from Sentinel-2, whose data the European Union's Copernicus programme publishes free of charge.

### How accurate are the pass times?

With orbital data younger than two days, usually within about a minute. The data ages: the app shows how old it is and refreshes it on its own about once a day when it has a connection. You can also refresh by hand in **Settings → Data → Orbital data**.

### Settings shows fewer than 90 satellites, or "No orbital data" on a satellite.

The last refresh did not bring data for every satellite. The app keeps what it had and tries again later, so this normally clears by itself. Open **Settings → Data → Orbital data** and tap **Refresh** if you want to retry now (a retry is allowed every two hours). Predictions for the satellites that do have data are not affected.

### I am not getting notifications.

Check, in this order:

1. Notifications are a **Pro** feature.
2. **Settings → Notifications → Permission** in the app must show them as allowed. If it does not, tap **Open Settings** and allow them for Seen from Space.
3. The reminder is sent a set time before the pass: 5 to 60 minutes, 10 by default (**Settings → Notifications → Default lead time**).
4. A Focus mode or Do Not Disturb on the iPhone silences them like any other notification.

Reminders are scheduled on the device itself, not sent from a server. iOS keeps at most 64 pending reminders per app, so the app schedules the nearest 60 and adds more as they pass; **Settings → Notifications → Scheduled** shows the count. Opening the app from time to time keeps the schedule full.

### Does the app work without a signal?

Predictions do. The orbital data is stored on the device, so pass times, angles and the timeline work offline for days. Images, the map background and place search need a connection.

### How much mobile data does it use?

Little. The app does not download whole scenes (hundreds of megabytes each); it reads only the small window around your point, a tiny fraction of that. On cellular it first loads a lighter 20 m version and fetches full 10 m detail when you zoom in. Images are kept in a cache of up to 200 MB that you can clear in **Settings → Data → Image cache**.

### Why does the app ask for my location?

Only if you tap **Use my location** while adding a point, and only to read one position for that point. The app does not follow you and works fully without the permission: you can add any point by searching for a place, tapping the map or typing coordinates. See the [Privacy Policy]({{ site.baseurl }}/privacy).

### Why does the app ask for access to Photos?

Only when you tap **Save to Photos** on an image. The permission is "add only": the app can save that picture and can never read your library.

### What is free, and what does Pro include?

**Free:** one saved point; every pass of Sentinel-2 (A, B and C) and Landsat 8 and 9 for the next 14 days; the last 7 days of history; the three most recent images of your point.

**Pro:** all 90 satellites, including commercial, radar and weather missions; unlimited points; notifications before a pass and when your point has been imaged; 30 days of history; every image of your point in that period; a larger image area (15 km instead of 5 km); comparing two dates; export to CSV.

Pro is offered as a monthly subscription, an annual subscription, or a one-time lifetime purchase. Prices are shown in the app in your own currency before you buy.

### How do I cancel a subscription?

On your iPhone: **Settings → your name → Subscriptions → Seen from Space → Cancel Subscription**. Cancel at least 24 hours before the renewal date and you keep Pro until the end of the period you paid for. Deleting the app does not cancel a subscription. The lifetime purchase has nothing to cancel.

### How do I restore my purchase?

If you reinstall the app or move to a new iPhone, tap **Restore**. The button is in **Settings** inside the app and on the Pro screen itself. You must be signed in with the same Apple Account that made the purchase.

### Can I get a refund?

Purchases are made from Apple, and refunds are decided by Apple. Request one at [reportaproblem.apple.com](https://reportaproblem.apple.com). I cannot issue refunds myself.

### Is there an iPad or Android version?

Not yet. The app is for iPhone and needs iOS 18 or later.

### A prediction or an image looks wrong.

Please tell me. Every confirmed error is added to the app's tests, so your report fixes it for everyone.

Send to **developer.barseghyan@gmail.com**:

1. the satellite and the date and time of the pass, ideally a screenshot of the pass page
2. roughly where the point is (the nearest town is enough; you do not need to send exact coordinates)
3. what you expected and what you saw instead

### Where does the data come from?

Orbital elements come from CelesTrak, through the public mirror tle.ivanstanojevic.me. Images are Copernicus Sentinel-2 Level-2A data read from the AWS Open Data programme. Sensor parameters come from each operator's published documentation and are listed per satellite inside the app. The full list is in **Settings → Data sources**.

Seen from Space is an independent app. It is not affiliated with or endorsed by ESA, the European Union, NASA, USGS, NOAA or any satellite operator.

---

[Privacy Policy]({{ site.baseurl }}/privacy) · [Terms of Use]({{ site.baseurl }}/terms)
