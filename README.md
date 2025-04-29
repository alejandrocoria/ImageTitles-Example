# ImageTitles Example
Example resource pack for the [ImageTitles](https://github.com/alejandrocoria/ImageTitles) mod.

You can use this repository and the zip in [releases](https://github.com/alejandrocoria/ImageTitles-Example/releases) as a reference to create your own resource pack.

You might also find [Tutorial: Creating a Resource Pack](https://minecraft.wiki/w/Tutorial:Creating_a_resource_pack) helpful.

# Directory Structure
Files and subfolders should go inside `assets/namespace/textures/title/` where *namespace* is a unique name for your resource pack so it doesn't collide with other resource packs that are loaded.

# File Formats
Images must be in PNG format with the `.png` extension. They support transparency.

Next to each image there must be a metadata file in JSON format with the same name and `.mcdata` suffix. For example, if you have an image named `my_image.png`, the metadata file would be called `my_image.png.mcdata`.

Example of a metadata file:
```JSON
{
	"title": "my image",
	"x": 0.3,
	"y": 0.75,
	"width": 600,
	"height": 200
}
```

* **title**: the image will be displayed when a title is created with this exact text (e.g. with the command `/title @s title {"text":"my image"}`)
* **x**: (optional) horizontal position of the image. Ranges from 0 to 1, with 0 being the left edge of the window and 1 being the right edge. If omitted, the default value is 0.5, which is the center of the window.
* **y**: (optional) vertical position of the image. Ranges from 0 to 1, with 0 being the top edge of the window and 1 being the bottom edge. If omitted, the default is 0.25, which is between the top edge and the center of the window.
* **width**: the actual width of the image.
* **height**: the actual height of the image.

The width and height may be removed in the future because they are redundant, but for now they are necessary for technical reasons.

---
# Credits
Example image created with [Font Generator](https://www.textstudio.com/).
