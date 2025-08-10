# SuperStation One Menu for ES-DE

This is a translation of the SuperStation One menu interface for ES-DE (originally designed & created by RetroRemake)

My work focused on tranlating the layout so that it could be buildable in the theme engine for ES-DE.  Please refer to the `Changes Made` section below for additional details. 

The original version of the UI can be found as part of the OS available on the SuperStation One made by [RetroRemake](https://retroremake.co/pages/superstation%E1%B5%92%E2%81%BF%E1%B5%89)

## Changes Made

- Used [SuperStation One UI designs](https://x.com/TakiUdon_/status/1901576056966086781) to approximate the elements that would be used build a theme compatible with ES-DE.
- Changed the helpsystem to ES-DE's native component and created a layout that tries to evoke the original helpsystem design
- Added icons and badges specific to ES-DE functionality
- Added a framework for adding additional color schemes and added RGB options to start
- Added a user customization framework

## **Preview**

| System View | Gamelist View: List | Gamelist View: Carousel |
|----|----|----|
| ![System View](https://github.com/user-attachments/assets/b712241c-05d6-4d30-9715-42e98e2b6ce3) | ![Gamelist View - List](https://github.com/user-attachments/assets/d46f7b9c-1688-4204-a4bf-8a9fbbde15e4) | ![Gamelist View - Carousel](https://github.com/user-attachments/assets/b17991b8-3be2-4212-a111-1834dca1d7b3) |

## **Configuration Options**

The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 

### **Variants:**

- `Theme Variant` - sets the color scheme that is used for the overall theme on all views.
   - `List` - The default color variant.  A simple list
   - `List: Boxart` - Adds the display of boxart to the list
   - `List: Screenshot` - Adds the display of screenshots to the list
   - `List: Title Screen` - Adds the display of title screens to the list
   - `List: Physical Media` - Adds the display of physical media to the list
   - `List: Miximage` - Adds the display of miximages to the list
   - `Carousel: Boxart` - A carousel variant that displays game boxart

### **Color Schemes:**

- `Theme Color Scheme` - sets the color scheme that is used for the overall theme on all views.
   - `Black` - The default color scheme. 
   - `Green`
   - `Blue`
   - `Red`
   - `Custom` - Enables the ability to create a custom color scheme.  You can create your own custom color scheme by following the instructions under "[Creating your own color scheme](#creating-your-own-color-scheme)"

### **Font Sizes:**

- `Theme Font Size` - sets the size that text will render at. This can be helpful when using the theme on small screens.
   - Supported Font Sizes:
   - `Medium` - Default size, good for small handheld screens under 6 inches in size.
   - `Large` - Good for small handheld screens under 4 inches in size.
   - `Small` - Smaller size, good for larger screens.
   - `Extra Large` - Good for small handheld screens under 4 inches in size.

### **Aspect Ratios:**

- `Theme Aspect Ratio` - sets the aspect ratio to match your display. This should happen automatically but can also be set manually if needed.
   - Supported Aspect Ratios:
   - `4:3`
   - `16:9`
   - `16:10`
   - `3:2`
   - `19.5:9`
   - `1:1`
 
## Customizations

### **Creating your own color scheme:**

A custom color scheme lets you to modify any of the colors, images and fonts used in the theme while also allowing you to continue to get updates from the theme downloader.

1) In the resources folder you will find a template file called [colors.xml](https://github.com/anthonycaccese/superstation-one-menu-es-de/blob/main/resources/colors.xml)

2) Make a folder named `theme-customizations` and place a copy of the `colors.xml` file inside that folder.  The folder structure should look like this when you are done:
   ```
   /ES-DE/themes/superstation-one-menu-es-de/theme-customizations/colors.xml
   ```

3) Edit the properites in `colors.xml` to create your custom color scheme
    
4) Set the `Theme Color Scheme` in ES-DE's UI Settings menu to `Custom` and you should see your custom color scheme display.  If you see an error check that the paths discussed above are correct and then check that the values you added for each property are correct and well formatted.

> [!NOTE]
> If you make a custom color scheme and are comfortable with sharing it, I would love to check it out 😊
> - Please feel free to create an issue in this repo called `Custom Color Scheme: [Name of your Color Scheme]`
> - Include the values you used for the properties above (xml is preferred), the artwork and logos you added (if any) and a screenshot of what it looks like.

## **Credits:**

- The SuperStation One UI was originally created & designed by [RetroRemake](https://retroremake.co/pages/superstation%E1%B5%92%E2%81%BF%E1%B5%89)
- The included font is called ["Free Pixel"](https://www.dafont.com/free-pixel.font) and created by levelb
