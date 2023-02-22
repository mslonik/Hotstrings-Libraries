# Hotstrings-Libraries

Hotstring library is text file (*.csv) formatted to work with [*Hotstrings*](https://github.com/mslonik/Hotstrings) application, which is text replacement tool.

In this article there are described libraries belonging to the following cathegories:

1. Free library files.
1. Not-free library files

Text replacement format and naming convention:

|   text to be replaced   | → |   replacement options   | → | replaced text |      output function      |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:-------------------------:|
| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | how hotstring is produced |


<br />
<br />
<br />

## **The free Library files**

| no.  |              **library name**              | **library description**                                                                               |                                    no. of definitions within library                                      |
| :--- |:------------------------------------------|:------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------:|
| 1. |  (Unicode Sender) Orthographic Sender.csv  | Helps type orthographic characters not found on the keyboard.                                         |                                  ~171                                   |
| 2. |   (Unicode Sender) Currency Symbols.csv    | Helps type the symbols of world currencies.                                                           |                                   61                                    |
| 3. | (Unicode Sender) Computer-Keys Symbols.csv | Helps type computer-keys symbols.                                                                     |                                   28                                    |
|    | AbbreviationsEnglish.csv                   | Acronyms / abbreviations typical for English language.                                                | ~550                                                                    |
| 5. | AutocompleteBrackets.csv                   | Adds closing bracket and shifts cursor in between the brackets.                                       |   5                                                                     |
|    | AutoCorrect.csv                            | Hotstrings to correct common English misspellings on-the-fly.                                         |   4841                                                                  |                    
| 6. |        AutoCorrectionHotstrings.csv        | Automatic corrections of mispelled words and couple more abbreviations.                               |                                  18                                    |
|    | BoxDrawing.csv                             | ASCII box drawing characters.                                                                         | 8 
| 7. |             CapitalLetters.csv             | Auto-capitalization of first letter in the first word like week days, month days, geographical names. |                                  ~80                                    |
| 8. |             CircledNumbers.csv             | Unicode characters: numbers inside of circles.                                                        |                                   46                                    |
| 9. |     DevanagariTyperHelper_VowelSet.csv     | (...)                                                                                                 |                   23                      |
|    |           DiacriticsHotstrings.csv          | So called diacritics or accented letters not present in English.                                      |                                  ~25                                    |
| 10. |            DiacriticPolish.csv             | Diacritic (accented) letters for Polish language.                                                     | 36  |
| 11. |            EmojiHotstrings.csv             | Unicode characters called emojis.                                                                     |                                  ~75                                    |
| 12. |              FirstCapital.csv              | Auto-capitalization of the first letter in the first word of each new sentence.                       |                 100                   |
| 13. |              FunctionKeys.csv              | Option to call function keys (or F keys): F1 ... F24 just by typing ordinary letters.                 |                                   25                                    |
| 14. |      GurmukhiTyperHelper_VowelSet.csv      | (...)                                                                                                 |                    9                      |
| 15. |               Incoterms.csv                | Abbreviations and full definitions of Incoterms.                                                      |                             24                                |
| 16. |           PhysicsHotstrings.csv            | Various unicode symbols more or less related to physics.                                              |                                  ~55                                    |
| 17. |               TimeHotstrings               | Definitions of time formats.                                                                          |                                   3                                     |

Remarks:
1. Only single definitions are counted. It means that if compound definition is present, then it is counted as one.

<br />
<br />
<br />

## **The not-free libraries**

In this section I show examples of other libraries which I use in my everyday life but which cannot be shared by various reasons (GDPR, licence constraints, proprietary names etc.).

| no.   |   library name     | library description                                                                                                             |     no. of definitions      |
| :---  |:-----------------------:|:------------------------------------------------------------------------------------------------------------------------------------|:--------------------:|
| 1.    | FirstAndSecondNames.csv | Collections of abbreviated first and second names of my colleagues, sometimes also other personal data like phone numbers, e-mails. | 49 |
| 2.    | BrandAndProperNames.csv | Brand names (reserved), proper names (reserved), used in everyday life.                                                             | ~100 | 

Remarks:
1. Only single definitions are counted. It means that if compound definition is present, then it is counted as one.

<br />
<br />
<br />

---


### AbbreviationsEnglish.csv

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

<br />
<br />
<br />

---
### **AutocompleteBrackets.csv**

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

<br />
<br />
<br />

---
### **AutoCorrect.csv**

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

<br />
<br />
<br />

---
### **AutocorrectionHotstrings.csv**

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Maciej Słojewski (🐘)

**Purpose**:   Content of this library is based on the concept of *AutoCorrect* library. It contains definitions which I wanted to have in separate, smaller library file, which are somewhat specific to my usage.

**Example**:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|   molkky               | → |           *             | → | mölkky      |       SI        |

Comment: name of Finnish coutry game. Origin written form contains diacritic character ö.
<br />
<br />
<br />

---
### **BoxDrawing.csv**

**License**:		CC BY-SA Creative Commons Attribution-ShareAlike

**Author**:		Maciej Słojewski (🐘)

**Purpose**:   ASCII box drawing characters. Based on: https://en.wikipedia.org/wiki/Box-drawing_character
Thanks to this library it is relatively easier to prepare ASCII only based block diagrams. Definitiots could be combined with ASCII box drawing online editors (e.g. https://textik.com/). Macros exchanging characters could be prepared e.g. in Notepad++.


**Example**:

*boxes1*/ converts into
```
╒═╤╕
│ ││
╞═╪╡
╘═╧╛
```
<br />
<br />
<br />

---

### **DiacriticsHotstrings.csv**

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

<br />
<br />
<br />

---
## Where libraries are stored? ##

As it was already mentioned, the library file can caontain fragile / protected in law data. Therefore such files should be protected against public access. The basic way to accomplish this task is to store library files within <UserData>: 
