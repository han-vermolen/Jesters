# Title
Proximity vs. Location

# Number
1

## Status
Accepted

## Context
In order for Hey, Blue! to optimally connect _police officers_ with _individuals_ the latter should have a frictionless experience while protecting the safety of the former. As _police officers_ have voiced some concerns about location tracking of their cell phones, we propose a solution that is a bit different. 

## Decision
While still providing the _police officers_ with the ability to turn their location tracking on we use Bluetooth Low Energy(BLE) proximity features as an alternative approach that safeguards the _police officer's_ privacy and security. This option aims to allow for more oppotunities to arise for communities to make a meaningful connection through Hey, Blue!. 

## Consequences
BLE proximity and direction measurements are somewhat less reliable over longer distances. For Hey, Blue! this should not be an issue. However, if in the future proximities in the range of 100 meters or more are to be considered we should BLE options will be far less reliable.

Using proximity instead of the distance between 2 measured locations (the _police officer's_ location and the _individual's_) we will have no need to centrally store location data. All applicable functions in the requirements set can be handled by proximity matching. 

BLE proximity is somewhat less accurate than GPS location coordinates. However, GPS measurements are by themselves guarenteed to be appropriatly accurate. The trade-off in favor of proximity measurements is worth it due to its security and privacy characteristics.

BLE proximity will allow us to perform far better indoor measurements. This could come in quite handily during indoor community meetups, police exhibitions, etc.
