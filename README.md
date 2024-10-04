# Location App Positioning System (LAPS)

This simple Android app allows you to broadcast your real-time location. Anyone with your dynamically generated unique key can track your location using the app. The project was developed for learning purposes, focusing on Firebase, Google Maps API, and Google Location API.

# Backend
The backend is built using Firebase Cloud Functions. 

# How it works?

- The first device continuously updates its location using GPS, network, etc.
- The location data is written to and updated in a specific Firebase Firestore document.
- The second device reads the Firestore document and displays a marker on the map representing the tracked location.

# Integrating Google Maps & Location API
- To use Google Maps in Android app, you can integrate it using SupportMapFragment or MapView.
- Using Google Maps fragment (inside a layout or as a root tag):
 
```xml
<fragment
	android:id="@+id/map"
	android:name="com.google.android.gms.maps.SupportMapFragment"
	android:layout_width="match_parent"
	android:layout_height="match_parent"/>
```

- Add location permissions and the Google Maps API key in the AndroidManifest.xml file:
- Ensure to include permissions for coarse and fine location, along with the meta-data tag for the API key.

# References
- [Set Up Google Play Services](https://developers.google.com/android/guides/setup)
- [Getting Started - Google Maps](https://developers.google.com/maps/documentation/android-api/start)
- [Get API Key](https://developers.google.com/maps/documentation/android-api/signup)
- [Add Marker in Maps](https://developers.google.com/maps/documentation/android-api/map-with-marker)
- [Firebase Documentation Guides](https://firebase.google.com/docs/guides/))
- [Get Started with Firebase Firestore](https://firebase.google.com/docs/firestore/quickstart)
- [Firestore Data Model](https://firebase.google.com/docs/firestore/data-model)
- [Firestore - Get Data](https://firebase.google.com/docs/firestore/query-data/get-data)
- [Firestore - Structure Data](https://firebase.google.com/docs/firestore/manage-data/structure-data)

