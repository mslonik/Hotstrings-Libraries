# Hotstrings-Libraries <a name="back-to-the-top"></a>

Hotstring library is text file (*.csv) formatted to work with [*Hotstrings*](https://github.com/mslonik/Hotstrings) application, which is text replacement tool.

In this article there are described libraries belonging to the following cathegories:

# List of content

1. [List of free library files.](#free-library-files)
2. [List of not-free library files.](#not-free-library-files)
3. [Text replacement format and naming convention.](#text-replacement-format)
4. [Library file format.](#library-file-format)

<br />
<br />
<br />

## **The free library files** <a name="free-library-files"></a>

| no.  |              library name              | library description**                                                                               |                                    no. of definitions within library                                      |
| :--- |:------------------------------------------|:------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------:|
| 1. |  (Unicode Sender) Orthographic Sender.csv  | Helps type orthographic characters not found on the keyboard.                                         |                                  ~171                                   |
| 2. |   (Unicode Sender) Currency Symbols.csv    | Helps type the symbols of world currencies.                                                           |                                   61                                    |
| 3. | (Unicode Sender) Computer-Keys Symbols.csv | Helps type computer-keys symbols.                                                                     |                                   28                                    |
|    | [AbbreviationsEnglish.csv](#abbreviations-english)                   | Acronyms / abbreviations typical for English language.                                                | ~550                                                                    |
| 5. | [AutocompleteBrackets.csv](#autocomplete-brackets)                   | Adds closing bracket and shifts cursor in between the brackets.                                       |   5                                                                     |
|    | [AutoCorrect.csv](#auto-correct)                            | Hotstrings to correct common English misspellings on-the-fly.                                         |   4841                                                                  |                    
| 6. |        [AutoCorrectionHotstrings.csv](#auto-correction-hotstrings)        | Automatic corrections of mispelled words and couple more abbreviations.                               |                                  18                                    |
|    | [BoxDrawing.csv](#box-drawing)                             | ASCII box drawing characters.                                                                         | 8 
| 7. |             [CapitalLetters.csv](#capital-letters)             | Auto-capitalization of first letter in the first word like week days, month days, geographical names. |                                  ~80                                    |
| 8. |             [CircledNumbers.csv](#circled-numbers)             | Unicode characters: numbers or letters inside of circles.                                                        |                                   46                                    |
|  |             [DiacriticsDeadkey_Polish.csv](#diacritics-deadkey-polish)             | Demonstration of dead key hotstrings used to enter diacritic characters (actually Polish diacritics).                                                        |                                   18                                    |
| 9. |     DevanagariTyperHelper_VowelSet.csv     | (...)                                                                                                 |                   23                      |
|    |           [DiacriticsHotstrings.csv](#diacritics-hotstrings)          | So called diacritics or accented letters not present in English.                                      |                                  ~25                                    |
| 11. |            [EmojiHotstrings.csv](emoji-hotstrings)             | Unicode characters called emojis.                                                                     |                                  ~75                                    |
| 11. |            [Examples_TestLib.csv](examples-testlib)             | Example and test definitions which check specific features of Hotstrings application.                                                                     |                                  27                                    |
|  |            [FileFormats.csv](file-formats)             | 1. Explain meaining of specific file extensions / name of applications which apply that name. 2. Enables entering not capitalized file extensions within filenames. 3. Capitalize file extension names when such extension is present standalone.                                                                     |                                  44                                    |
| 12. |              FirstCapital.csv              | Auto-capitalization of the first letter in the first word of each new sentence.                       |                 100                   |
| 13. |              FunctionKeys.csv              | Option to call function keys (or F keys): F1 ... F24 just by typing ordinary letters.                 |                                   25                                    |
| 14. |      GurmukhiTyperHelper_VowelSet.csv      | (...)                                                                                                 |                    9                      |
| 15. |               Incoterms.csv                | Abbreviations and full definitions of Incoterms.                                                      |                             24                                |
| 16. |           PhysicsHotstrings.csv            | Various unicode symbols more or less related to physics.                                              |                                  ~55                                    |
| 17. |               TimeHotstrings               | Definitions of time formats.                                                                          |                                   3                                     |

Remarks:
1. Only single definitions are counted. It means that if compound definition is present, then it is counted as one.

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

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

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           (            | → |           *B0           | → | ){left} |       SI       |

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

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|   bilites               | → |           ?             | → | bilities      |       SI        |

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

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|   molkky               | → |           *             | → | mölkky      |       SI        |

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

*boxes1/* converts into
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

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           sweden            | → |           C*           | → | Sweden |       SI       |

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

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           LiteraR            | → |           C*           | → | {U+24C7} |       SI       |

*LiteraR* converts into
```
Ⓡ
```

[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
### DiacriticsDeadkey_Polish.csv <a name="diacritics-deadkey-polish"></a>
**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		   Maciej Słojewski (🐘)

**Purpose**:      Demonstration of dead key hotstrings used to enter diacritic characters (actually Polish diacritics). Actually key used to enter diacritics is not dead as it is displayed on the screen, but concept is similar: two keys have to be entered to get one diacritic key. As "dead key" the slash "/" is applied.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           /a            | → |           *C?           | → | ą |       SI       |

"k/at" converts into
```
kąt
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

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

**Purpose**:   Collection of [emoticons](https://en.wikipedia.org/wiki/Emoticon), [emojis](https://en.wikipedia.org/wiki/Emoji) and [ASCII art](https://en.wikipedia.org/wiki/ASCII_art).

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           flowers/            | → |           *           | → | 💐: 🌹🍀🌻🌺🌸 |       SI       |

"flowers/" converts into
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

**Purpose**:   Examples of use, test suit for Hotstrings application. Set of definitions to test Hotstrings application.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           ex6/            | → |           *           | → | newline (linefeed/LF) `n |       SI       |

"ex6/" converts into
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

**Purpose**:   
1. Explain meaining of specific file extensions / name of applications which apply that name. 
2. Enables entering not capitalized file extensions within filenames. 
3. Capitalize file extension names when such extension is present standalone.

**Example**:

Ad. 1. "svg/" converts into 
```
Scalable Vector Graphics. 
```

Ad. 2. "Filename.svg" converts into 
```
Filename.svg
```
(hotstring was triggered, but file extension wasn't capitalized). 


Ad. 3. "This is file extension pdf" converts into
```
This is file extension PDF
```
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

---
## **The not-free libraries** <a name="not-free-library-files"></a>

In this section I show examples of other libraries which I use in my everyday life but which cannot be shared by various reasons (GDPR, licence constraints, proprietary names etc.).

| no.   |   library name     | library description                                                                                                             |     no. of definitions      |
| :---  |:-----------------------:|:------------------------------------------------------------------------------------------------------------------------------------|:--------------------:|
| 1.    | [BrandAndProperNames.csv](#brand-and-proper-names) | Brand names (reserved), proper names (reserved), used in everyday life.                                                             | ~100 | 
| 2.      | [BuildingBlocks.csv](#building-blocks) | Building blocks from specific template file of Microsoft Word | 37 |
| 2.    | [dSAT.csv](#dsat) | Text replacements valid for Diagnostic and Monitoring Technologies for Rolling Stock. | ~100 |
| 2.    | FirstAndSecondNames.csv | Collections of abbreviated first and second names of my colleagues, sometimes also other personal data like phone numbers, e-mails. | 49 |

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
| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           joomla            | → |           *           | → |  Joomla{!}¦https://www.joomla.org/ |       MSI       |
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
| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           @copyrights            | → |           *           | → |  Copyrights{F3} |       SI       |

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

## Where libraries are stored?

As it was already mentioned, the library file can caontain fragile / protected in law data. Therefore such files should be protected against public access. The basic way to accomplish this task is to store library files within <UserData>: 
[Back to the top](#back-to-the-top)
<br />
<br />
<br />

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