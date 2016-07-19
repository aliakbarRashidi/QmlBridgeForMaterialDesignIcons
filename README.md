# QmlBridgeForMaterialDesignIcons

This project provides a simple interface for integrating the Material Design Icons font into Qt/QML projects, which pairs nicely with the new Material Design theme for Qt Quick Controls 2. It is released under the terms of the SIL Open Font License, version 1.1, in order to match the licensing terms that apply to the font.

To use this in your project:

    1. Download the Material Design Icons font, available at [https://materialdesignicons.com/](https://materialdesignicons.com/)
    2. Add the font file, and Icon.js from this project to the project's QRC file
    3. When initializing the application from C++, add the font to the font database, `QFontDatabase::addApplicationFont(":/materialdesignicons-webfont.ttf");`
    4. Import `Icon.js` in any QML file where icons will be referenced: `import "Icon.js" as MdiFont`
    5. Add the desired icon to any QML item that can display text
        * Set font.family to "Material Design Icons"
        * Set the text property to the desired property of MdiFont.Icon, e.g. MdiFont.Icon.mdiFileImage
