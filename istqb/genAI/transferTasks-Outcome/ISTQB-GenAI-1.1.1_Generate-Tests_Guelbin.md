# TRATAS – GenAI Testfall-Generator: Warenkorb & Checkout

## Ziel
Verwenden Sie generative KI, um wertvolle und wiederverwendbare Testfälle für die Warenkorb- und Checkout-Funktionalität des ToolShop-Systems zu erstellen und die Ergebnisse kritisch zu bewerten.

---

## Kontext (System Under Test)
- ToolShop E-Commerce Plattform: https://practicesoftwaretesting.com/
- Fokusbereiche:
  - Warenkorb (Hinzufügen, Aktualisieren, Entfernen von Artikeln)
  - Checkout (Benutzerfluss, Zahlung, Validierung)

---

## Aufgabe (≤ 30 Minuten)

### Teil 1 – Verständnis der Testbasis (5 Min)
1. Öffnen Sie die ToolShop-Anwendung
2. Führen Sie die folgenden Aktionen aus:
   - Fügen Sie ein Produkt zum Warenkorb hinzu
   - Navigieren Sie zum Checkout

**Dokumentieren Sie:**
- 2–3 zentrale Schritte des Benutzerflusses

1. Ein Produkt wird zum Warenkorb hinzugefügt und der Warenkorb geöffnet.
2. Über die Schaltfläche „Zur Kasse“ erfolgt die Navigation zum Checkout bzw. zur Login-Seite.
3. Der Checkout-Prozess wird mit der Zahlungsmethode „Kaufe jetzt, zahle später“ mit 3 monatlichen Raten erfolgreich abgeschlossen.

---

### Teil 2 – Erstellen eines Prompts (5 Min)

Verwenden Sie den folgenden strukturierten Prompt:

<Definieren Sie den Prompt – der Testfall-Titel sollte die Syntax T1T5 haben>

* ### ERSTE PROMPT-VERSION: 
Du bist Software-Tester.

Die Testfälle sollen auf der ToolShop-Anwendung basieren:
https://practicesoftwaretesting.com/

Erstelle realistische und detaillierte Testfälle für den Warenkorb- und Checkout-Flow.

Verwende für die Testfall-Titel die T1T5-Syntax:

- T1 = Standard Case (Happy Path)
- T2 = Alternative Case
- T3 = Exception Case
- T4 = Negative Case
- T5 = Misuse Case

Verwende folgende Namenssyntax:

#### `<Tx>_<Feature>_<BusinessRule>_<ExpectedResult>`

Beispiel:
T1_Checkout_PaymentWithCreditCard_OrderCompletedSuccessfully

Für jeden Testfall sollen folgende Informationen enthalten sein:
- Vorbedingungen
- Testschritte
- Erwartetes Ergebnis

Die Testfälle sollen realistisch für die ToolShop-Anwendung sein und typische Benutzer- sowie Fehlerszenarien abdecken.

#### ERSTE ERGEBNISSE:
Die erste Prompt-Version erzeugte bereits realistische Testfälle für den Warenkorb- und Checkout-Prozess. 
* ### Beispiel:
Warenkorb & Checkout Testfälle
T1_Cart_AddAvailableProduct_ProductDisplayedInCart

Vorbedingungen: Benutzer ist auf der Produktübersicht. Ein Produkt ist verfügbar.
Testschritte: Produkt öffnen → „Add to cart“ klicken → Warenkorb öffnen.
Erwartetes Ergebnis: Produkt wird mit Name, Preis, Menge 1 und Zwischensumme im Warenkorb angezeigt.

T1_Cart_UpdateQuantity_TotalPriceRecalculatedCorrectly

Vorbedingungen: Ein Produkt befindet sich im Warenkorb.
Testschritte: Menge von 1 auf 2 erhöhen.
Erwartetes Ergebnis: Menge wird aktualisiert, Zwischensumme und Gesamtsumme werden korrekt neu berechnet.

