# What is this repo
It's a repository of fonts that are used in rich content designs.

# Purpose
Purpose of this repository is to have a place for hosting custom fonts.

# Reason
I created this repo because of numerous issues with fonts. Some eRetailers don't allow font files, some allow only Google Fonts, but there are cases where the design uses custom fonts (aka not from Google), there are cases where the designer didn't send font file, etc.
To prevent such issues and streamline smooth RC delivery I decided it would be helpful to have such a repository.

# How to use
## STEP 1.
Find the name and weight of the font you need in the file structure.
## STEP 2.
In CSS file, add this:
```
@font-face {
    font-family: "[Font-Name]";
    src: url("https://estorelabs.github.io/FONTS/[folder-name]/[font-filename.format]") format("[format]");
    font-weight: [weight];
    font-display: swap;
}
```
Replace everything [between square brackets] with your desired font family.

for example, for Gilroy Regular:
```
@font-face {
    font-family: "Gilroy-Regular";
    src: url("https://estorelabs.github.io/FONTS/Gilroy/Gilroy-Regular.otf") format("otf");
    font-weight: 400;
    font-display: swap;
}
```
## STEP 3.
Done, it should work.

# How to expand on it
1. One font family should go into one folder.
2. One folder can contain multiple font files in many formats. .woff2 and .woff are preferred.
3. Naming convention: `Family-Variation.format`. e.g. `FONTS/Gotham/Gotham-Black.ttf`.
4. For each new RC design that doesn't use Google Fonts, add font files here and host them in the master.

# Important
For the hosting to work, repo needs to be public (however I'm not 100% sure it's correct, but better safe than sorry).

# License
No loicense unless The Important People decide otherwise.