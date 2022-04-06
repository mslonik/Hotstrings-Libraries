# Hotstrings-Libraries

Hotstring library is text file (*.csv) formatted to work with [*Hotstrings*](https://github.com/mslonik/Hotstrings) application, which is text replacement tool.

In this article there are described libraries belonging to the following cathegories:

1. Free library files.
1. Not-free library files

Text replacement format:

| text to be replaced     | →     | replacement options     | →     | replaced text | output function |
| :---:                   | :---: | :---:                   | :---: | :---:         | :---: |
| triggerstring + trigger | →     | (triggerstring) options | →     | hotstring     | how hotstring is produced |

## The free Library files

| **library name** | **library description** | **remarks**|
| :---:            | :---                   | :---:      |
| (Unicode Sender) Orthographic Sender.csv | Helps type orthographic characters not found on the keyboard. | ~171 definitions  |
| (Unicode Sender) Currency Symbols.csv | Helps type the symbols of world currencies. | 61 definitions  |
| (Unicode Sender) Computer-Keys Symbols.csv | Helps type computer-keys symbols. | 28 definitions  |
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

Acronyms (fitting into cathegory of abbreviations) can be used in up to 3x forms:
- short version, e.g. **ADC**
- expanded version, e.g. **Analog to Digital Converter**
- full version, explaining definition of acronym: 

Thanks to **Hotstrings** application all three forms can be easily applied.

Example:

| triggerstring + trigger | →     | (triggerstring) options | →     | hotstring     | output function |
| :---:                   | :---: | :---:                   | :---: | :---:         | :---:           |
| adc                     | →     | C                       | →     | ADC           | SI              |
| adc/                    | →     | *                       | →     | Analog to Digital Converter¦analog-to-digital converter is a system that converts an analog signal, such as a sound picked up by a microphone or light entering a digital camera, into a digital signal | MSI                            |

**Remarks:** 

1. Convention. For my libraries I use the following convention: 
   - if I want to immediately trigger a phrase, I use one of the characters freely available keys of keyboard, but seldomly used for other purposes. There are coupe of candidates: "~", "/", "\". I decided to use "/" as it is relatively easy reachable;
   - short version of acronyms are usually present in a sentence, so to trigger such hotstring it is enough to press one of usual triggers (e.g. space, dot (.), colon (,) etc.). This way I don't have to enter the acronyms in capital letters - they are converted to capitals by AutoHotkey automatically. Additionally I use option "C": in case I'd enter abbreviation in capital letters (following above example: ADC), then AutoHotkey is not used to convert it between small letters and capital letters, what spares some time of microprocessor 😉;
   - additionally for reference purposes for some definitions I use comment field for storage of link to definitions.

1. Unification of language / culture.
   - If many people use the same set of abbreviations and definitions in written form, it builds at customers confidence and understanding. The same terms, the same definitions brings together and reduces area for misunderstanding. You can use **Hotstrings** aplication as basic aid for understanding.
   - You can use the same principle for definitions and names of your products in your company. For example all people in e-mail correspondence will use the same, unified definitions, no matter if it is technical documentation, datasheet or just a marketing leaflet.

1. Sometimes acronym names are the same as words used 

### AccentsDiacritics.csv  ###

Example:

| triggerstring + trigger | →     | (triggerstring) options | →     | hotstring     | output function |
| :---:                   | :---: | :---:                   | :---: | :---:         | :---:           |
| a^                      | →     | C*?                     | →     | å¦ä¦â¦à¦á¦ą¦ā | MSI             |

Thanks to the option:
- "?" this definition can be called even from within any word,
- "C" it is case sensitive (small letter a^ will produce corresponding hotstring),
- "*" the trigger is a part of triggerstring (trigger = "^").

After triggerstring + trigger is pressed, user can choose from the list of 7x diacritics one fitting to the current purpose.

## Not-free libraries ##

In this section I show examples of other libraries which I use in my everyday life but which cannot be shared by various reasons (GDPR, licence constraints, proprietary names etc.).

| **library name** | **library description** | **remarks**|
| :---:            | :---                   | :---:      |
| FirstAndSecondNames.csv | Collections of abbreviated first and second names of my colleagues, sometimes also other personal data like phone numbers, e-mails. | GDPR protected data. |

## Where libraries are stored? ##

As it was already mentioned, the library file can caontain fragile / protected in law data. Therefore such files should be protected against public access. The basic way to accomplish this task is to store library files within <UserData>: 
