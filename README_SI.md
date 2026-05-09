# Velotube Android APK projekt

To je Android WebView aplikacija iz obstoječe spletne strani:

`https://staging.velotube.kolesar.ski/`

## Kaj je vključeno
- odpira obstoječo Velotube stran v aplikaciji,
- JavaScript in localStorage sta omogočena,
- podprt je gumb nazaj,
- podprt je izbor/upload videa iz telefona,
- dodana so dovoljenja za internet, video datoteke in kamero.

## Kako narediš APK v Android Studiu
1. Odpri mapo `VelotubeAPK` v Android Studiu.
2. Počakaj, da se Gradle sinhronizira.
3. Izberi **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. APK najdeš v:
   `app/build/outputs/apk/debug/app-debug.apk`

## Če želiš spremeniti URL strani
Odpri:
`app/src/main/java/ski/kolesar/velotube/MainActivity.java`

Spremeni vrstico:
`START_URL = "https://staging.velotube.kolesar.ski/";`
