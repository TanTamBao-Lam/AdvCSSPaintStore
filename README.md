# Paint Store
In this project, you will follow step-by-step instructions to improve a vibrant, color-rich web page for a home paint business. It displays information about using color in a home and color swatches with varying lightness, saturation, and hue.

The page is almost ready to be published. You’ll be making the following color-related changes:
* Exchange some named colors with hexadecimal color values.
* Add some semi-transparent overlays to the banner and footer using RGBA.
* Fill in the first color column of the swatch samples using HSL colors.

## Tasks
1. In style.css, find the three CSS rules that use the named color _orange_. This color is not exactly the right orange to match the paint store brand. Replace _orange_ with the hex color _#ff8000_.
* The first place of _orange_ is the background of the header, under the selector _header_.
* The second location is the text color for the “Color Guide” heading, under the selector `#color-guide h2`.
* The final location is in the button in the footer, under the selector `footer .button`.

2. Make the main title text of the `h1` element semi-transparent to match the spooky text theme. To do so, set the `color` property with _rgba()_ to make the text black _(0 for red, green, and blue values)_ with _0.7_ alpha value.

3. Give the header’s background image a semi-transparent orange overlay to simulate a photographic filter.

In the `#banner:before` selector on line 95, add a background color with the value _rgba(255, 128, 0, 0.75)_.

4. Now do the same for the footer, adding a semi-transparent layer on top of the image to soften and darken it.

Find the selector `footer:before` and add a background color with same semi-transparent value that you used for the `h1` element.

5. Soften the subtitles which say “Saturation,” “Lightness,” and “Hue.” Currently, they are the default black.

Add a property to the `.color .swatches h4` rule to change the text color to the light gray hex value _#9b9b9b_.

6. There are three `span` tags which describe the “base color” for each color section. Each of them falls under a `<div>` tag with a class specific to the color. Currently, all these base colors are described with hex values. Change these to HSL.

For example, the value for color within the rule `.reds .base-color` is currently _#ff002b_. Change this to the HSL value _hsl(350, 100%, 50%)_.

You can find the base color values for the green and blue sections in the web page text. Update those to their corresponding HSL value as well.

7. In each section (red, green, and blue), there are 15 color cells. Each cell has its own rule specifying its color in style.css. Notice that at the beginning of each color swatch, the first cell is empty. Find the rule for each of the empty cells and fill in the _hsl()_ value which completes the pattern.

For example, the first blank swatch is `.reds .lightness .color-1`. In each HSL value in this section, notice that the lightness value decreases by 15 percentage points. Following the pattern, fill in the value for the background-value for this cell, `hsl(350, 100%, 80%)`.

Use the patterns for each of the other 8 rows and fill in the missing cell for each row.

In **style.css**, there is a comment above each empty cell’s rule that describes the pattern.
