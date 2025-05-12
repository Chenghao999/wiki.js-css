[View Chinese Version](README_ZH.md)

# wikijs-citizen-styles

A Wiki.js override stylesheet inspired by the style of the MediaWiki skin at <mcurl name="StarCitizenTools/mediawiki-skins-Citizen" url="https://github.com/StarCitizenTools/mediawiki-skins-Citizen/"></mcurl>. I prefer a lighter style rather than the default blue and black of Wiki.js.

## Usage

1. Open the Wiki.js backend. Click the "Theme" menu on the left side.
2. **Do not** put the styles in the "CSS Override" section. Instead, insert a pair of HTML tags `<style type="text/css"></style>` in the "Body HTML Injection" section.
3. Open the downloaded `styles.css` file and copy all its contents into the `<style>` tags, like this: `<style type="text/css">...CSS content goes here...</style>`.

## Compilation

* Clone the project using `git clone https://github.com/AurLemon/wikijs-citizen-styles.git`.
* The project files are located in `src/styles.scss`. After configuring the runtime environment and package manager, you can build the project using `npm run build-css`. The compiled file will be in `dist/styles.css`.
* If you want to change the theme color, you can modify the following variables under the `:root` selector in the project file: `--color-primary-override__h: 200; --color-primary-override__s: 55%; --color-primary-override__l: 48%;`. The theme color uses the HSL color system, and these three CSS variables represent the hue, saturation, and lightness of the theme color respectively.
* If you want to change other colors, you can modify other CSS variables under the `:root` selector. After making the changes, compile the project and apply the styles according to the "Usage" instructions.
