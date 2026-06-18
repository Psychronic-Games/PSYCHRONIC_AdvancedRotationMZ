# PSYCHRONIC_AdvancedRotationMZ

**RPG Maker MZ Plugin**

Advanced rotation system for events and pictures with continuous rotation support

## What It Does

PSYCHRONIC_AdvancedRotationMZ enhances RPG Maker MZ's rotation capabilities for events and pictures with precise floating-point control and continuous rotation.

## Plugin File

- `PSYCHRONIC_AdvancedRotationMZ.js`
- Version: `1.3`
- Target: RPG Maker MZ
- Author: Psychronic
- URL: https://psychronic.itch.io

## Plugin Commands

### Rotate Picture

- Command: `RotatePicture`
- Description: Rotates a picture with specified parameters

Arguments:

- `pictureId` (Picture ID) - type: number; default: 1: ID of the picture to rotate (positive only, 1 or higher)
- `angle` (Angle) - type: number; default: 0: Target angle in degrees (positive or negative)
- `speed` (Speed) - type: number; default: 1: Degrees per frame (positive or negative)
- `continuous` (Continuous) - type: boolean; default: false: 0 = one-time rotation, 1 = continuous

### Rotate Event

- Command: `RotateEvent`
- Description: Rotates an event with specified parameters

Arguments:

- `eventId` (Event ID) - type: number; default: 0: Event ID (0 for this event, positive or negative)
- `angle` (Angle) - type: number; default: 0: Target angle in degrees (positive or negative)
- `speed` (Speed) - type: number; default: 1: Degrees per frame (positive or negative)
- `continuous` (Continuous) - type: boolean; default: false: 0 = one-time rotation, 1 = continuous

### Stop Rotation

- Command: `StopRotation`
- Description: Stops rotation of specified object

Arguments:

- `type` (Type) - type: select; default: Picture; options: Picture, Event: Type of object to stop rotating
- `id` (ID) - type: number; default: 1: ID of the object to stop (positive or negative)

## Installation

1. Download `PSYCHRONIC_AdvancedRotationMZ.js`.
2. Place it in your RPG Maker MZ project's `js/plugins/` folder.
3. Enable it from the RPG Maker Plugin Manager.
4. Configure any plugin parameters or commands listed below.

## Full Plugin Help

PSYCHRONIC_AdvancedRotationMZ enhances RPG Maker MZ's rotation capabilities for events
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

## Source

This standalone repository is generated from the latest PSYCHRONIC plugin source in the RPG Reactor Complex template.

## License

MIT. See `LICENSE`.
