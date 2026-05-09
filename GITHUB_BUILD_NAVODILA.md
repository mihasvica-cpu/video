# Kako narediti APK brez Android Studia — prek GitHub

## 1. Ustvari GitHub repository
1. Pojdi na GitHub.
2. Klikni **New repository**.
3. Ime naj bo npr. `VelotubeAPK`.
4. Izberi **Public** ali **Private**.
5. Klikni **Create repository**.

## 2. Naloži datoteke iz tega ZIP-a
1. Odpri repository.
2. Klikni **Add file > Upload files**.
3. Naloži **vso vsebino mape `VelotubeAPK_GitHub`**.
   - Pomembno: datoteke `app`, `.github`, `build.gradle`, `settings.gradle` morajo biti na vrhu repositoryja.
4. Klikni **Commit changes**.

## 3. Zaženi build
1. V repositoryju klikni zavihek **Actions**.
2. Izberi **Build Android APK**.
3. Klikni **Run workflow**.
4. Počakaj, da se build konča.

## 4. Prenesi APK
1. Odpri končan workflow run.
2. Spodaj poišči **Artifacts**.
3. Prenesi `velotube-debug-apk`.
4. V ZIP-u bo `app-debug.apk`.

## Namestitev na telefon
1. Pošlji `app-debug.apk` na Android telefon.
2. Odpri datoteko.
3. Dovoli **Install unknown apps**, če telefon vpraša.
4. Namesti aplikacijo.

## URL aplikacije
Aplikacija trenutno odpira:
`https://staging.velotube.kolesar.ski/`

Če želiš zamenjati URL, odpri:
`app/src/main/java/ski/kolesar/velotube/MainActivity.java`

Spremeni vrstico:
`START_URL = "https://staging.velotube.kolesar.ski/";`
