# mdTranslator

## Architecture

### Internal Object
---
#### imageInfo:

The *imageInfo* object contains information about the thematic classification item.

````ruby
    def newImageInfo
        intObj = {
            illuminationElevationAngle: nil,
            illuminationAzimuthAngle: nil,
            imageCondition: nil,
            imageQuality: {},
            cloudCoverPercent: nil,
            compressionQuantity: nil,
            triangulationInfo: false,
            radiometricCalibrationInfo: false,
            cameraCalibrationInfo: false,
            filmDistortionInfo: false,
            lensDistortionInfo: false
        }
    end
````

__illuminationElevationAngle:__ *real* - illumination elevation measured in degrees clockwise from the target plane at intersection of the optical line of sight with the Earth’s surface. For images from a scanning device, refer to the center pixel of the image. 

__illuminationAzimuthAngle:__ *real* - illumination azimuth measured in degrees clockwise from true north at the time the image is taken. For images from a scanning device, refer to the center pixel of the image.

__imageCondition:__ *string* - a code which indicates conditions which may affect the image.  Example: snow, fog, clouds, night, blurred...

__imageQuality:__ *object* - a [resourceId](../mdtranslator/resourceId.md) object which specifies the image quality. 

__cloudCoverPercentage:__ *real* - area of the dataset obscured by clouds, expressed as a percentage of the spatial extent.

__compressionQuantity:__ *integer* - count of the number of lossy compression cycles performed on the image. 

__triangulationInfo:__ *Boolean* - indication of whether or not triangulation has been performed upon the image.

__radiometricCalibrationInfo:__ *Boolean* - indication of whether or not the radiometric calibration information for generating the radiometrically calibrated standard data product is available.

__cameraCalibrationInfo:__ *Boolean* - indication of whether or not constants are available which allow for camera calibration corrections.

__filmDistortionInfo:__ *Boolean* - indication of whether or not Calibration Reseau information is available.

__lensDistortionInfo:__ *Boolean* - indication of whether or not lens aberration correction information is available.
