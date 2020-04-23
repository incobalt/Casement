# Casement
A popup-oriented engine for making adventure games in Twine.

This is a work-in-progress engine designed to create adventure games in Twine. It is built on top of the Sugar Cube story format (v. 2.30.0). Casement currently implements stackable popup windows, a standard inventory, a dedicated inventory window, text reactive to popups being viewed, and a simple conversation window and system. Possible future systems could include a character system and an action section/popup.

The current version is a proof-of-concept. To see this version in action, check out [Sunset Directive](https://incobalt.itch.io/sunset-directive).

## Changelog
### v0.002a 04/22/2020
* Added top-level object namespace for Casement
* Casement has objects for each major system planned
* Existing Inventory functions converted to object structure
* Added Casement.Inventory.Item type to better handle inventory items
* Fixed an issue where inventory popups would close early when removing items

### v0.001a 04/22/2020
* Merged all changes made during development of Sunset Directive
* Added inventory item highlights and flashes
* Changed CSS Styling of popups to better react to screen space //More work needs to be done
* Fixed an issue where the inventory popup displayed the passage name
