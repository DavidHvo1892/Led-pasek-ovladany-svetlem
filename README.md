# 🌙 Soumrakový spínač pro LED pásek (12V)

Tento projekt představuje automatický **soumrakový spínač**, který ovládá LED osvětlení na základě okolních světelných podmínek. Hlavním cílem bylo vytvořit bezkontaktní, spolehlivý a energeticky efektivní systém regulace pro domácí využití.

## 📋 Hlavní vlastnosti
* **Bezkontaktní spínání:** Žádné mechanické části, automatický provoz.
* **Vysoký výkon:** Použitý MOSFET tranzistor zvládne proud až 30 A.
* **Nastavitelná citlivost:** Možnost přesného nastavení prahu sepnutí pomocí trimru.
* **Bezpečnost:** Provoz na bezpečném napětí 12 V DC.

## 🛠 Seznam součástek
| Součástka | Specifikace | Funkce |
| :--- | :--- | :--- |
| **Napájecí adaptér** | 12 V / 1 A | Zdroj energie pro systém |
| **DC konektor** | Samice 5,5/2,1 mm | Vstup pro napájecí adaptér |
| **Tranzistor** | N-MOSFET FQP30N06 | Výkonový spínač (spíná záporný pól) |
| **Senzor** | Fotorezistor GL5539 | Detekce intenzity světla |
| **Trimr** | 100 kΩ lineární | Nastavení citlivosti (úrovně šera) |
| **Rezistor** | 1 kΩ | Ochrana hradla (Gate) tranzistoru |
| **LED pásek** | 12 V DC | Světelný výstup |
| **Prototypování** | Nepájivé pole + vodiče | Propojení bez pájení |

## ⚙️ Technický princip
Systém pracuje na principu **napěťového děliče**. Ten je tvořen fotorezistorem (LDR) a trimrem.

1.  **Detekce šera:** Při poklesu intenzity světla se zvýší odpor fotorezistoru.
2.  **Dělič napětí:** Zvýšení odporu způsobí nárůst napětí na hradle (**Gate**) MOSFET tranzistoru.
3.  **Sepnutí:** Jakmile napětí na hradle překročí prahovou hodnotu, tranzistor se otevře a propojí záporný pól LED pásku se zemí (GND).
4.  **Výstup:** LED pásek se rozsvítí.



## 🚀 Příklady použití
* **Osvětlení schodiště:** Automatické zapnutí při setmění pro vyšší bezpečnost.
* **Terasa/Zahrada:** Dekorativní osvětlení, které se samo zapne večer.
* **Noční světlo:** Orientační osvětlení chodby s minimální spotřebou ve dne.

## 📸 Schéma zapojení
