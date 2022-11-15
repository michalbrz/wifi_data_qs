**Project failed** 

I've tried to fork the original project to add mobile data tile to it, but it turns out it's not possible. My learnings below.

There are two ways so control mobile data from Android app:
- having special first-party app only permission [MODIFY_PHONE_STATE](https://developer.android.com/reference/android/Manifest.permission.html#MODIFY_PHONE_STATE) - not feasible. Permission was enforced in this way back in the days (Gingerbread I think?), so it's not something that can be hacked away like original project of Wi-Fi only tile which can target Android R.
- rooted phone, because you can do anything with rooted phone
- running adb commands (what [Better-Internet-Tiles](https://github.com/CasperVerswijvelt/Better-Internet-Tiles) is doing) - requires either root or Shizuku app. Not perfect, but unfortunately the only option you have as 3rd party app developer.
