# Programmiere einen simplen Computer.

*Quelle: http://adventofcode.com/day/23*

Der Computer hat zwei Register, Register a und Register b. Diese können jeden nicht-negativen Wert speichern. Beim Start sind beide Register mit 0 initialisiert.
Folgende Instruktionen beherrscht der Computer:

* `hlf r`: Halbiert den Wert in Register r und geht weiter zur nächsten Instruktion
* `tpl r`: Verdreifacht den Wert in Register r, geht dann weiter zur nächsten Instruktion
* `inc r`: Addiert 1 zum Wert in Register r, geht dann weiter zur nächsten Instruktion
* `jmp offset`: Springt um den Offset weiter (relativ zur Instruktion selbst)
* `jie r, offset`: Springt um den Offset weiter, wenn der Wert in Register r gerade ist ("jump if even")
* `jio r, offset`: Springt um den Offset weiter, wenn der Wert in Register r 1 ist ("jump if one")

Beispielcode:

    inc a
    jio a, +2
    tpl a
    inc a

Nach Ausführung enthält Register a den Wert 2.

Implementiere den Computer.


---

## Anhang

### Großes Programm:

	jio a, +19
	inc a
	tpl a
	inc a
	tpl a
	inc a
	tpl a
	tpl a
	inc a
	inc a
	tpl a
	tpl a
	inc a
	inc a
	tpl a
	inc a
	inc a
	tpl a
	jmp +23
	tpl a
	tpl a
	inc a
	inc a
	tpl a
	inc a
	inc a
	tpl a
	inc a
	tpl a
	inc a
	tpl a
	inc a
	tpl a
	inc a
	inc a
	tpl a
	inc a
	inc a
	tpl a
	tpl a
	inc a
	jio a, +8
	inc b
	jie a, +4
	tpl a
	inc a
	jmp +2
	hlf a
	jmp -7



