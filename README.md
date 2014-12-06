Create a booklet using pandoc and LibreOffice
=============================================

LibreOffice Advent Calendar 2014
: http://www.adventar.org/calendars/507

pandocとLibreOffice WriterでiDエディタのマニュアルを製本する
: http://www.nofuture.tv/diary/20141206.html

Files
-----

- LernOSM.html: iD Editor Manual
- reference.odt: Pandoc reference.odt (Original)
- reference-japanese.odt: Pandoc reference.odt (Japanese)
- pandoc-writer.md: text "Create a booklet using pandoc and LibreOffice"

Build
-----

iD Manual

    $ pandoc -f html -t odt --reference-odt=reference-japanese.odt -o idmanual.odt LearnOSM.html

text

    $ pandoc -f markdown -t odt --reference-odt=reference-japanese.odt -o pandoc-writer.odt pandoc-writer.md

License
-------

pandoc-writer.md: Creative Commons License [Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/deed.ja)
Other: Public Domain

