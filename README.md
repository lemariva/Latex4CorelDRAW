Latex4CorelDraw
--------------

This is a repository created from [Latex for CorelDraw](http://www.interactive-graphics.de/index.php/downloads/14-latex-for-coreldraw). Although [the new version](https://github.com/InteractiveComputerGraphics/Latex4CorelDRAW) offers more functionalities, it usually has some compatibility problems with new CorelDraw versions. This version is easier to maintain and works for almost every purpose.

## Prerequisites
* [MikTex](https://miktex.org/) >= 2.9.0
* [Ghostscript 64bits](https://www.ghostscript.com/download/gsdnld.html)
Add the folder `C:\Program Files\gs\gsx.xx\bin` to the [Windows path](https://docs.alfresco.com/4.2/tasks/fot-addpath.html).

## Instructions
1. Download the `LatexEdit.gms` file.
2. Right-click and open "Properties". If you see the following text, you have to unblock the file: 
"Security: This file came from another computer and might be blocked to help protect this computer."
3. Move the file inside the folder `C:\Program Files\Corel\CorelDRAW xxxx \Draw\GMS`
4. Go to `Tools->Options->Custumization` and add a shortcut to the `CorelMacros.LatexEdit` function (see Fig. 1)
5. Use the shortcut to open the GUI and enter the Latex text.

The first time that you use the macro you will need to install some Latex plugins. A CMD console will execute the installation, and you'll need to press some enters, click ok/install buttons, etc.

| |
|:--|
|![Add a shortcut to the CorelMacros.LatexEdit function](images/customization.jpg?raw=true "Add a shortcut to the CorelMacros.LatexEdit function")|
|Fig. 1: Add a shortcut to the CorelMacros.LatexEdit function|

If you've already written some text, you can edit that:
1. Select the object
2. Use the shortcut to open the GUI and edit the Latex text.

## Typical errors
* You can open and edit the macro going to `Tools->Scripts->Script Editor`. To edit and save the macro, you need to open CorelDraw with administration rights. Otherwise, you cannot edit the file under `C:\Program Files`.
* If the Latex text is not correctly displayed (Arial font), you need to install some fonts. Try to import the file `teximport_neu.ps` located inside `%%TEMP%%` folder (usually `C:\Users\<username>\AppData\Local\Temp`) using `File->Import`. By the import options, select **Text**. CorelDraw will popup a windows with subtitution recommendations for the fonts (see Fig. 2). Search [here](https://www.ctan.org/tex-archive/fonts/cm/ps-type1/bakoma/ttf/) and install those fonts. Then, repeat step 5. 

| |
|:--|
|![Fonts not installed](images/font_substitutions.jpg?raw=true "Fonts not installed")|
|Fig. 2: Check font name to install.|

## Acknowledge
[Prof. Dr. rer. nat. Jan Bender](http://www.interactive-graphics.de/index.php/downloads/14-latex-for-coreldraw)