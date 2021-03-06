# lovelace-live-text-update-card
A text card for Home Assistant that will call a service as you type.

**This is mainly a proof of concept and may break since the code is super janky! Please don't judge as this is my first custom card project! Please make a PR if you want to help fix the code!**

Inspired by and uses code from [lovelace-text-input-row](https://github.com/gadgetchnnel/lovelace-text-input-row) by [@gadgetchnnel](https://github.com/gadgetchnnel) and is built for use with [esphome-blekeyboard](https://github.com/dmamontov/esphome-blekeyboard) by [@dmamontov](https://github.com/dmamontov)

## Card Config
| Name | Type |Requirement | Description | Default |
|--|--|--|--|--|
| `type` | string |Required | `custom:live-text-update` |
| `service` | string | Required | Service that is used for espkeyboard. Ex: `esphome.blekeyboard` |
| `placeholder` | string | Optional | Text to show when box is empty. Ex: `Search` | `Search` | 
| `placeholder_enabled` | boolean | Optional | Enables or disables placeholder text. Ex: `true` | `true` |
| `clear_button_enabled` | boolean | Optional | Enables or disables the clear button. Ex: `true` | `true`

## Example Config
```yaml
type: custom:live-text-update
service: esphome.blekeyboard
placeholder_enabled: true
placeholder: Search
clear_button_enabled: true
```



