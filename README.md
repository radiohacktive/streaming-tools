# streaming-goodies

This project contains scripts and useful settings to create the streaming widgets and overlays for Radiohacktivity on Twitch.

This is just getting started- there will be a few large commits initially followed by tweaks as I maintain it from here.

## extra-life/streamDonations.html

This widget shows the running total of the donations received since the page has been active.

### Configuration and installation

Simply change the value of donorDriveID (near the top of the script) from 'IDNUMBER' to your DonorDrive ID (keeping the single quotes around them). If needed, the interval to check this sum can be adjusted from 30 sec, but keep in mind that with the PublicAPI this retrieval is rate-limited and should not running every second. The HTML portion below the Javascript can be edited to create a customized display of the sum.

When ready, add this to your streaming software as a brosder source pointing to this file. This widget will proceed to track the sum of donations from the point at which it is loaded; if this page is refreshed, it will "reset" back to zero.