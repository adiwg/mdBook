# mdTranslator

## Architecture

### Internal Object
---
#### sensorInfo:

The *sensorInfo* object contains information about the sensor that collected the grid cell values.

````ruby
    def newSensorInfo
        intObj = {
            toneGradations: nil,
            sensorMin: nil,
            sensorMax: nil,
            sensorUnits: nil,
            sensorPeakResponse: nil
        }
    end
````

__toneGradations:__ *integer* - the number of discrete numerical values in the grid data.

__sensorMin:__ *real* - shortest wavelength that the sensor is capable of collecting within a designated band. 

__sensorMax:__ *real* - longest wavelength that the sensor is capable of collecting within a designated band.

__sensorUnits:__ *string* - units in which sensor wavelengths are expressed. 

__sensorPeakResponse:__ *real* - wavelength at which the sensor response is highest.
