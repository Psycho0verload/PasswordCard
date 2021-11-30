Kennwort-Karte
============

Flexibler Kennwortkarten-Generator.

Werkzeug zum Generieren von Passwortkarten via NodeJS mit benutzerdefinierten Spalten-, Zeilen- und Zeichenlängen.


### Muster
String zur Definition der Struktur jedes Codes/jeder Zelle.

| Symbol | Beschreibung |
| ------ | ---------------------------------------------- |
| __a__ | Kleinbuchstaben des Ascii-Alphabets `[a-z]` |
| __A__ | Ascii-Zeichen in Großbuchstaben `[A-Z]|
| __1__ | numerische Zeichen `0123456789` |
| __!__ | Symbole `!?@#$%&()[]+-*/=<>_.,;"'` |
| __i__ | `[a-zA-Z]` |
| __n__ | `[0-9a-z]` |
| __N__ | `[0-9A-Z]` |
| __9__ | `[0-9a-zA-Z]` |
| __*__ | `[0-9a-zA-Z]` + Symbole |
| __#__ | wie `*`, aber dies durchläuft die Typen |
| __c__ | wie `#`, aber ohne `/="`|

_Beispiele:_

| Typ | Muster |
| --------------------- | ------- |
| Standard | `####` |
| Eins von jedem | `aA1!` |
| Nur Ziffern | `1111` |
| Nur Alpha-Zeichen | `aAaA` |

### Beispiel für eine Passwortkarte

#### Konsolenausgabe

Ausgabe des Beispiels `genPwdCardConsole.js`. Passphrase: `ThisIsMyCardCode`, Größe: 13x13, Muster: `aA1!`.

	qE7, hR6& jW0- uN9< rL2[ pA4% zS5" aV1_ kF8; fI3@ dC2] tG1* bM3'
	iO5> yP7? vY4= eB9! sX0( cD6# oK8/ lZ3$ mH8. nT4+ xQ2) wJ6; gU1'
	jN0] lI5) yH9[ iT7= zJ9- wZ7, sU2& fS6. mA0_ nF4! rQ5% tE3# eR8(
	pB1$ qC9< cD8+ gG2" hV4? dP0/ uY5@ vM7* bK1> oX6! xO3" aL2; kW1*
	uM0' fB7@ dX8/ hA9= iC6- wI5( zF4< sP3. qD1] rN0+ aS7) lW9? yQ3_
	gO6% jY4[ pL8& tU2, nH5$ cJ2> kZ0# vR1$ eG5# xV9@ oK7; bT6< mE3?
	cI4> zZ8" eR4_ mM7[ vJ0% xB8( tO2- nX6& fQ5/ hA1] gG9* rT3, wU9=
	kV8) lC2! aK3+ sH1' uY6. iW5@ yS7% bD0# jF4$ oL3, dP6_ pN0> qE8"
	oQ4) nX5! vG2] fB1[ rW7; qP9+ aJ5- mF9? iD4/ lC7* cH2. yY8( sO1'
	gK3< jZ6= xU0& kA4[ eE8= tL5- wS0% bR3" uN6$ hV1! dM2* pT7; zI9,
	nC6. lW4& xA3' tH2< uU8+ vG5# cJ7) dP0/ eI1( qK9_ zV3] aE4@ bQ5>
	kF9? rZ7< iO0' hS1* sD2% oT8[ gY6( fX7- mR2. pM6, yN3& wL5@ jB8)
	dW9; cC1] gJ0# vL4$ bI7> sT9_ uS4" rA2/ qY3= aO1! iP8+ zV5? pE0(
