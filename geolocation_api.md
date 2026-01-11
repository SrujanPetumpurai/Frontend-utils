# GEOLOCATION API
-Browser-provided Web API that lets a website request the user’s physical location.
-What it provides
1.Latitude
2.Longitude
3.Accuracy (meters)
4.Optional: altitude, speed, heading

## Where it exists & Main methods
- Exists at navigator.geolocation();
- navigator.geolocation.getCurrentPosition()
- navigator.geolocation.watchPosition() - continuous tracking
- navigator.geolocation.clearWatch() - stop tracking
## Current Position
- !'geolocation' in navigator is to check if browser supports Geolocation api
```js
//Syntax
navigator.geolocation.getCurrentPosition(successfunction,errorFunction)

function getUserLocation = (){
    if(!('geolocation' in navigator)){
    console.log("Geo location not supported")
    return
    }
    navigator.geolocation.getCurrentPosition(
        (position)=>{
            const {latitude,longitude} = position.cords;
            console.log("Latitude:", latitude);
            console.log("Longitude:", longitude);
        },
        (error)=>{
            console.log(error.message)
        },
        {
          enableHighAccuracy: true,
          timeout: 10000,
          maximumAge: 0,
        }   
    )
}
```

