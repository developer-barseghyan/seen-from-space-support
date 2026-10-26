---
layout: default
title: Seen from Space Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Seen from Space: Satellite Map**

Effective date: 26 October 2026 (version 1.1)<br>
Developer: Tigran Barseghyan<br>
Contact: **developer.barseghyan@gmail.com**

---

## In short

> The places you save stay on your iPhone. There is no account and no server of mine.
>
> The app sends anonymous usage statistics to Google Firebase Analytics. They never contain your points, their names or their coordinates.
>
> To show images of a point, the app asks public image services (Microsoft Planetary Computer, and for US aerial photos also USGS) for that area. Those requests necessarily contain an approximate location.
>
> Nothing is sold, and nothing is used for advertising or for tracking you across other apps.

The rest of this page explains each of these in full.

---

## Your saved points

You add a point by searching for a place, tapping the map, typing coordinates, or, only if you tap **Use my location**, from your iPhone's current position.

A point's name, coordinates and notification settings are stored **only on your device**, in the app's own storage. The developer never receives them and cannot see them. Deleting the app deletes them. There is no sync between devices.

## Location

The app asks for location access ("While Using the App") only when you tap **Use my location**, and reads a single position to create the point. It does not track you, does not read your location in the background, and works fully without the permission.

## Predictions

Pass times, angles and the classification of each pass are computed on your device. Nothing about them is sent anywhere.

## Orbital data

To predict passes, the app downloads public orbital elements from **tle.ivanstanojevic.me**, a public mirror of CelesTrak's data, and from **CelesTrak** (celestrak.org) itself as a fallback. The requests ask for satellites by family or catalog number and are the same for every user. They contain no location, no identifier and nothing about your points. As with any internet request, those services see your IP address.

The app refreshes this data when opened if it is more than six hours old, and in the background about once a day.

## Satellite images of your points

After a Sentinel-2 pass over a point, the app looks for the image itself, directly from public sources and not through any server of mine.

- It searches **Earth Search** (earth-search.aws.element84.com), a public catalog run by Element 84 on Amazon Web Services. **The request contains a box of about 2 × 2 km around the point and a range of dates.**
- It then asks **Microsoft Planetary Computer** (planetarycomputer.microsoft.com) for the same Sentinel-2 scene and for the image window around the point: **a box of 5 km or 15 km around the point**, or a smaller box around the area you zoom into. This happens for points anywhere in the world.
- If Planetary Computer cannot answer and you are on Wi-Fi, the app reads the same window from the public **AWS Open Data** bucket for Sentinel-2 (Amazon S3). These requests name the Sentinel-2 tile (about 110 km across) and the portion of the file that is needed.

None of these requests contains a point name, an identifier or an account.

## Vegetation view

When you open the vegetation view of an image (also in its trend, in Compare or in a timelapse), the app asks **Microsoft Planetary Computer** for two small images of the same 5 km box around the point: the vegetation index and the scene classification (which marks cloud and water). On Wi-Fi, if Planetary Computer cannot answer, it reads the same bands from the AWS Sentinel-2 bucket. The vegetation index is computed for display only and stays on your device.

## Aerial photos (United States only)

For a point in the United States, the app shows aerial photos from the US Department of Agriculture's NAIP programme.

- It searches **Microsoft Planetary Computer** for the photos available there, with **a box of about 15 × 15 km around the point**, and asks it for photo crops around the point (5 km or 15 km across, or a smaller box around the area you zoom into).
- If Planetary Computer has no photo or does not answer, it asks **USGS The National Map** (imagery.nationalmap.gov) for the same crops and for the year of the photo under the point.

To decide whether a point is in the United States, the app uses the country Apple's geocoder returns for the point (see below), at most once a month per point. For points outside the United States these requests are never made.

## What image services can see

Stated plainly: Element 84, Microsoft, Amazon Web Services and, for US points, the USGS can see an approximate location you are interested in, together with your IP address, as a map or weather service would. They are not told who you are, and the point may be anywhere on Earth, not where you are. Each runs these services under its own privacy terms.

The app repeats the Sentinel-2 search for up to 48 hours after a pass, also in the background, and may download the newest image of your selected point in advance so that it opens instantly. Downloaded images are cached on your device and can be cleared in **Settings → Data → Image cache**.

## Map, place search and country lookup

