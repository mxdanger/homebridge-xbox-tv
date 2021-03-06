# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.3.2] - 2021-01-18
#### Fixed
* Fix log info regarding Input references ([#63](https://github.com/grzegorz914/homebridge-xbox-tv/issues/63))

## [1.3.1] - 2021-01-06
### Fixed
* Fix `getAppChannelLineups` data error.

## [1.3.0] - 2020-11-20
### Fixed
* Dependency bump ([#55](https://github.com/grzegorz914/homebridge-xbox-tv/issues/55))

## [1.2.41] - 2020-11-20
### Fixed
* Fix slow response on RC control.

## [1.2.1] - 2020-09-18
### Changes
* Updated device category to `TV_SET_TOP_BOX` ([#47](https://github.com/grzegorz914/homebridge-xbox-tv/pull/47))

## [1.2.0] - 2020-09-17
### Changes
* Fix send power on until successful ([#38](https://github.com/grzegorz914/homebridge-xbox-tv/issues/38))
* Fix remote control function ([#28](https://github.com/grzegorz914/homebridge-xbox-tv/issues/28))
* Add `refreshInterval` with a default of five seconds.
* Updated config layout.

## [1.1.0] - 2020-09-06
### Changes
* Completely reconfigured layout of the configuration schema.

## [1.0.0] - 2020-06-28
### Added
* Release version.

## [0.9.0] - 2020-05-23
### Added
* Add possibility to select what a type of extra volume control you want to use. None, Slider, Fan.

## [0.8.21] - 2020-05-23
### Changes
* Output app reference to log when opening app ([#22](https://github.com/grzegorz914/homebridge-xbox-tv/issues/22), [#26](https://github.com/grzegorz914/homebridge-xbox-tv/issues/26))
  * Used for discovering the value to use for `reference` when adding new inputs.

## [0.8.0] - 2020-05-20
### Added
* Add mute ON/OFF to the slider volume.

## [0.7.60] - 2020-05-18
### Fixed
* Fix bug in RC control.

## [0.7.35] - 2020-05-17
### Added 
* Add read console configuration after Homebridge restart and save to `/homebridge_folder/xboxTv/` file.

## [0.7.2] - 2020-05-14
### Added 
* Add descriptions in `config.schema.json`.

## [0.7.0] - 2020-05-14
### Added
* Revert back with defaults inputs.
* Add input type to inputs.
* Add other fixes in code to prevent app crash without configured inputs.

## [0.6.0] - 2020-05-14
### Breaking Changes
* Update yor config.json: Add types to the inputs.

### Default Inputs
```json
"inputs": [
	{
		"name": "TV",
		"reference": "Microsoft.Xbox.LiveTV_8wekyb3d8bbwe!Microsoft.Xbox.LiveTV.Application",
		"type": "HDMI"
	},
	{
		"name": "Dashboard",
		"reference": "Xbox.Dashboard_8wekyb3d8bbwe!Xbox.Dashboard.Application",
		"type": "HOME_SCREEN"
	},
	{
		"name": "Settings",
		"reference": "Microsoft.Xbox.Settings_8wekyb3d8bbwe!Xbox.Settings.Application",
		"type": "OTHER"
	},
	{
		"name": "Accessory",
		"reference": "Microsoft.XboxDevices_8wekyb3d8bbwe!App",
		"type": "OTHER"
	}
]
```

## [0.5.0] - 2020-05-10
### Changes
* Code cleanup.
* Miscellaneous fixes and performance improvements.

## [0.4.0] - 2020-05-06
### Changes
* Adapted to HAP-Node JS lib.

## [0.3.12] - 2020-05-05
### Changes
* Cleanup code.

### Breaking Changes
* Update yor config.json: replace `apps` with `inputs`.

## [0.3.12] - 2020-05-05
### Changes
* Fix and performance improvements.
* Corrected logging state.

## [0.3.9] - 2020-05-05
### Added
* Add real time read and write data for lightbulb slider volume value.

## [0.2.3] - 2020-04-27
### Added
* Add switch ON/OFF volume control.

## [0.2.1] - 2020-04-27
### Added
* Add Siri volume control.
* Add slider or Brightness volume control.

## [0.1.39] - 2020-04-21
* Different fixes.

## [0.1.12] - 2020-04-13
* Fix memory leak.

## [0.1.9] - 2020-04-07
* Fix store of position in HomeKit favorites.

## [0.1.6] - 2020-04-06
* Test 2.

## [0.1.5] - 2020-04-05
* Test 1.

## [0.1.2] - 2020-04-05
* Some improvements.

## [0.1.1] - 2020-04-05
* Update `README.md`.
* Update `sample-config.json`.

## [0.1.0] - 2020-03-29
* Fix crash if no device name defined.
* Fix `config.schema.json`.
* Fix store file inside the Homebridge directory.

## [0.0.118] - 2020-03-29
* Small fixes.

## [0.0.115] - 2020-03-21
* Corrections for Homebridge git.
* Performance improvements.

## [0.0.1] - 2020-02-05
* Initial release.
