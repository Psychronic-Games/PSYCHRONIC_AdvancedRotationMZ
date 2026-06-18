# PSYCHRONIC_AdvancedRotationMZ

**RPG Maker MZ Plugin**

Advanced rotation system for events and pictures with continuous rotation support

## What It Does

and pictures with precise floating-point control and continuous rotation.

## Plugin File

- `PSYCHRONIC_AdvancedRotationMZ.js`
- Version: `1.3`
- Target: RPG Maker MZ
- Author: Psychronic
- URL: https://psychronic.itch.io

## Plugin Commands

- `RotatePicture`
- `RotateEvent`
- `StopRotation`

## Installation

1. Download `PSYCHRONIC_AdvancedRotationMZ.js`.
2. Place it in your RPG Maker MZ project's `js/plugins/` folder.
3. Enable it from the RPG Maker Plugin Manager.
4. Configure any plugin parameters or commands listed below.

## Full Plugin Help

and pictures with precise floating-point control and continuous rotation.

Plugin Commands:
RotatePicture <pictureId> <angle> <speed> <continuous>
RotateEvent <eventId> <angle> <speed> <continuous>
StopRotation <type> <id>

Parameters:
<pictureId/eventId>: Numeric ID of the target (positive or negative; 0 for current event)
<angle>: Target angle in degrees (float, positive or negative)
<speed>: Degrees per frame (float, positive or negative)
<continuous>: 0 = one-time rotation, 1 = continuous

Examples:
RotatePicture 1 -90.5 0.25 0
RotateEvent 2 -360 -1.5 1
StopRotation Picture 1

@command RotatePicture
@text Rotate Picture
@desc Rotates a picture with specified parameters
@arg pictureId
@type number
@text Picture ID
@desc ID of the picture to rotate (positive only, 1 or higher)
@default 1
@arg angle
@type number
@decimals 2
@text Angle
@desc Target angle in degrees (positive or negative)
@default 0
@min -3600
@max 3600
@arg speed
@type number
@decimals 2
@text Speed
@desc Degrees per frame (positive or negative)
@default 1
@min -3600
@max 3600
@arg continuous
@type boolean
@text Continuous
@desc 0 = one-time rotation, 1 = continuous
@default false

@command RotateEvent
@text Rotate Event
@desc Rotates an event with specified parameters
@arg eventId
@type number
@text Event ID
@desc Event ID (0 for this event, positive or negative)
@default 0
@arg angle
@type number
@decimals 2
@text Angle
@desc Target angle in degrees (positive or negative)
@default 0
@min -3600
@max 3600
@arg speed
@type number
@decimals 2
@text Speed
@desc Degrees per frame (positive or negative)
@default 1
@min -3600
@max 3600
@arg continuous
@type boolean
@text Continuous
@desc 0 = one-time rotation, 1 = continuous
@default false

@command StopRotation
@text Stop Rotation
@desc Stops rotation of specified object
@arg type
@type select
@option Picture
@option Event
@text Type
@desc Type of object to stop rotating
@default Picture
@arg id
@type number
@text ID
@desc ID of the object to stop (positive or negative)
@default 1

## Source

This standalone repository is generated from the latest PSYCHRONIC plugin source in the RPG Reactor Complex template.

## License

MIT. See `LICENSE`.
