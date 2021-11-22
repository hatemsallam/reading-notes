# Location

* your app can request the last known location of the user's device Using the Google Play services location APIs.
* use the fused location provider to retrieve the device's last known location.
* The fused location provider is one of the location APIs in Google Play services.
* It manages the underlying location technology and provides a simple API so that you can specify requirements at a high level

## Set up Google Play services

* To access the fused location provider, your app's development project must include Google Play services.
* Download and install the Google Play services component via the SDK Manager and add the library to your project.

## Specify app permissions

* Apps whose features use location services must request location permissions, depending on the use cases of those features.

## Create location services client

* In your activity's onCreate() method, create an instance of the Fused Location Provider Client

```
    private FusedLocationProviderClient fusedLocationClient;

    // ..

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        // ...

        fusedLocationClient = LocationServices.getFusedLocationProviderClient(this);
    }
```

## Get the last known location

* Once you have created the Location Services client you can get the last known location of a user's device.
* you can use the fused location provider's getLastLocation() method to retrieve the device location.
* The getLastLocation() method returns a Task that you can use to get a Location object with the latitude and longitude coordinates of a geographic location.
* The location object may be null in the following situations:
  * Location is turned off in the device settings.
  * The device never recorded its location
  * Google Play services on the device has restarted

## Choose the best location estimate

* The FusedLocationProviderClient provides several methods to retrieve device location information.
* getLastLocation() :gets a location estimate more quickly and minimizes battery usage that can be attributed to your app.
* getCurrentLocation(): gets a fresher, more accurate location more consistently. 