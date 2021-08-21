## <a name="markdown-pane"></a>ReadMe
**Weather Pets** lets children and their families experience the weather, air quality, and other important environmental factors in an easy-to-understand animated presentation

  - Real time weather conditions
  - Real time air quality index
  - Moon phase
 
# Design

There are two View Controllers 

  - #### Home Screen
  ![](https://github.com/rafaellevy/weatherPets-ReadMe/blob/master/IMG_3821b.png)

  
    - Displays nine layers of animation based on the data retrieved from the APIs
    - Animation views based on [GPUImage](https://github.com/BradLarson/GPUImage) & [VideoTransparentBackground](https://github.com/agordeev/VideoTransparentBackground)
    - Weather updates every five minutes and moon updates once a day based on location
	
   
- #### Detail Screen
![](https://github.com/rafaellevy/weatherPets-ReadMe/blob/master/IMG_3822b.png)


	- Displays API data as numeric values or helpful tips. The following values are displayed: 

    Parameters  | Info 
    ------------- |-------------
    AQI  | Air Quality Index
    Temperature  | Celsius and Farenheit
    Humidity |  Relative ( % ) 
    Wind | Mph and Km/h
    UV | Ultraviolet index
    Moon | Moon Phase
    
    
    
    - Wind direction is displayed graphically as a compass arrow
    - Air quality is shown using [MKMagneticProgress](https://github.com/malkouz/MKMagneticProgress)




### Model
- Handles the raw values from the different APIs and categorizes each aspect of the weather for displaying the appropriate tips and animations.
- Handles location collection and management
- Interacts with the networking layer
- Interacts with CoreData      

# Persistence
Beauty in the air uses [CoreData](https://developer.apple.com/documentation/coredata) to save preferences:  

- Temperature and speed units
- Selected character
- Useful tips displayed 

# API

Beauty in the sky uses a number of projects to work properly:

* [OpenWeather](https://openweathermap.org/) - Weather and Ultraviolet
* [AirNow](https://docs.airnowapi.org/) - Air Quality
* [SunMoonCalc](https://rapidapi.com/kirs26/api/sunmooncalc/details) - Moon Phase 


# Requirements

- [Xcode](https://developer.apple.com/xcode/) v9+ to run.

- Swift 4.2

License
----

MIT


**Free softaware**

