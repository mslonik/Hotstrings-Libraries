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

## The free Library files

| no.  |              **library name**              | **library description**                                                                               |                                    **remarks**                                     |
| :--- |:------------------------------------------|:------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------:|
| 1. |  (Unicode Sender) Orthographic Sender.csv  | Helps type orthographic characters not found on the keyboard.                                         |                                  ~171 definitions                                  |
| 2. |   (Unicode Sender) Currency Symbols.csv    | Helps type the symbols of world currencies.                                                           |                                   61 definitions                                   |
| 3. | (Unicode Sender) Computer-Keys Symbols.csv | Helps type computer-keys symbols.                                                                     |                                   28 definitions                                   |
|    | AbbreviationsEnglish.csv                   | Acronyms / abbreviations typical for English language.                                                | ~500 definitions                                                                   |
| 4. |           AccentsDiacritics.csv            | So called diacritics or accented letters not present in English.                                      |                                  ~25 definitions                                   |
| 5. | AutocompleteBrackets.csv                   | Adds closing bracket and shifts cursor in between the brackets.                                       |   5 definitions                                                                    |
| 6. |        AutoCorrectionHotstrings.csv        | Automatic corrections of mispelled words and couple more abbreviations.                               |                                  ~25 definitions                                   |
| 7. |             CapitalLetters.csv             | Auto-capitalization of first letter in the first word like week days, month days, geographical names. |                                  ~80 definitions                                   |
| 8. |             CircledNumbers.csv             | Unicode characters: numbers inside of circles.                                                        |                                   46 definitions                                   |
| 9. |     DevanagariTyperHelper_VowelSet.csv     | (...)                                                                                                 |                   23 definitions. Protects against mispellings.                    |
| 10. |            DiacriticPolish.csv             | Diacritic (accented) letters for Polish language.                                                     | 36 definitions. For the same purpose there is dedicated tool called Diacritics.ahk |
| 11. |            EmojiHotstrings.csv             | Unicode characters called emojis.                                                                     |                                  ~75 definitions                                   |
| 12. |              FirstCapital.csv              | Auto-capitalization of the first letter in the first word of each new sentence.                       |                 100 definitions. Based on idea from this article.                  |
| 13. |              FunctionKeys.csv              | Option to call function keys (or F keys): F1 ... F24 just by typing ordinary letters.                 |                                   25 definitions                                   |
| 14. |      GurmukhiTyperHelper_VowelSet.csv      | (...)                                                                                                 |                    9 definitions. Protects against mispellings.                    |
| 15. |               Incoterms.csv                | Abbreviations and full definitions of Incoterms.                                                      |                             24 definitions. Incoterms                              |
| 16. |           PhysicsHotstrings.csv            | Various unicode symbols more or less related to physics.                                              |                                  ~55 definitions                                   |
| 17. |               TimeHotstrings               | Definitions of time formats.                                                                          |                                   3 definitions                                    |

<br />
<br />
<br />

---


### AbbreviationsEnglish.csv ###

Acronyms (fitting into cathegory of abbreviations) can be used in up to 3x forms:
- short version, e.g. **ADC**,
- expanded version, e.g. **Analog to Digital Converter**,
- full version, explaining definition of acronym: 

Thanks to **Hotstrings** application all three forms can be easily applied.

Example:

| triggerstring + trigger | → | (triggerstring) options | → |                                                                                                hotstring                                                                                                | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------:|
|           adc           | → |            C            | → |                                                                                                   ADC                                                                                                   |       SI        |
|          adc/           | → |            *            | → | Analog to Digital Converter¦analog-to-digital converter is a system that converts an analog signal, such as a sound picked up by a microphone or light entering a digital camera, into a digital signal |       MSI       |

**Remarks:** 

1. Convention. For my libraries I use the following convention: 
   - If I want to immediately trigger a triggerstring, I use one of the characters freely available keys of keyboard, but seldomly used for other purposes. There are coupe of candidates: "~", "/", "\". I decided to use "/" as it is relatively easy reachable.
   - According to my style of writing, a short version of acronym is usually present at the end of a sentence. To trigger automatic text replacement it is enough to press one of usual triggers just after short version (e.g. adc and space, dot (.), colon (,) etc.). This way I don't have to enter any of acronym letters as capitals - they are converted to capitals by AutoHotkey automatically. It speeds up writing enormously on longer run. Additionally I use option "C": in case I'd enter abbreviation in capital letters (following above example: ADC), then AutoHotkey is not used to convert it between small letters and capital letters, what spares some time of microprocessor 😉.
   - Additionally for reference purposes for some definitions I use comment field (part of hotstring definition) for storage of link to definition (e.g. from Wikipedia).

1. Unification of language / culture.
   - If many people use the same set of abbreviations and definitions in written form, it builds at customers confidence and understanding. The same terms, the same definitions brings together and reduces area for misunderstanding. You can use **Hotstrings** aplication as basic aid for understanding.
   - You can use the same principle for definitions and names of your products in your company. For example all people in e-mail correspondence will use the same, unified definitions, no matter if it is technical documentation, datasheet or just a marketing leaflet.

1. Sometimes acronym names are the same as entire word. Good example in English is word "can". There is also acronym CAN which can stand for "Controller Area Network". It can be sometimes confusing when it is triggered automatically in unwanted situation. The fallback scenario is to undo last hotstring by pressing shortcut key combination dedicated to Hotstring application and that purpose (by default Win + Z). But if it is still unconvenient, you can define another triggerstring. For this particular acronym I use can\<Tab>, what is denoted as "can\`t", where "\`t" stands for \<Tab> or tabulator key.

<br />
<br />
<br />

---
### AccentsDiacritics.csv ###

[Accents or Diacritics](https://en.wikipedia.org/wiki/Diacritic) is a glyph added to a letter. Sometimes it is useful to enter one accented character without a need to temporarily switch keyboard layout or code page. For example correct spelling of French originated term "a la" is "à la" with accented "à".

Example:

| triggerstring + trigger | → | (triggerstring) options | → |   hotstring   | output function |
|:-----------------------:|:-:|:-----------------------:|:-:|:-------------:|:---------------:|
|           a^            | → |           C*?           | → | å¦ä¦â¦à¦á¦ą¦ā |       MSI       |

Meaning of options:
- "?" this definition can be called even from within any word.
- "C" it is case sensitive (only ordinary letter "a" and caret ^ will produce corresponding hotstring).
- "*" the trigger is a part of triggerstring (trigger = "^").
After triggerstring + trigger is pressed, user can choose from the list of 7x diacritics one fitting to the current purpose.

<br />
<br />
<br />

---
### AutocompleteBrackets.csv ###

Usually brackets come in pairs, e.g. after the opening ordinary bracket "(" comes the closing one ")". Definitions within this library automatically add closing bracket and also shifts cursor position in between pair of brackets in order to enable typing.

Example:

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
### AutoCorrect.csv  ###

<br />
<br />
<br />

---
## Not-free libraries ##

In this section I show examples of other libraries which I use in my everyday life but which cannot be shared by various reasons (GDPR, licence constraints, proprietary names etc.).

|    **library name**     | **library description**                                                                                                             |     **remarks**      |
|:-----------------------:|:------------------------------------------------------------------------------------------------------------------------------------|:--------------------:|
| FirstAndSecondNames.csv | Collections of abbreviated first and second names of my colleagues, sometimes also other personal data like phone numbers, e-mails. | GDPR protected data. |

## Where libraries are stored? ##

As it was already mentioned, the library file can caontain fragile / protected in law data. Therefore such files should be protected against public access. The basic way to accomplish this task is to store library files within <UserData>: 
