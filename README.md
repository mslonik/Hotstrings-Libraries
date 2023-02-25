# Hotstrings-Libraries <a name="back-to-the-top"></a>

Hotstring library is text file (*.csv) formatted to work with [*Hotstrings*](https://github.com/mslonik/Hotstrings) application, which is text replacement tool.

In this article there are described libraries belonging to the following cathegories:

# List of content

1. [List of free library files.](#free-library-files)
2. [List of not-free library files.](#not-free-library-files)
3. [List of free "second instance" library files.](#free-second-instance)
4. [Text replacement format and naming convention.](#text-replacement-format)
5. [Library file format.](#library-file-format)

<br />
<br />
<br />

## **The free library files** <a name="free-library-files"></a>

| no. | library name                                                    | library description                                                                                    | no. of definitions within library |
|:----|:----------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------|:---------------------------------:|
| 1.  | (Typer Helper) DevanagariTyperHelper_VowelSet.csv               | Helps type orthographic characters not found on the keyboard.                                          |                ???                |
| 2.  | (Typer Helper) GreekSigmaHelper.csv                             | Helps type orthographic characters not found on the keyboard.                                          |                ???                |
| 3.  | (Typer Helper) GurmukhiTyperHelper_VowelSet.csv                 | Helps type orthographic characters not found on the keyboard.                                          |                ???                |
| 4.  | (Unicode Sender) Combining Diacritics.csv                       | Helps type orthographic characters not found on the keyboard.                                          |                ???                |
| 5.  | (Unicode Sender) Computer-Keys Symbols.csv                      | Helps type the symbols of world currencies.                                                            |                ???                |
| 6.  | (Unicode Sender) Currency Symbols.csv                           | Helps type computer-keys symbols.                                                                      |                ???                |
| 7.  | (Unicode Sender) Ligatures.csv                                  | Helps type computer-keys symbols.                                                                      |                ???                |
| 8.  | (Unicode Sender) Mathematical (Needs Improvement).csv           | Helps type computer-keys symbols.                                                                      |                ???                |
| 9.  | (Unicode Sender) Orthographic.csv                               | Helps type computer-keys symbols.                                                                      |                ???                |
| 10. | (Unicode Sender) Roman Numerals.csv                             | Helps type computer-keys symbols.                                                                      |                ???                |
|     |                                                                 |                                                                                                        |                                   |
| 11. | [AbbreviationsEnglish.csv](#abbreviations-english)              | Acronyms / abbreviations typical for English language.                                                 |               ~550                |
| 12. | [AutocompleteBrackets.csv](#autocomplete-brackets)              | Adds closing bracket and shifts cursor in between the brackets.                                        |                 5                 |
| 13. | [AutoCorrect.csv](#auto-correct)                                | Hotstrings to correct common English misspellings on-the-fly.                                          |               4841                |
| 14. | [AutoCorrectionHotstrings.csv](#auto-correction-hotstrings)     | Automatic corrections of mispelled words and couple more abbreviations.                                |                18                 |
| 15. | [BoxDrawing.csv](#box-drawing)                                  | ASCII box drawing characters.                                                                          |                 8                 |
| 16. | [CapitalLetters.csv](#capital-letters)                          | Auto-capitalization of first letter in the first word like week days, month days, geographical names.  |                ~80                |
| 17. | [CircledNumbers.csv](#circled-numbers)                          | Unicode characters: numbers or letters inside of circles.                                              |                46                 |
| 18. | [DiacriticsDeadkey_Polish.csv](#diacritics-deadkey-polish)      | Demonstration of dead key hotstrings used to enter diacritic characters (actually Polish diacritics).  |                18                 |
| 19. | [DiacriticsHotstrings.csv](#diacritics-hotstrings)              | So called diacritics or accented letters not present in English.                                       |                ~25                |
| 20. | [EmojiHotstrings.csv](#emoji-hotstrings)                        | Unicode characters called emojis.                                                                      |                ~75                |
| 21. | [Examples_TestLib.csv](#examples-testlib)                       | Example and test definitions which check specific features of Hotstrings application.                  |                27                 |
| 22. | [FileFormats.csv](#file-formats)                                | File formats specific.                                                                                 |                44                 |
| 23. | [Finance.csv](#finance)                                         | Abbreviations and definitions dedicated to subject of finances.                                        |                30                 |
| 24. | [FirstNameCapitalizer.csv](#first-name-capitalizer)             | Replaces text string representing first name with first capitalized first letter.                      |                40                 |
| 25. | [FunctionKeys.csv](#function-keys)                              | Option to call function keys (or F keys): F1 ... F24 just by typing ordinary letters.                  |                36                 |
| 26. | [HotstringsHotstrings.csv](#hotstrings-hotstrings)              | Prepare triggerstring tips about hotstrings active for Hotstrings application.                         |                 9                 |
| 27. | [Incoterms.csv](#incoterms)                                     | Abbreviations and full definitions of Incoterms.                                                       |                24                 |
| 28. | [Markdown.csv](#markdown)                                       | Markdown lightweight markup language cheat sheet.                                                      |                15                 |
| 29. | [PersonalHotstringsTemplate.csv](#personal-hotstrings-template) | Personal hotstrings template.                                                                          |                13                 |
| 30. | [PhysicsHotstrings.csv](#physics-hotstrings)                    | Various unicode symbols more or less related to physics.                                               |                ~75                |
| 31. | [polski.csv](#polski)                                           | Mix of various subcategories such as abbrevitaions, "capital letters", Polish specific "auto correct". |                ~20                |
| 32. | [Punctuation.csv](#punctuation)                                 | Punctuation and non-breaking characters.                                                               |                ~20                |
| 33. | [TimeHotstrings](#time-hotstrings)                              | Definitions of time.                                                                                   |                22                 |

Remarks:
1. Only single definitions are counted. It means that if compound definition is present, then it is counted as one.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

| 12. |              FirstCapital.csv              | Auto-capitalization of the first letter in the first word of each new sentence.                       |                 100                   |


---
### **AbbreviationsEnglish.csv** <a name="abbreviations-english"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Maciej Słojewski (🐘)

**Purpose**: Acronyms (fitting into cathegory of abbreviations) can be used in up to 3x forms:
- short version, e.g. **ADC**,
- expanded version, e.g. **Analog to Digital Converter**,
- full version, explaining definition of acronym: 

Thanks to **Hotstrings** application all three forms can be easily applied.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |                                                                                                hotstring                                                                                                | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------:|
|           adc           | → |            C            | → |                                                                                                   ADC                                                                                                   |       SI        |
|          adc/           | → |            *            | → | Analog to Digital Converter¦analog-to-digital converter is a system that converts an analog signal, such as a sound picked up by a microphone or light entering a digital camera, into a digital signal |       MSI       |

**Remarks:** 

1. Convention. For any of my *Abbreviation** libraries I use the following convention: 
   - If I want to immediately trigger a triggerstring, I use one of the characters freely available keys of keyboard, but seldomly used for other purposes. There are coupe of candidates: "~", "/", "\". I decided to use "/" as it is relatively easy reachable.
   - According to my style of writing, a short version of acronym is usually present at the end of a sentence. To trigger automatic text replacement it is enough to press one of usual triggers just after short version (e.g. adc and space, dot (.), colon (,) etc.). This way I don't have to enter any of acronym letters as capitals - they are converted to capitals by AutoHotkey automatically. It speeds up writing enormously on longer run. Additionally I use option "C": in case I'd enter abbreviation in capital letters (following above example: ADC), then AutoHotkey is not used to convert it between small letters and capital letters, what spares some time of microprocessor 😉.
   - Additionally for reference purposes for some definitions I use comment field (part of hotstring definition) for storage of link to definition (e.g. from Wikipedia).

1. Unification of language / culture.
   - If many people use the same set of abbreviations and definitions in written form, it builds at customers confidence and understanding. The same terms, the same definitions brings together and reduces area for misunderstanding. You can use **Hotstrings** aplication as basic aid for understanding.
   - You can use the same principle for definitions and names of your products in your company. For example all people in e-mail correspondence will use the same, unified definitions, no matter if it is technical documentation, datasheet or just a marketing leaflet.

1. Sometimes acronym names are the same as entire word. Good example in English is word "can". There is also acronym "CAN" which can stand for "Controller Area Network". It can be sometimes confusing when it is triggered automatically in unwanted situation. The fallback scenario is to undo last hotstring by pressing shortcut key combination dedicated to Hotstring application and that purpose (by default Win + Z). But if it is still unconvenient, you can define another triggerstring. For this particular acronym I use can\<Tab>, what is denoted as "can\`t", where "\`t" stands for \<Tab> or tabulator key.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **AutocompleteBrackets.csv** <a name="autocomplete-brackets"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Maciej Słojewski (🐘)

**Purpose**: Usually brackets come in pairs, e.g. after the opening ordinary bracket "(" comes the closing one ")". Definitions within this library automatically add closing bracket and also shifts cursor position in between pair of brackets in order to enable typing.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|            (            | → |           *B0           | → |  ){left}  |       SI        |

Meaning of options:
- "*" the trigger is a part of triggerstring (trigger = "(").
- B0 the triggerstring will be not erased (Backspaced).

Meaning of hotstring:
- {left} stands for special keyboard key: left cursor "←".

**Remarks**:
1. The hotstrings are so common and handy that keys used for closing brackets can be reserved for other purposes, e.g. can be used as triggers.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **AutoCorrect.csv** <a name="auto-correct"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Author: Jim Biancolo and Wikipedia's Lists of Common Misspellings.

**Purpose**:		Hotstrings to correct about 4700 common English misspellings on-the-fly.
                  The file downloaded following the first link after convertion to Hotstrings application format.	

1. https://www.autohotkey.com/download/AutoCorrect.ahk
2. https://www.autohotkey.com/docs/v1/Hotstrings.htm#AutoCorrect
3. https://www.biancolo.com/blog/autocorrect/
4. https://en.wikipedia.org/wiki/Wikipedia:Lists_of_common_misspellings

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|         bilites         | → |            ?            | → | bilities  |       SI        |

Meaning of options:
- "?" whenever before triggerstring any alphanumeric is detected, the hotstring is triggered. This definition can be called even from within any word.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **AutocorrectionHotstrings.csv** <a name="auto-correction-hotstrings"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Maciej Słojewski (🐘)

**Purpose**:   Content of this library is based on the concept of *AutoCorrect* library. It contains definitions which I wanted to have in separate, smaller library file, which are somewhat specific to my usage.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|         molkky          | → |            *            | → |  mölkky   |       SI        |

Comment: name of Finnish coutry game. Origin written form contains diacritic character ö.
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **BoxDrawing.csv** <a name="box-drawing"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Maciej Słojewski (🐘)

**Purpose**:   ASCII box drawing characters. Based on: https://en.wikipedia.org/wiki/Box-drawing_character
Thanks to this library it is relatively easier to prepare ASCII only based block diagrams. Definitiots could be combined with ASCII box drawing online editors (e.g. https://textik.com/). Macros exchanging characters could be prepared e.g. in Notepad++.


**Example**:

*boxes1/* is replaced into
```
╒═╤╕
│ ││
╞═╪╡
╘═╧╛
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **CapitalLetters.csv** <a name="capital-letters"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		   Maciej Słojewski (🐘)

**Purpose**:      Automatically change capitalization of frequently used words like first names, day / month names, geographical names etc. Thanks to this library it is possible to enter those names quicker without pressing Shift keyboard keys.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|         sweden          | → |           C*            | → |  Sweden   |       SI        |

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **CircledNumbers.csv** <a name="circled-numbers"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		   Maciej Słojewski (🐘)

**Purpose**:      Unicode characters used to denote items on pictures / diagrams / figures. For some items it is useful to put text in form of Unicode characters to denote items. E.g. ⑤. Next, below picture, in a legend it is possible to reference to such item.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|         LiteraR         | → |           C*            | → | {U+24C7}  |       SI        |

*LiteraR* is replaced into
```
Ⓡ
```

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **DiacriticsDeadkey_Polish.csv** <a name="diacritics-deadkey-polish"></a>
**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		   Maciej Słojewski (🐘)

**Purpose**:      Demonstration of dead key hotstrings used to enter diacritic characters (actually Polish diacritics). Actually key used to enter diacritics is not dead as it is displayed on the screen, but concept is similar: two keys have to be entered to get one diacritic key. As "dead key" the slash "/" is applied.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|           /a            | → |           *C?           | → |     ą     |       SI        |

"k/at" is replaced into
```
kąt
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **DiacriticsHotstrings.csv** <a name="diacritics-hotstrings"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Maciej Słojewski (🐘)

**Purpose**:   [Accents or Diacritics](https://en.wikipedia.org/wiki/Diacritic) is a glyph added to a letter. Sometimes it is useful to enter one accented character without a need to temporarily switch keyboard layout or code page. For example correct spelling of French originated term "a la" is "à la" with accented "à".

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           a^            | → |           C*?           | → | å¦ä¦â¦à¦á¦ą¦ā |       MSI       |

Meaning of options:
- "?" whenever before triggerstring any alphanumeric is detected, the hotstring is triggered. This definition can be called even from within any word.
- "C" it is case sensitive (only ordinary letter "a" and caret ^ will produce corresponding hotstring).
- "*" the trigger is a part of triggerstring (trigger = "^").
After triggerstring + trigger is pressed, user can choose from the list of 7x diacritics one fitting to the current purpose.
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **EmojiHotstrings.csv** <a name="emoji-hotstrings"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Collection of [emoticons](https://en.wikipedia.org/wiki/Emoticon), [emojis](https://en.wikipedia.org/wiki/Emoji) and [ASCII art](https://en.wikipedia.org/wiki/ASCII_art).

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring    | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:--------------:|:---------------:|
|        flowers/         | → |            *            | → | 💐: 🌹🍀🌻🌺🌸 |       SI        |

"flowers/" is replaced into
```
💐: 🌹🍀🌻🌺🌸
```

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **Examples_TestLib.csv** <a name="examples-testlib"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Examples of use, test suit for Hotstrings application. Set of definitions to test Hotstrings application.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           ex6/            | → |           *           | → | newline (linefeed/LF) `n |       SI       |

"ex6/" is replaced into
```
newline (linefeed/LF) 

```

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **FileFormats.csv** <a name="file-formats"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   
1. Explain meaining of specific file extensions / name of applications which apply that name. 
2. Enables entering not capitalized file extensions within filenames. 
3. Capitalize file extension names when such extension is present standalone.

**Example**:

Ad. 1. 
| triggerstring + trigger | → | (triggerstring) options | → |        hotstring         | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:------------------------:|:---------------:|
|          svg/           | → |            *            | → | Scalable Vector Graphics |       SI        |

svg is replaced into
```
Scalable Vector Graphics
```

Ad. 2. 
| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|          .svg           | → |           B0?           | → |           |       SI        |

"Filename.svg" is replaced into 
```
Filename.svg
```
(hotstring was triggered, but file extension wasn't capitalized). 


Ad. 3. 
| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|           svg           | → |                         | → |    SVG    |       SI        |

"This is file extension svg." is replaced into
```
This is file extension SVG.
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **Finance.csv** <a name="finance"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Abbreviations and definitions dedicated to subject of finances.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |      hotstring       | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:--------------------:|:---------------:|
|          bic/           | → |            *            | → | Bank Identifier Code |       SI        |

"bic/" is replaced into
```
Bank Identifier Code 

```

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **FirstNameCapitalizer.csv** <a name="first-name-capitalizer"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Replaces text string representing first name with first capitalized first letter.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|         daniel          | → |            *            | → |  Daniel   |       SI        |

"daniel" is replaced into
```
Daniel 

```

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **FunctionKeys.csv** <a name="function-keys"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Option to call function keys (or F keys): F1 ... F24 just by typing ordinary letters.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|          f10/           | → |            *            | → |   {F10}   |       SI        |

"f10/" is replaced into pressing of F10 function key. It's behavior is application dependant, but in many applications menu is activated.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **HotstringsHotstrings.csv** <a name="hotstrings-hotstrings"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Prepare triggerstring tips about hotstrings active for Hotstrings application. All the hotsrings start from "hs" and have "immediate execute" (*)  feature and have no replacement string (they are removed after). Thanks to that user should be able to find and least what hotstrings exist.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|        hsenable/        | → |            *            | → |           |       SI        |

If option "show triggerstring tips" is enabled in configuration of Hotstrings application and this library is enabled, then user should see on the screep triggerstring tip after entering "hs" (hotstring) what options from within this library are available in form of hotstrings.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **Incoterms.csv** <a name="incoterms"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Abbreviations and full definitions of Incoterms.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |                                                                                                                                                                                                                                                                                                                                                                                                              hotstring                                                                                                                                                                                                                                                                                                                                                                                                              | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------:|
|          cfr/           | → |            *            | → | Cost and Freight (named port of destination)¦The seller pays for the carriage of the goods up to the named port of destination. Risk transfers to buyer when the goods have been loaded on board the ship in the country of Export. The shipper is responsible for origin costs including export clearance and freight costs for carriage to the named port. The shipper is not responsible for delivery to the final destination from the port (generally the buyer's facilities), or for buying insurance. If the buyer requires the seller to obtain insurance, the Incoterm CIF should be considered. CFR should only be used for non-containerized seafreight and inland waterway transport; for all other modes of transport it should be replaced with CPT.¦https://en.wikipedia.org/wiki/Incoterms#FCA_%E2%80%93_Free_Carri |       MCL       |

If user enters "cfr/", then on the screep hotstring menu is displayed. After choosing the second poition it is replaced into:
```
The seller pays for the carriage of the goods up to the named port of destination. Risk transfers to buyer when the goods have been loaded on board the ship in the country of Export. The shipper is responsible for origin costs including export clearance and freight costs for carriage to the named port. The shipper is not responsible for delivery to the final destination from the port (generally the buyer's facilities), or for buying insurance. If the buyer requires the seller to obtain insurance, the Incoterm CIF should be considered. CFR should only be used for non-containerized seafreight and inland waterway transport; for all other modes of transport it should be replaced with CPT.
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **Markdown.csv** <a name="markdown"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Markdown lightweight markup language cheat sheet.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |                                                                       hotstring                                                                       | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-----------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------:|
|        mdcolor/         | → |            *            | → | hex color: `{#}0969DA`¦RGB color: `rgb(9, 105, 218)`‖https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-format |       MSI       |

If you enter "cfr/", then on the screep hotstring menu is displayed. After choosing the second poition it is replaced into:
```
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-format
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **PersonalHotstringsTemplate.csv** <a name="personal-hotstrings-template"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Personal hotstrings template.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |            hotstring             | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:--------------------------------:|:---------------:|
|         cardmy/         | → |            *            | → | 1122334455667788¦123¦07/26¦07¦26 |       MSI       |

If you enter "cardmy/", then on the screep hotstring menu is displayed containing all data relevant to register your bank card. After choosing the second poition it is replaced into your bank card secret code:
```
123
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **PhysicsHotstrings.csv** <a name="physics-hotstrings"></a>

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Various unicode symbols more or less related to physics.

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|           <=            | → |            *            | → |     ≤     |       CL        |

If you enter "<=" it is replaced into:
```
≤
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **polski.csv** <a name="polski"></a>
**Author**:		Maciej Słojewski (🐘)

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Mix of various subcategories related to Polish language such as abbrevitaions, "capital letters", "auto correct".

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |            hotstring             | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:--------------------------------:|:---------------:|
|         cardmy/         | → |            *            | → | 1122334455667788¦123¦07/26¦07¦26 |       MSI       |

If you enter "cardmy/", then on the screep hotstring menu is displayed containing all data relevant to register your bank card. After choosing the second poition it is replaced into your bank card secret code:
```
123
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **Punctuation.csv** <a name="punctuation"></a>
**Author**:		Julia Kierska, Maciej Słojewski

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Punctuation and non-breaking characters.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|        emspace/         | → |           *?            | → | {U+2003}  |       SI        |

If you enter "emspace/" even in a middle of a word, it is replaced into "em space" which is wider than normal space. "cateemspace/dog" is replaced into:
```
cat dog
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **TimeHotstrings** <a name="time-hotstrings"></a>

**Author**:		Maciej Słojewski

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Purpose**:   Definitions of time.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |    hotstring    | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------------:|:---------------:|
|           d[            | → |            *            | → | A_YYYYA_MMA_DD_ |       SI        |

If you enter "d[" it is replaced into:
```
20230225_
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
## **The not-free libraries** <a name="not-free-library-files"></a>

In this section I show examples of other libraries which I use in my everyday life but which cannot be shared by various reasons (GDPR, licence constraints, proprietary names etc.).

| no. | library name                                       | library description                                                                                                                 | no. of definitions |
|:----|:---------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------|:------------------:|
| 1.  | [BrandAndProperNames.csv](#brand-and-proper-names) | Brand names (reserved), proper names (reserved), used in everyday life.                                                             |        ~100        |
| 2.  | [BuildingBlocks.csv](#building-blocks)             | Building blocks from specific template file of Microsoft Word                                                                       |         37         |
| 3.  | [dSAT.csv](#dsat)                                  | Text replacements valid for Diagnostic and Monitoring Technologies for Rolling Stock.                                               |        ~100        |
| 4.  | [FirstAndSecondNames.csv](#first-and-second-names) | Collections of abbreviated first and second names of my colleagues, sometimes also other personal data like phone numbers, e-mails. |         –          |
| 5.  | [ProjectSpecific.csv](#project-specific)           | Collections of abbreviations, terms, definitions which are specific to one project.                                                 |         –          |
| 6.  | [TechnicalHotstrings.csv](#technical-hotstrings)   | Technical standards, technical documents useful on time of authoring technical documentation.                                       |         –          |
| 7.  | [SubjectSpecific.csv](#technical-hotstrings)       | Collections of abbreviations, terms, definitions which are specific to one subject.                                                 |         –          |
| 8.  | [ProductSpecific.csv](#technical-hotstrings)       | Collections of abbreviations, terms, definitions which are specific to one product.                                                 |         –          |
| 9.  | [CompanySpecific.csv](#technical-hotstrings)       | Collections of abbreviations, terms, definitions which are specific to one company.                                                 |         –          |

Remarks:
1. Only single definitions are counted. It means that if compound definition is present, then it is counted as one.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **BrandAndProperNames.csv** <a name="brand-and-proper-names"></a>

**Concept**: Brand names, proper names of products.

**Example**: joomla
| triggerstring + trigger | → | (triggerstring) options | → |             hotstring             | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------------------------------:|:---------------:|
|         joomla          | → |            *            | → | Joomla{!}¦https://www.joomla.org/ |       MSI       |
```
 Joomla!
```
Comment:
- special character "!" have to be escaped into "{!}"

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **BuildingBlocks.csv** <a name="building-blocks"></a>

**Concept**: Building blocks from Microsoft Word template file (.dotm or .dotx) must belong to "autotext" category. After entering "autotext" dedicated to specific building block F3 key has to be pressed. Next building block is inserted into document content. The definitions belonging to this library make sense only when: 1. Microsoft Word is open. 2. Active Microsoft Word document has attached specific template file.

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → |   hotstring    | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:--------------:|:---------------:|
|       @copyrights       | → |            *            | → | Copyrights{F3} |       SI        |

```
Company specific copyright note.
```

Comment:
- special character "F3" is called by entering in between curved brackets "{F3}"

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **dSAT.csv** <a name="dsat"></a>
**Concept**: In railway business certain specific definitions of common terms are applied. To keep unified lanugage this library was created.

**Example**: –

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **FirstAndSecondNames.csv** <a name="first-and-second-names"></a>
**Concept**: In formal e-mail correspondence or even in corporate text messengers it is good to have set ot first-name second-name abbreviations which are replaced with full Firstname Secondname, starting from capital letters. 

In some languages (e.g. Polish) endings of first-name and second-name are changed according to position and form in a sentence. Thanks to Hotstrings this local feature is addressed.

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → |                        hotstring                        | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------------------------------------------------:|:---------------:|
|           js/           | → |            *            | → | John Smith¦Johna Smitha¦Johnowi Smithowi¦Johnem Smithem |       MSI       |

"js/" is replaced into small on-screen menu and when 1st position is selected
```
John Smith 
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **ProjectSpecific.csv** <a name="project-specific"></a> 
**Concept**: Collections of abbreviations, terms, definitions which are specific to one project. Sometimes in commercial project are required literal definitions of notions, which can differ from other, well known sources of information. In such cases it is good to have handy set of definitions, which can be quickly and exactly called in any text / edit / input. Thanks to flexibility of *Hotstrings* application it is possible on the fly to switch on and off specific libraries when for example the same abbreviation is present in different projects. Another feature worth to remember is option to move specific definition from one library to another. Finally it is possible to place comments to specific definitions.

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → |                                                                                                                        hotstring                                                                                                                         | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------:|
|          atp/           | → |            *            | → | Automatic Train Protection¦The subsystem within Automatic Train Control system whichenforces safe operation, including speed restriction andseparation of trains running on the same track, unauthorizedtrain door opening, and over interlocked routes. |       MSI       |

"atp/" is replaced into small on-screen menu and when 2nd position is selected
```
The subsystem within Automatic Train Control system whichenforces safe operation, including speed restriction andseparation of trains running on the same track, unauthorizedtrain door opening, and over interlocked routes. 
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **TechnicalHotstrings.csv** <a name="technical-hotstrings"></a>
**Concept**: Technical standards, technical documents useful on time of authoring technical documentation. Collection of technical standards short names which are complemented in full form with dates, exact title. Useful on time of bringing references to technical documentation, quotations, building lists of references.

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → |                                       hotstring                                       | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------------------------------------------------------------------------------:|:---------------:|
|        iso14001/        | → |            *            | → | ISO 14001:2015 Environmental management systems ─ Requirements with guidance for use. |       SI        |

"iso14001/" is replaced into 
```
ISO 14001:2015 Environmental management systems ─ Requirements with guidance for use
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **SubjectSpecific.csv** <a name="technical-hotstrings"></a>
**Concept**: Collections of abbreviations, terms, definitions which are specific to one subject, e.g. "information security (cybersecurity)".

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → |                          hotstring                           | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:------------------------------------------------------------:|:---------------:|
|      asset owner/       | → |            *            | → | individual or organization responsible for one or more IACSs |       SI        |

"asset owner/" is replaced into 
```
individual or organization responsible for one or more IACSs
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### **ProductSpecific.csv** <a name="technical-hotstrings"></a> 
**Concept**: Collections of abbreviations, terms, definitions which are specific to one product, e.g. "system".

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → | hotstring | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:---------:|:---------------:|
|          fp52           | → |            C            | → |   FP52    |       SI        |

"fp52," is replaced into 
```
FP52,
```
what saves some time on writing (two time less of Shift presses).

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
<details>
<summary><h3><b>CompanySpecific.csv</b></h3></summary> <a name="technical-hotstrings"></a>

**Concept**: Collections of abbreviations, terms, definitions which are specific to one company.

**Example**:
| triggerstring + trigger | → | (triggerstring) options | → |          hotstring           | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:----------------------------:|:---------------:|
|          hqct/          | → |            *            | → | Head of Quality Control Team |       SI        |

"hqct/" is replaced into 
```
Head of Quality Control Team
```
what saves some time on writing (two time less of Shift presses).

[Back to the top](#back-to-the-top)
<br />
<br />
<br />
</details>

---

## List of free "second instance" library files <a name="free-second-instance"></a>

Sooner or later collection of definitions is so large that definitions start to overlap. 

It is possible to prepare hotstrings, which will detect end of a sentence. In many languages sentences are finished with such characters as ".", "?", "!". New sentence usually is also started after pressing of "enter". Then it is enough to start next word with capital letter. Many text editors have in-build such functionality, many do not. This feature is called "first capital".

It is possible to run second instance of *Hotstrings* application with separate set of libraries. This trick helps to overcome overlapping of definitions which are present in the first instance. In order to run second instance please remeber to change name of the script or executable into something different. For example, the first (default) instance: *Hotstrings.ahk*, the second instance: *Hotstrings2.ahk*. Please also mind to keep libraries of second instance into separate folder.

Another trick which is necessary to enable "first capital" is to feed back characters produced by hotstring definitions back to hook buffer. Thanks to that produced hotstrings can be again part of new created triggerstring, which in a moment can trigger another hotstring. To make it possible there are new categories of libraries:

- S1: Unique feature: last character of hotstring will be fed back to hook buffer. Name of library file must start with "S1_", "output function" for all definitions within this file must be S1. 
- S2: Unique feature: last character of hotstring will be fed back to hook buffer. Name of library file must start with "S2_", "output function" for all definitions within this file must be S2.

At the moment there is no way to choose S1 or S2 "output functions" from GUI of *Hotstrings* application. The only way is manual edition of library files. But there are also good news. You can simply run second instance with already prepared libraries from the following table. Advice: switch off triggerstring tips at least for all S2 libraries.

| no. | library name                                                 | library description                                                                                              | no. of definitions |
|:----|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------|:------------------:|
| 1.  | [Exceptions.csv](#exceptions)                                | Exceptions to "first instance".                                                                                  |         1          |
| 2.  | [FirstCapitalExceptions.csv](#first-capital-exceptions)      | Because of overlapping between Hotstring instances some definitions have to be shifted to separate library file. |         23         |
| 3.  | [S2_BasicLayerToShiftLayer.csv](#basic-layer-to-shift-layer) | Method to get characters from the Shift layer without using Shift keys.                                          |         19         |
| 4.  | [S2_DoubleSpace.csv](#s2-double-space)                       | Double pressing of 2x space key converted into dot and space.                                                    |         26         |
| 5.  | [S2_DoubleSpace_Polish.csv](#s2-double-space-polish)         | Enables pressing of 2x space key converted into dot and space also for words finished with Polish diacritic.     |         9          |
| 6.  | [S2_FirstCapital.csv](#s2-first-capital)                     | When sentence is finished with . or ! or ? or \<Enter\> then next word is started with capital letter.           |        104         |
| 7.  | [S2_LayerKeys.csv](#s2-layer-keys)                           | Sends back some special characters, which can be used to control Hotstrings application.                         |         3          |

**TOTAL**: 185 (last checked on: 2023-02-25)

Remarks:
1. Only single definitions are counted. It means that if compound definition is present, then it is counted as one.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
## Where libraries are stored?

As it was already mentioned, the library file can caontain fragile / protected in law data. Therefore such files should be protected against public access. The basic way to accomplish this task is to store library files within <UserData>: 
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
## Text replacement format and naming convention <a name="text-replacement-format"></a>

|   text to be replaced   | → |   replacement options   | → | replaced text |      output function      |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:-------------------------:|
| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | how hotstring is produced |
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

## Library file format <a name= "library-file-format"></a>
(tbd)
[Back to the top](#back-to-the-top)
<br />
<br />
<br />