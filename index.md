# Chinese Annotator for Microsoft Word #

A Microsoft Word add-in for adding tone graphs, pinyin or zhuyin to Hanzi（汉字）.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/Welcome.png)

The tones are automatically placed above the chinese characters, by the computer using a dictionary ([CC-CEDICT](http://www.mdbg.net/chindict/chindict.php?page=cedict)) for the longest word it can find. If it is unsure of the tones, it will place multiple tones above the character (here 好， as 大家好 is not in the dictionary as one word).

To annotate tones for [LaTeX](http://www.latex-project.org/), see [hanzi2tghz](http://code.google.com/p/hanzi2tghz/).


## Installation
0. Download [the installer](https://sourceforge.net/p/tghz-word-tone-annotator/code/HEAD/tree/trunk/Publish/setup.exe?format=raw).
0. Run the [the installer](https://sourceforge.net/p/tghz-word-tone-annotator/code/HEAD/tree/trunk/Publish/setup.exe?format=raw).
0. Open Word and the hanzi2tghz ribbon should be there. 
0. If any of the previous steps failed, _please_ write about them on the [issues](https://github.com/twighk/tghz-word-tone-annotator/issues) page or  [email me](http://www.google.com/recaptcha/mailhide/d?k=01NPKkqVdpvGCxT19t2FK-Zw==&c=nCA8B1q_gIq9ORG1LB4DfW-z0SdUwQXlicZ-lR7pil8=).
0. Read the documentation, to see what it can do.
0. Any feedback would be much appreciated. Please write about it on the  [issues](https://github.com/twighk/tghz-word-tone-annotator/issues) page or  [email me](http://www.google.com/recaptcha/mailhide/d?k=01NPKkqVdpvGCxT19t2FK-Zw==&c=nCA8B1q_gIq9ORG1LB4DfW-z0SdUwQXlicZ-lR7pil8=).



## Documentation 
Before use, please remember to make a backup of your document, just in case.
### Contents 
0. [Tones, Pinyin or Zhuyin Fuhao](https://twighk.github.io/tghz-word-tone-annotator/#tones-pinyin-or-zhuyin-fuhao)
    1. [Adding](https://twighk.github.io/tghz-word-tone-annotator/#adding)
    1. [Removing](https://twighk.github.io/tghz-word-tone-annotator/#removing)
    1. [Editing](https://twighk.github.io/tghz-word-tone-annotator/#editing)
0. [Resizing Text](https://twighk.github.io/tghz-word-tone-annotator/#resizing-text)
0. [Dictionary Correction](https://twighk.github.io/tghz-word-tone-annotator/#dictionary-correction)
    1. [Enabling Dictionary Correction](https://twighk.github.io/tghz-word-tone-annotator/#enabling-dictionary-correction)
    1. [Editing the Corrections Dictionary](https://twighk.github.io/tghz-word-tone-annotator/#editing-the-corrections-dictionary)
    1. [Importing and Exporting](https://twighk.github.io/tghz-word-tone-annotator/#importing-and-exporting)
0. [Colouring Tones](https://twighk.github.io/tghz-word-tone-annotator/#colouring-tones)
0. [Converting Traditional/Simplified Characters](https://twighk.github.io/tghz-word-tone-annotator/#converting-traditionalsimplified-characters)
0. [Troubleshooting](https://twighk.github.io/tghz-word-tone-annotator/#troubleshooting)
    1. [Certificate Error](https://twighk.github.io/tghz-word-tone-annotator/#certificate-error)
    1. [Visual Studio Tools for Office Solution Installer Error](https://twighk.github.io/tghz-word-tone-annotator/#visual-studio-tools-for-office-solution-installer-error)
    1. [Other Problems](https://twighk.github.io/tghz-word-tone-annotator/#other-problems)



### Tones, Pinyin or Zhuyin Fuhao 
![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/Tones%20or%20Pinyin.png)

#### Adding 
To add tones or pinyin to text select some, or all the text (`Ctrl+a`), and press either the `Add Tones`, `Add Pinyin` or `Add Zhuyin` Button. When the dictionary finds multiple pronunciations for tones it puts multiple tones. For Pinyin or Zhuyin, it duplicates the words with the various pronuciations. To reduce duplicates use the Dictionary Correction utilities.

When tones or pinyin are added, all the font information about the text before is lost, so the size, colour, font, etc. are reset to the default.   

#### Removing 
When removing tones or pinyin, it is preferable to use the `undo` button, to undo the previous action of adding them. For tones, the `Remove Tones/Pinyin` button can be used, but it can be problematic for pinyin, as it does not remove the duplicated characters caused by converting to pinyin. 

#### Editing 
To edit tones or pinyin, click on or select some text, then press the `Edit Tones or Pinyin` button and the incorrectly named `Edit Text or Pinyin` window should appear.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/EditTextOrPinyin.png)

Here 大家好 has tones, and 欢迎来到我的网站 has pinyin. For tones, put the number of the tone or tones, in the text box on the right. For pinyin put the pinyin followed by the tone number.





### Resizing Text 
When the text is resized the tone/pinyin do not scale with the text size. The solution is to use one of the `resize` buttons.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/Resize.png)

#### Pinyin or Zhuyin Fuhao 
To resize pinyin or zhuyin fuhao, use the `Pinyin Resize:` button. The number next to it (`0.5` is the default) is the relative size of the text compared to the characters, i.e. `0.5` is half the size, `1.0` is the same size.

#### Tones 
For Tones there are two issues the size of the tones and the height of the tones above the characters. For the size of the tones use the `Tone Resize:` button and change the relative size if you wish. For the height of the tones, change the number next to the `Tone Height:` button (`12` is the default, make it larger for larger text), then click the `Tone Height:` button.




### Dictionary Correction 
#### Enabling Dictionary Correction 
To enable dictionary correction press the `Enable` button in the `Dictionary Corrections` Section of the toolbar/Ribbon. By default there are no corrections, you can see the avaliable corrections, by pressing the `Edit Dictionary` in the `Dictionary Corrections` section. To import a tone corrections dictionary, or make yourown, see below.

#### Editing the Corrections Dictionary
To open the Dictionary Corrections window press the `Edit Dictionary` button.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/DictionaryCorrections.png)

Press the `Done` button to close the window saving changes. 
##### Adding Words 
To add a correction, type the chinese characters in the box containing `汉字` and the pinyin, separated by character by spaces, postfixed with the tone graph number, in the `han4 zi4` box. Then press the `Add` button and it should be copied into the list. See the above window for examples.

For multiple pronuciations add the same chinese characters twice, with different pronunciations.

##### Deleting Words 
To delete words, select the large grey box to the left of the row you wish to delete, and press the delete key. There is no button in the window to do this.

##### Editing Words 
The words in the dictionary cannot be edited, to preven errors in the program. To edit one delete it, and add the corrected version.

##### Enabling/Disabling Words 
Words can be enabled or disabled individually, buy having the tickbox checked or unchecked, respectively.


#### Importing and Exporting 
Edits to the dictionary can be imported or exported, to enable sharing, by selecting an option in the `File` Menu.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/DictionaryCorrectionsImportExport.png)

Currently there is no undo mechanism for this. The tone corrections file is a hidden file called `tghzToneCorrections.txt` in your personal user or home folder. The file can be backed up by exporting it (see below) or making a duplicate. Deleting this file should cause a new empty file.

##### Importing 
To import a tone corrections file, press the `Edit Dictionary` button, and then `File -> Import Dictionary Corrections File` from the menu bar in the `Dictionary Corrections` window. A file dialog box will appear allowing you to choose the file to import. Please be careful to select the correct file.

Here is my [Tone Corrections File](https://raw.githubusercontent.com/twighk/tghz-word-tone-annotator/master/Hanzi2TGHZRibbon/ToneCorrections.txt). To download it, right-click the hyperlink and choose `Save Link As...`, or similar.

##### Exporting 
To export a tone corrections file, press the `Edit Dictionary` button, and then `File -> Export Dictionary Corrections File` from the menu bar in the `Dictionary Corrections` window. A file dialog box will appear allowing you to choose where to export the file to.

### Colouring Tones 
Tones/pinyin and/or characters can be coloured using the colour button. Tick the box(es) before adding tones or pinyin for the output to also be coloured.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/Welcome%20Color.png)




### Converting Traditional/Simplified Characters 
To convert from traditional or simplified to simplified or traditional, select the text and press the `To Simplified` or `To Traditional` buttons, respectively.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/TraditionalSimplified.png)


### Troubleshooting 
If you have any problems, please feel free to [email me](http://www.google.com/recaptcha/mailhide/d?k=01NPKkqVdpvGCxT19t2FK-Zw==&c=nCA8B1q_gIq9ORG1LB4DfW-z0SdUwQXlicZ-lR7pil8=).

#### Certificate Error
While running the setup file there may be a certificate error:

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/certerror.png)

, because it is installing from an untrusted location.

To fix this, `https://tghz-word-tone-annotator.googlecode.com` needs to be added to the list of trusted sites:

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/certerrorfix.png)

Open Internet Explorer, and click the `Gear Icon` (top right corner) and then choose `Internet Options`. In the `Internet Options` window select `Security`, then `Trusted Sites`, then click the button that says `Sites`. In the `Trusted sites` window copy and paste:

`https://tghz-word-tone-annotator.googlecode.com`

and `Add` it. It should now be possible to install the program.

### Visual Studio Tools for Office Solution Installer Error
While running the setup file, there may be an error message with the `Visual Studio Tools for Office Solution Installer`.

![](https://github.com/twighk/tghz-word-tone-annotator/raw/master/Images/VSTOInstaller.png)

To fix this, please run the setup program as an administrator.

(This problem was seen on Windows 8.1)

### Other Problems
If there are any other problems with using or installing the software, please [email me](http://www.google.com/recaptcha/mailhide/d?k=01NPKkqVdpvGCxT19t2FK-Zw==&c=nCA8B1q_gIq9ORG1LB4DfW-z0SdUwQXlicZ-lR7pil8=) or [submit an issue](https://github.com/twighk/tghz-word-tone-annotator/issues).