The map background, the place search and the lookup of the country a point lies in are provided by **Apple** (Apple Maps services). Apple receives the map area being viewed, the text you search for, or the coordinates being looked up. Apple's handling of this is described in [Apple's Privacy Policy](https://www.apple.com/legal/privacy/).

## Links to public image browsers

Some passes offer a link to a public imagery site: Copernicus Browser (ESA / European Union), NASA Worldview or USGS EarthExplorer. The link opens in your browser and **contains the coordinates of the point and the date of the pass**, because that is what centres the map there. Opening it is your choice; once opened, that site's own privacy policy applies.

## Usage analytics

The app uses **Google Firebase Analytics** to measure how its features are used, so that I know what to improve. It is product measurement only: no advertising, no profiling, no tracking across other apps or websites.

**What is recorded**

- which screens are opened and which filters are used
- that a point was added, how (location, map or typing), how many points exist, and **the two-letter code of the country the point lies in**, nothing finer
- that a pass was opened, with the satellite's group, sensor type and pass class
- how long the timeline took to compute and how many passes it found
- whether orbital data refreshed successfully, and how long it took
- whether pass alerts and new image alerts are on, and that a notification was opened
- which public imagery site was opened (the mission name only)
- which image features are used: opening an image, the full-screen viewer, zoom buttons, Compare (including the free comparison), Timelapse and its export format, the vegetation view, its trend and change map, aerial photos and the year chosen, and sharing a PDF report
- how a satellite image or aerial photo was loaded (which service answered, the resolution, the size and the time it took), never which area
- which Pro feature was tapped, whether the purchase screen was shown, which plan was selected (with its price and currency) and how the purchase or restore ended
- which settings you change, and your current ones: units, whether you have Pro, whether pass alerts and new image alerts are on, and a rough count of your points (1, 2 to 3, 4 or more)

Firebase also records standard technical information on its own: device model, iOS version, app version, language, and an approximate region derived from your IP address on Google's servers. The IP address itself is not stored in the reports.

**What is never sent**

- the names or coordinates of your points, or any location finer than a country
- your device's location
- the text you type or search for
- your name, email address, Apple Account or payment details
- the advertising identifier (IDFA). The app does not include the advertising part of Firebase and does not ask for tracking permission, because it does not track.

**Identifiers.** Firebase gives each installation a random app-instance identifier and can read the vendor identifier that iOS provides to an app (IDFV). Neither tells me who you are. Deleting the app resets the app-instance identifier; iOS resets the vendor identifier when no app from this developer remains on the device.

**No switch in the app.** Analytics are part of how the app is developed and cannot be turned off inside it. If you do not want them, please do not use the app.

**Retention and location of data.** Google stores this data on its servers, which may be outside your country, and keeps event-level data for a limited period (no longer than 14 months); after that only aggregated statistics remain. Google's processing is governed by [Google's Privacy Policy](https://policies.google.com/privacy) and [Firebase's privacy and security terms](https://firebase.google.com/support/privacy).

## Purchases

Pro subscriptions and the lifetime purchase are processed **entirely by Apple** through your Apple Account. The developer never receives your name, payment details or billing address. The app receives only a confirmation from Apple that a purchase is active on the device.

## Notifications

All notifications are **local**: they are scheduled or posted by the app on your device, not sent through any server.

- **Pass alerts** contain the satellite, the kind of pass, the time and the name you gave the point.
- **New image alerts** are posted when the app, checking in the background, finds a new Sentinel-2 image of a saved point. They contain the point's name, the satellite and the cloud cover.

Neither ever contains coordinates.

## Photos

**Save** (on an image) and saving a timelapse ask for permission to add a file to your library. The permission is "add only": the app cannot read your photos.

## Sharing and export

**Share**, timelapse export (video or GIF), PDF reports and **Export CSV** create a file from your own data and open the standard iOS share sheet. A PDF report includes the point's name and coordinates, because that is what makes it useful to the person you send it to. The content goes only where you send it. The developer never sees it.

## What the app does not do

- No user accounts or registration.
- No servers of the developer; no sync.
- No advertising, no advertising identifier, no data brokers.
- No sale or rental of any data.
- No access to your contacts, photos, microphone, camera or health data.

## Children

The app is not directed at children under 13 and does not knowingly collect personal data from them.

## Your rights

The developer holds no data that identifies you: there is no account, and analytics are tied only to the random identifiers described above. For that reason there is no record that can be looked up, corrected or exported for a particular person.

What you control directly:

- delete the app to remove all local data and reset the app-instance identifier
- revoke location or Photos access in **Settings → Privacy & Security** on your iPhone
- manage or cancel a subscription in **Settings → your name → Subscriptions**

If you live in the European Economic Area, the United Kingdom or another place with similar law, analytics are processed on the basis of legitimate interest in understanding and improving the app. You may object or ask any question by writing to the address below, and you may complain to your local data protection authority.

## Changes

If the app's data practices change, this policy and its effective date are updated before the change takes effect, and the change is noted in the app's release notes.

## Contact

**developer.barseghyan@gmail.com**

---

[Support]({{ site.baseurl }}/) · [Terms of Use]({{ site.baseurl }}/terms)
