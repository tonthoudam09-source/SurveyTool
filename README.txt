KHONGJOM FIELD SURVEY TOOLS
===========================

No build step. No npm. Three static files.

DEPLOY (about 30 seconds)
-------------------------
1. Go to app.netlify.com and sign in.
2. Drag THIS ENTIRE FOLDER onto the "deploy manually" drop area.
3. Netlify returns an HTTPS address, e.g. https://random-name.netlify.app
4. Rename the site to something you can type from memory:
   Site settings -> Change site name -> khongjom-survey

WHY IT MUST BE HOSTED
---------------------
Browsers refuse GPS access to pages that are not on HTTPS. Opening these
files directly from the phone's storage will NOT work - the location
readout stays blank. Hosting is not optional for these tools.

BEFORE THE FIELD TRIP
---------------------
Open the site on the actual survey phone, on Wi-Fi, and confirm both lines
of the device check are green. Grant location permission there and then.
Write the URL on paper and take it with you.

WHAT EACH TOOL DOES
-------------------
index.html             Launcher plus a device check.
field-recorder.html    Use this one. Zone coordinates typed or pasted from
                       GPS Test, anchor and offset records tied to Scaniverse
                       scans, and a live walk test. Exports JSON and a
                       ready-to-paste waypoints.js block.
geofence-surveyor.html Superseded. Averages browser GPS samples itself.
                       Only needed if you stop using GPS Test.

DATA SAFETY
-----------
Nothing is stored in the browser. Every save triggers a download instead, so
a stray reload or a flat battery cannot cost you a walk back across the site.
Check the phone's Downloads folder before leaving the memorial.
