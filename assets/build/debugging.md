[⬅️ Take me back Home 🏡](../../README.md)

# Troubleshooting/FAQ

## Table of Contents
- [How does WordPress identify theme type?](#how-does-wordpress-identify-theme-type)
- [How to identify theme type from backend?](#how-to-identify-theme-type-from-backend)
- [What displays with minimum files?](#what-displays-with-minimum-files)

## How does WordPress identify theme type?
* If you have `index.html` in the theme files - then block
* If you have `index.php` in the theme files - then classic

## How to identify theme type from backend?
* If it is a classic theme, then you would see under appearance Customise, widgets and menus
* If it is a block theme, then you would see under appearance Editor instead of customize (no widgets or menus)

## What is displayed on the frontend with minimum files?
* *Classic Theme :*  You see a white screen, no header/footer, wpadminbar
* *Block Theme :* "Empty template: Index". (with wpadminbar - if logged in)

## My theme.json custom settings are not reflecting.
* some of the syntax of theme.json might be invalid. use your IDE to check or validate on 

## JSON Formatting - Highlights
* Data is in name/value pairs
* Data is separated by commas
* Objects are encapsulated within the opening and closing curly brackets `{}`
* Arrays are encapsulated within opening and closing square brackets `[]`
* A member is represented by a key-value pair, contained in double quotes
* Each member should have a unique key within an object structure
* String : value of a member must be contained in double quotes
* Boolean : are represented using the true or false literals in lower case
* Number : are represented using double-precision floating-point format and * shouldn't have leading zeroes
* "Offensive" characters in a string need to be escaped using the backslash * character \
* Null values are represented by the null literal in lower case
* Each member of an object or array value must be followed by a comma, except for the last one
* The standard extension for the JSON file is '.json'