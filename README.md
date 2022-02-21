# Hotstrings-Libraries

Hotstring library is text file (*.csv) formatted to work with [*Hotstrings*](https://github.com/mslonik/Hotstrings) application, which is text replacement tool.

In this article there are described libraries belonging to the following cathegories:

1. Free library files.
1. Not-free library files

Text replacement format:

| text to be replaced | →     | replacement options | →     | replaced text |
| :---:               | :---: | :---:               | :---: | :---:         |
| triggerstring + trigger | → | (triggerstring) options | → | hotstring |

## The free Library files

| **library name** | **library description** | **remarks**|
| :---:            | :---                   | :---:      |
| Abbreviations.csv | Technical abbreviations (mainly acronyms). | ~480 definitions  |
| AccentsDiacritics.csv | So called diacritics or accented letters not present in English. | ~25 definitions |
| AutoCorrectionHotstrings.csv | Automatic corrections of mispelled words and couple more abbreviations. | ~25 definitions |
| CapitalLetters.csv | Auto-capitalization of first letter in the first word like week days, month days, geographical names.  | ~80 definitions |
| CircledNumbers.csv | Unicode characters: numbers inside of circles. | 46 definitions |
| DevanagariTyperHelper_VowelSet.csv | (...) | 23 definitions. Protects against mispellings. |
| DiacriticPolish.csv | Diacritic (accented) letters for Polish language. | 36 definitions. For the same purpose there is dedicated tool called Diacritics.ahk |
| EmojiHotstrings.csv | Unicode characters called emojis. | ~75 definitions |
| FirstCapital.csv | Auto-capitalization of the first letter in the first word of each new sentence. | 100 definitions. Based on idea from this article. |
| FunctionKeys.csv | Option to call function keys (or F keys): F1 ... F24 just by typing ordinary letters. | 25 definitions |
| GurmukhiTyperHelper_VowelSet.csv | (...) | 9 definitions. Protects against mispellings. |
| Incoterms.csv | Abbreviations and full definitions of Incoterms. | 24 definitions.
Incoterms |
| PhysicsHotstrings.csv | Various unicode symbols more or less related to physics. | ~55 definitions |
| TimeHotstrings | Definitions of time formats. | 3 definitions |

### Abbreviations.csv ###

Examples:

## Not-free libraries ##

In this section I show examples of other libraries which I use in my everyday life but which cannot be shared by various reasons (GDPR, licence constraints, proprietary names etc.).

| **library name** | **library description** | **remarks**|
| :---:            | :---                   | :---:      |
| FirstAndSecondNames.csv | Collections of abbreviated first and second names of my colleagues, sometimes also other personal data like phone numbers, e-mails. | GDPR protected data. |

## Where libraries are stored? ##

As it was already mentioned, the library file can caontain fragile / protected in law data. Therefore such files should be protected against public access. The basic way to accomplish this task is to store library files within <UserData>: 