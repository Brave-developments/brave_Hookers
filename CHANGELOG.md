# Changelog

## [fix] - 2026-10-07

### Fixed
- Server-side triggerNotify calls now pass (message, type, src) instead of (src, message, type).
- onResourceStop removes the pimp target entity correctly and deletes the pimp ped instead of calling RemoveZone on an entity key.
