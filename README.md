# HOI4 Mod Utilities

This extension add tools for Heart of Iron IV modding. Some of the tools may work on other Paradox games.

**Please set extension setting `hoi4ModUtilities.installPath` to correct HOI4 install path (and reload VSCode if possible) before using any preview features below. Or they won't be properly rendered.**

## Features

* World map preview
* Focus tree preview
* Technology tree preview
* `.gfx` file preview (sprites used by HOI4 are defined here)
* `.dds` file preview (images files used by HOI4)

## Steps to start

1. Install and enable this extension in VSCode.
2. Update setting `hoi4ModUtilities.installPath` to the folder that installed Heart of Iron IV.
3. Open your mod develop folder.
4. (*Optional*) Open command palette using `Ctrl+P`. Use command `Select mod file` to set working mod descriptor (the `.mod` file).
5. Use these entries:
    * Command palttle (`Ctrl+P`) commands: `Preview World Map` and `Preview HOI4 file`*.
    * `Preview HOI4 file` (![Preview HOI4 file button](demo/preview-icon.png))* button on right-top tool bar of text editor.
    * Open a `.dds` file.

\* *`Preview HOI4 file` (![Preview HOI4 file button](demo/preview-icon.png)) button/command is invisible, except on `.gfx`, technology tree or national focus tree files.*

## Demos

### World map preview

![World map preview demo](demo/5.gif)

### Focus tree preview

![Focus tree preview demo](demo/1.gif)

### Technology tree preview

![Technology tree preview demo](demo/4.gif)

### GFX file preview

![GFX file preview demo](demo/2.gif)

## Extension Settings

|Setting|Type|Description|
|-------|----------|--------|
|`hoi4ModUtilities.installPath`|`string`|Hearts of Iron IV install path. Without this all icons will be invisible.|
|`hoi4ModUtilities.loadDlcContents`|`boolean`|Whether to load DLC images when previewing files. Enabling this will use more memory (All DLCs are around 600MB).|
|`hoi4ModUtilities.modFile`|`string`|Path to the working .mod file. This file is used to read replace_path. If not specified, will use first .mod file in first folder of the workspace.|

## Known Issues

* GUI of focus tree can't be configured like technology tree.
* Edge lines on world map not alway fit edge of colors.

## Release Notes

### 0.3.1

### Added
* World map preview
  * New view modes: strategic region and supply area.
  * New color sets: supply value.

### Changed
* Refine map loading and auto reload.
* Changed scale level to show edges and labels for different view modes.

### Fixed
* Fixed bug that can't copy file if parent folder not exist.
* Fixed bug that sometimes world map not properly reloaded.
