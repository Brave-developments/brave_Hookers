# brave_Hookers

Prostitute / pimp system for QBCore (converted from [sawu_hookers](https://github.com/stianhje/sawu_hookers)).
Talk to the pimp, pick a girl via the NUI menu, she marks on your GPS, and when
you pick her up in a car you can order services for cash (stress relief included).

## How it plays

1. Talk to the **pimp** (strip club) → NUI menu with 4 hookers
2. Pick one — she spawns at one of 12 locations with a GPS blip
3. Pick her up in a car, signal her with **E** (whistle)
4. Stop in the car and press **E** for the services menu:
   - Blowjob ($1,000) / Sex ($3,000, configured in `config.lua`)
   - Press **H** to make her leave
5. Money is checked & charged server-side; stress is relieved on success
6. Optional [ps-dispatch](https://github.com/Project-Sloth/ps-dispatch) hook —
   10% chance the service is flagged as suspicious activity

## Requirements

- [qb-core](https://github.com/qbcore-framework/qb-core)
- [qb-target](https://github.com/qbcore-framework/qb-target)
- [ox_lib](https://github.com/overextended/ox_lib)
- [InteractSound](https://github.com/M presume/InteractSound) — with a `mysound.ogg`
- Optional: [ps-dispatch](https://github.com/Project-Sloth/ps-dispatch)

## Installation

1. Copy the resource into your `resources` folder.
2. Add to `server.cfg` (ox_lib **before** this resource):

```cfg
ensure ox_lib
ensure brave_Hookers
```

3. Move your `mysound.ogg` into InteractSound's
   `standalone/interact-sound/client/html/sounds` folder.

## Configuration

`config.lua`: core/target/notify (`qb` or `ox`), dispatch hook, prices, the pimp
spawn and all 12 hooker spawn locations. Debug prints toggle with `Config.Debug`.

## Credits

Original by [sawu_hookers](https://github.com/stianhje/sawu_hookers) (MARFY),
QBCore conversion by Brave. Preview: <https://youtu.be/B6wSxh2hGC0>

## License

All rights reserved.
