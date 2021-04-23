## Rework of the german translation for SheetCam

The po-files can be edited for example with:
- Poedit
- Lokalize (Linux)
- Gtranslator (Linux)

To use it with SheetCam they have to be converted in the mo-format, either with Poedit or with [msgfmt](https://www.gnu.org/software/gettext/manual/html_node/msgfmt-Invocation.html):
```
msgfmt messages.po -o messages.mo
```

Updating from the reference-file (*.pot) can be done with Poedit or with [msgmerge](https://www.gnu.org/software/gettext/manual/html_node/msgmerge-Invocation.html):
```
msgmerge --no-fuzzy-matching -U messages.po messages.pot
```

