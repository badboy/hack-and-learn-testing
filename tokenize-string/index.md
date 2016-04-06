# String Tokenizer

*Quelle: http://rosettacode.org/wiki/Tokenize_a_string_with_escaping*

String zerlegen anhand von Trennsymbolen und Escapezeichen.

Aufgabe

* Schreibe Tests für einfache Strings
* Schreibe Tests für den vollständigen String aus dem Link
* Implementiere eine Funktion, die den gegebenen String entsprechend der Zeichen trennt und als Vector die Teilstrings zurückgibt.

## Beispiel

**Input**

* String: `one^|uno||three^^^^|four^^^|^cuatro|`
* Separator: `|`
* Escape: `^`

**Output**

    ["one|uno", "", "three^^", "four^|cuatro", ""]
