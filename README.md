This is a port of the Wox plugin [WoxDictionary](https://github.com/harrynull/WoxDictionary) created by Harry (@harrynull). 

This is a fork of [harrynull's Flow.Launcher.Dictionary](https://github.com/harrynull/Flow.Launcher.Dictionary) with the intention of having less Chinese bits. Not that there is anything wrong with it, but, it feels superfluous and jolting when looking for English terms to have mostly-Pinyin labelled results.

This port is intended to be used for [Flow Launcher](https://github.com/Flow-Launcher/Flow.Launcher). It will not work for Wox.

To use this plugin:

From Flow Launcher, type `pm install dictionaryEn`

Changes contained in this port (by harrynull):

- Upgraded to .Net Core 3.1
- Changed Wox's plugin library to Flow's plugin library
- Removed System.Speech.Synthesis which is not supported in .Net Core https://github.com/dotnet/runtime/issues/30991


----------------------------------
# WoxDictionary
![Demonstration](Images/demo.gif)

Features

* Phonetic

  ![Phonetic](Images/demo/phonetic.png)

* Definitions

  Add `!d` at the end of the word to trigger.

  ![Definition](Images/demo/definition.png)

* Synonym

  Add `!s` at the end of the word to trigger.

  ![Synonym](Images/demo/synonym.png)

* Exchanges

  Add `!e` at the end of the word to trigger.

  ![Exchanges](Images/demo/exchanges.png)

* Spelling correction

  ![Spelling correction](Images/demo/spelling_correction.png)

* Word copy

  Pressing Alt+Enter can copy the word.

* Pronunciation

  `Ctrl+Enter` can read the selected word. (#TODO is this pronunciation for Mandarin or English?)

* Search Words

  Select any results in the `!` mode can jump to the configured website.


## Compilation

1. Visual Studio - Compile it using Visual Studio.
2. `generate_dist.bat` - Pack it using `generate_dist.bat`

## Installation

### 

1. You need to have [Wox](https://github.com/Wox-launcher/Wox) installed first.

2. (Manual Installation) Copy dist folder to `C:\Users\\{User Name}\AppData\Local\Wox\app-{Version Number}\Plugins\`

   (WPM) Wox `wpm install Dictionary`

   (Wox Plugin Manager) Type `wpm install Dictionary` in your Wox.

3. **Download, uncompress and copy [ecdict.db](https://github.com/harrynull/WoxDictionary/releases/tag/dict) to `C:\Users\{your_user_name}\AppData\Roaming\Wox\Plugins\Dictionary-{random_characters}\dicts`.**

4. API tokens - Open settings and configure API tokens.


## Acknowledgments

这个项目没有以下伟大项目的帮助是不可能完成的：

The project won't be possible without the help of the following great projects:

* [Wox](https://github.com/Wox-launcher/Wox) Launcher for Windows, an alternative to Alfred and Launchy.
* [SymSpell](https://github.com/wolfgarbe/SymSpell) 1 million times faster through Symmetric Delete spelling correction algorithm. By Wolf Garbe.
* [Big Huge Thesaurus](https://words.bighugelabs.com/api.php) A very simple API for retrieving the synonyms for any word.
* [Flow.Launcher.Dictionary](https://github.com/harrynull/Flow.Launcher.Dictionary) the original English-Chinese dictionary for Flow, by [harrynull](https://github.com/harrynull)

## License

I _*think*_ this project is released under LGPL 3.0 License...

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.
    
    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.
    
    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