* ### VERBESSERTE PROMT-VERSION:
Zusätzlich ergänzt:
Beispiel:
TC_101 – T1_Checkout_PaymentWithCreditCard_OrderCompletedSuccessfully
Für jeden Testfall sollen folgende Informationen enthalten sein:
- Test-ID
- Vorbedingungen
- Testschritte (nummeriert)
- Erwartetes Ergebnis
Die Testschritte sollen klar, strukturiert und realistisch für die ToolShop-Anwendung formuliert sein.
Die erwarteten Ergebnisse sollen präzise und überprüfbar formuliert werden.

#### ERGEBNISSE:
Durch die zusätzliche Strukturierung mit Test-ID, nummerierten Testschritten und präziseren Anforderungen wurden die Ergebnisse übersichtlicher und konsistenter.

* ### Beispiel:
TC_101 – T1_Cart_AddProductToCart_ProductAddedSuccessfully

Test-ID: TC_101

Vorbedingungen:
Benutzer befindet sich auf der Produktübersicht. Mindestens ein Produkt ist verfügbar.

Testschritte:

Ein verfügbares Produkt auswählen.
Auf der Produktdetailseite auf Add to cart klicken.
Den Warenkorb öffnen.

Erwartetes Ergebnis:
Das ausgewählte Produkt wird im Warenkorb mit korrektem Produktnamen, Preis, Menge 1 und Zwischensumme angezeigt.

---

### Teil 3 – Generieren von Testfällen (10 Min)
1. Führen Sie den Prompt mit einem generativen KI-Tool aus (z. B. ChatGPT)
2. Überprüfen Sie die Ausgabe
3. Wählen Sie mindestens 5 nützliche Testfälle aus




---

### Teil 4 – Bewertung der Qualität (10 Min)

Bewerten Sie die generierten Testfälle:

- Sind sie realistisch für ToolShop?
- Fehlen wichtige Szenarien?
- Sind einige Testfälle zu allgemein?


**Obwohl die Aufgabe ursprünglich nicht den Vergleich mehrerer KI-Modelle vorsah, habe ich zusätzlich Gemini AI verwendet, um die Ergebnisse zu vergleichen und Unterschiede in der Qualität der generierten Testfälle zu analysieren.**

**Die mit ChatGPT generierten Testfälle wirken realistisch und gut an den ToolShop-Checkout- und Warenkorbprozess angepasst. Die Testschritte sind klar strukturiert und die erwarteten Ergebnisse präzise formuliert.**

**Auch die mit Gemini AI erstellten Testfälle wirken grundsätzlich realistisch. Allerdings sind sie teilweise allgemeiner formuliert und enthalten bei den erwarteten Ergebnissen mehrere mögliche Varianten oder Formulierungen. Dadurch wirken die Testfälle ausführlicher, aber teilweise auch weniger präzise und stärker spekulativ.**

**Insgesamt eignen sich beide KI-Systeme gut zur schnellen Erstellung von Testfällen. Die Ergebnisse sollten jedoch immer manuell überprüft und an die tatsächliche Anwendung angepasst werden.**




Verbessern Sie das Ergebnis:
- Fügen Sie mindestens 2 fehlende Testfälle hinzu, die von der KI nicht generiert wurden

    **Die generierten Testfälle decken bereits viele wichtige Szenarien des Warenkorb- und Checkout-Prozesses ab. Daher konnten keine gravierenden fehlenden Testfälle identifiziert werden.**

---

## Erwartetes Ergebnis / Team-Mehrwert

- Erste Sammlung von KI-generierten Testfällen für Warenkorb & Checkout
- Identifikation von:
  - Lücken in den KI-generierten Tests
  - Typischen Schwächen generativer KI
- Grundlage für:
  - Regressionstests
  - Testautomatisierung

---

## Akzeptanzkriterien

- Der Warenkorb- und Checkout-Flow wurde manuell untersucht
- Ein strukturierter Prompt wurde erstellt und ausgeführt
- Mindestens 5 generierte Testfälle wurden ausgewählt
- Die Testfälle enthalten:
  - Vorbedingungen
  - Testschritte
  - Erwartete Ergebnisse
- Eine kritische Bewertung der KI-Ausgabe wurde durchgeführt
- Mindestens 2 zusätzliche Testfälle wurden manuell ergänzt
- Die Ergebnisse sind dokumentiert und wurden mit dem Team geteilt (z. B. Testmanagement-Tool, Confluence)