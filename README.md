# Casement
A popup-oriented engine for making adventure games in Twine.

This is a work-in-progress engine designed to create adventure games in Twine. It is built on top of the Sugar Cube story format (v. 2.30.0). Casement currently implements stackable popup windows, a standard inventory, a dedicated inventory window, text reactive to popups being viewed, and a simple conversation window and system. Possible future systems could include a character system and an action section/popup.

The current version is a proof-of-concept. To see this version in action, check out [Sunset Directive](https://incobalt.itch.io/sunset-directive).

## Changelog

### 04/26/2020
* Moved inventory popups into the Casement.Inventory namespace
* Added work for robustly building inventory links to keep highlighting persisting across passage transitions
* Removed the need for $InvenShowing in Twine variables, now the invWindow keeps track of the window and the item associated with it.
* Known Issue: Since Casement.Popup is not finished, Casement.Inventory.showItem() complains about Casement.Popup.refreshTop() not existing (it doesn't yet).

### 04/22/2020
* Added top-level object namespace for Casement
* Casement has objects for each major system planned
* Existing Inventory functions converted to object structure
* Added Casement.Inventory.Item type to better handle inventory items
* Fixed an issue where inventory popups would close early when removing items

* Merged all changes made during development of Sunset Directive
* Added inventory item highlights and flashes
* Changed CSS Styling of popups to better react to screen space //More work needs to be done
* Fixed an issue where the inventory popup displayed the passage name
