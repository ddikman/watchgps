# watchgps

Tiny test project to check GPS on a watch with Flutter

My Falster 2 watch didn't seem to want to give me GPS positioning in apps like Adidas or Strava when I went running without carrying my phone. This project is to check if I would be able to get the GPS working in an app of my own.

## result

The `geolocator: ^8.0.1` project ends up showing nothing but a missing implementation.

![Failing to get gps](screenshot.png)

I believe the reason is that the Wear OS simply doesn't provide a standard implementation of the GPS SDK for Android. Instead you have to jump over hoops to get this working and for Flutter, there doesn't seem to be any existing implementation of this.

See:
https://stackoverflow.com/questions/24848970/is-it-possible-to-get-gps-location-from-android-wear-sdk