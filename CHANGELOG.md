# Change Log

All notable changes to the "hoi4modutilities" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [0.2.0] - 2020/04/25 - Latest

### Added
* Technology tree preview
  * Render technology tree as GUI defined in `interface\countrytechtreeview.gui` (icons, texts defined in this file will also be rendered).
  * Navigate to related technology tag by clicking technology or subtechnology.
  * Auto update preview when technology file changed.
  * Switch technology folder if a technology tree contains technology from different folder.
  * Can be dragged to scroll.
* GFX file preview
  * Support `corneredTileSpriteType` tags.

### Changed
* GFX file preview
  * Show image size on tooltip.
* Focus tree preview
  * Can be dragged to scroll.

### Fixed
* Fix 1 pixel offset of read `.dds` file.

## [0.1.1] - 2020/04/19

### Fixed
* Fix bug that the tokenizer will read `={` as one token.

## [0.1.0] - 2020/04/18

### Added
* Focus tree preview
  * Render focus tree as graph.
  * Navigate to `focus` tag in document by clicking a focus in graph.
  * Show/hide focus branches (available for focuses has `allow_branch` tag).
  * Auto update preview when document updates.
  * Preview focus tree file that contains `shared_focus` tree.
* GFX file preview
  * Preview all `spritetype` tags in `.gfx` files.
  * Filter sprites by name.
  * Navigate to `spritetype` tag in document by clicking a sprite in list.
* DDS preview
  * Supports RGB and RGBA format.
