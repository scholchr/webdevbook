# Schlüsselbegriffe

## Abschreibung (AfA)

Die Absetzung für Abnutzung (AfA) beschreibt die technische oder wirtschaftliche Wertminderung von Wirtschaftsgütern.

### lineare Abschreibungsmethode (lineare AfA)

Bei der linearen Abschreibungsmethode (lineare AfA) werden die geleisteten Anschaffungs- und Herstellungskosten (AHK) des abnutzbaren Anlagevermögens gleichmäßig auf die Nutzungsdauer (steuerliche bzw. kalkulatorische) verteilt.

Die steuerliche und wirtschaftliche Nutzungsdauer können differieren.

Die lineare Abschreibung (LAfA) in einem Jahr $t$ und der Restbuchwert ($RBW_t$ - nach Abschreibung) am Ende des Jahres $t$ sind also:

$LAfA =  \frac{AHK}{n}$

$RBW_t = \frac{n - t}{n} \cdot AHK$

### degressive Abschreibungsmethode

Bei der **degressiven Abschreibungsmethode** (degressive AfA) handelt es sich um eine Abschreibung mit fallenden Jahresbeträgen. Es werden dabei immer niedrigere Teile der Anschaffungskosten auf die Jahre der Nutzung verteilt werden.

Da die Abschreibung ein konstanter Bruchteil des sinkenden Restbuchwerts ist, sinkt sie im Zeitablauf. Dies führt dazu, dass der Restbuchwert nie "Null" werden kann. Aus diesem Grunde ist es steuerlich gestattet und handelsrechtlich zur Vermeidung von Überbewertungen notwendig, nach einer gewissen Abschreibungsdauer auf die lineare Abschreibung zu wechseln.

### degressive / lineare Abschreibungsmethode

Bei der degressiven / linearen Abschreibungsmethode wird in den ersten Jahren der Nutzungsdauer degressiv abgeschrieben und später auf die lineare Abschreibungsmethode (mit steuerlicher Nutzungsdauer) umgestellt. Dies geschieht im Programm automatisch, wenn die linearen Abschreibungsbeträge höher sind als die degressiven Abschreibungsbeträge.


### Abschreibungsmethode - Beispiel

* Steuerliche Nutzungsdauer	= 10 Jahre
* Degressive AfA = 30 %
* Anschaffungskosten = 1.000 EUR

|    Zeitachse    |   1   |   2   |   3   |   4   |   5   |   6   |   7   |   8   |   9   |   10  |
| --------------- | ----: | ----: | ----: | ----: | ----: | ----: | ----: | ----: | ----: | ----: |
| AfA linear      |   100 |   100 |   100 |   100 |   100 |   100 |   100 |   100 |   100 |   100 |
| Restbuchwert    |   900 |   800 |   700 |   600 |   500 |   400 |   300 |   200 |   100 |     0 |
|                 |       |       |       |       |       |       |       |       |       |       |
| AfA degressiv   |   300 |   210 |   147 |   103 |    72 |    50 |    36 |  *25**|    17 |    12 |
| Restbuchwert    |   700 |   490 |   343 |   240 |   168 |   118 |    82 |    57 |    40 |    28 |
|                 |       |       |       |       |       |       |       |       |       |       |
| AfA degr./lin.  |   300 |   210 |   147 |   103 |    72 |    50 |    36 |  *27**|    28 |    27 |
| Restbuchwert    |   700 |   490 |   343 |   240 |   168 |   118 |    82 |    55 |    27 |     0 |

\* hier wird auf linear gewechselt

$82 \cdot 0,30 = 24,6$

$\frac{82}{3} = 27,3$

### Abschreibungstypen

Hier können Sie entscheiden, wie die Abschreibungen nachträglicher Investitionen behandelt werden sollen:

* **Nachgeholt** - Die Abschreibung wird im Jahr des Anfalls der Kosten nachgeholt.
* **Restnutzung** - Die Abschreibungen werden auf die Restnutzungsdauer der Erstinvestition verteilt.
* **Laufzeit** - Die Kosten werden, vom Jahr des Anfalls an, erneut über die komplette Laufzeit abgeschrieben. Die Ausgabe des jeweiligen Jahres wird als selbständiges Wirtschaftsgut betrachtet.


Der Abschreibungsmonat der Re-Investition ergibt sich aus:

*	Dem gesetzten Häkchen in der Maske Projektinformation im Feld AfA-Beginn wie im ersten Jahr und dem Eintrag in der Maske Investition im Feld AfA-Beginn. In diesem Fall wird der Monat angenommen, der im Feld AfA-Beginn eingetragen ist.
*	Dem nicht gesetzten Häkchen in der Maske Projektinformation Feld AfA-Beginn wie im ersten Jahr. In diesem Fall wird der Monat Januar als AfA-Beginn gesetzt.

**Beispiel:**

* Abschreibungsbeginn: 01.01.2003
* Abschreibung linear:	20%

|  Zeitachse  |	2002 | 2003 |	2004 | 2005 | 2006 | 2007 | 2008 | 2009 |
| ---------   | ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| Investition |  100 |      |      |   50 |      |      |      |      |
| Nachgeholt  |      |   20 |   20 |   50 |   30 |   30 |      |      |
| Restnutzung	|      |   20 |   20 |   37 |   36 |   37 |      |      |
| Laufzeit 	  |   20 |   20 |   30 |   30 |   30 |   10 |   10 |      |

### außerplanmäßige Abschreibung (Sonderabschreibung)

Nach **§ 253 Abs. 2 Satz 3 HGB** können bei Vermögensgegenständen (VG) des Anlagevermögens (AV) außerplanmäßige Abschreibungen vorgenommen werden, um die VG mit dem niedrigeren Wert anzusetzen, der am Stichtag beizulegen ist. Sie sind vorzunehmen bei einer voraussichtlich dauernden Wertminderung.

Nach **§ 253 Abs. 3 HGB** müssen die VG des Umlaufvermögens (UV) auf einen niedrigeren Wert abgeschrieben werden. Dieser Wert ergibt sich aus dem Börsen- oder Marktpreis am Abschlussstichtag. Außerdem dürfen die Abschreibungen vorgenommen werden, die "nach vernünftiger kaufmännischer Beurteilung notwendig sind, um zu verhindern, dass in der nächsten Zukunft der Wertansatz dieser VG auf Grund von Wertschwankungen geändert werden muss".

Für Kapitalgesellschaften gilt außerdem **§ 279 Abs. 1 HGB**.

--8<-- "includes/glossar_iuf.md"