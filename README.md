# Lyrify
Lyrify is a lyrics app built specifically for a Car Android Head Unit in mind. The App uses the 
Spotify API to get the currently playing track from your Spotify account and a 3rd party API
for the lyrics display. It also has easy-to-use playback and volume controls so that you won't have to 
remove your eyes from the road.

## Screenshots

  <img alt="Default Screen" src="https://raw.githubusercontent.com/janjanmedinaaa/lyrify/master/screenshots/default.png">

  <img alt="Playing Screen" src="https://raw.githubusercontent.com/janjanmedinaaa/lyrify/master/screenshots/playing.png">

## Usage
go to https://developer.spotify.com/dashboard and create a new app, the redirect uri is `com.medina.juanantonio.lyrify://callback`, select `Android` for the APIs used

copy client id and client secret into a keys.properties file:

```
spotifyClientId=<client id>
spotifyClientSecret=<client secret>
```

next create a keystore.properties with the following:

```
storeFile=release.keystore
storePassword=release
keyAlias=release
keyPassword=release
```

then you can build the debug version, for a signed release build you will need to generate a keystore and update the keystore.properties file with the appropriate values.

once you open the app, click the `Spotify` logo to open the web browser and login with spotify