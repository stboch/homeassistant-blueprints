# homeassistant-blueprints
My collection of home-assistant.io blueprints

## Mobile Companion App Notification Script Blueprints
[Android Alarm from static Time ![Android Alarm from static Time](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstboch%2Fhomeassistant-blueprints%2Fblob%2Fmain%2Fmobile_app_android_alarm.yaml)

[Android Bluetooth ![Android Bluetooth](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstboch%2Fhomeassistant-blueprints%2Fblob%2Fmain%2Fmobile_app_android_bluetooth.yaml)

[Android Do Not Disturb ![Android Do Not Disturb](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstboch%2Fhomeassistant-blueprints%2Fblob%2Fmain%2Fmobile_app_android_dnd.yaml)

[Android High Accuracy ![Android High Accuracy](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstboch%2Fhomeassistant-blueprints%2Fblob%2Fmain%2Fmobile_app_android_ham.yaml)

[Android Set Ringer ![Android Set Ringer](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstboch%2Fhomeassistant-blueprints%2Fblob%2Fmain%2Fmobile_app_android_ringer.yaml)

[Android/iOS Location Update ![Android/iOS Location Update](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstboch%2Fhomeassistant-blueprints%2Fblob%2Fmain%2Fmobile_app_location_update.yaml)

## Common Notification Standard Scripts ## 
All my notification scripts use a standard call format below, message is required for everything, while title, critical, and data are optional.  
Critical allows a device to bypass the devices input boolean used to as a do not disturb. Title and data is currently used by only mobile apps.  
Data for mobile apps are for including additional [mobile app notification features](https://companion.home-assistant.io/docs/notifications/notifications-basic)  
You need to create an input_boolean prior to adding these blueprints that is used for the blueprints control of the do not disturb features.  
```
data:
  title: Testing
  message: test this!
  critical: true
  data:
    actions:
      - action: ALARM
        title: Sound Alarm
        icon: sfsymbols:bell
      - action: SILENCE
        title: Silence Alarm
        icon: sfsymbols:bell.slash
```
[Android/iOS Notification Script ![Android/iOS Notification Script](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstboch%2Fhomeassistant-blueprints%2Fblob%2Fmain%2Fmobile_app_notification.yaml)
