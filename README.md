# Dungeon di Musci - 3D Raycasting School Parody 🏫🎮

Un videogioco sparatutto in prima persona con grafica pseudo-3D retro stile anni '90, sviluppato interamente in **Python** con la libreria **Pygame**. Il progetto è una parodia scolastica ironica creata come elaborato finale per il laboratorio di Informatica.

---

## 🎯 Obiettivo del Gioco

Il gioco è strutturato su **2 livelli complessivi**:

1. **Livello 1 (La Classe):** Il giocatore ha a disposizione **90 secondi** per trovare e sabotare i 2 computer del laboratorio scolastico premendo il tasto `F` (attivando il famigerato *Blue Screen of Death*). Nel frattempo, deve evitare o neutralizzare i minion ("Prof. Mattana") che pattugliano la stanza.
2. **Livello 2 (Boss Fight):** Dopo una cutscene narrativa, il giocatore viene trasportato nell'arena finale per affrontare il **Professor Musci**. Il boss attacca a distanza lanciando sanzioni scolastiche (*"Brutto Voto"*, *"Nota sul Registro"*).

Il giocatore parte con **10 HP (chiamato Voto)**. Ogni colpo subìto riduce la vita del 10%. Se gli HP si azzerano o scade il tempo, si viene **BOCCIATI**. Sconfiggendo il Prof. Musci si ottiene la **MISSIONE COMPIUTA!**.

---

## ✨ Caratteristiche Tecniche e Originalità

* **Motore 3D Raycasting Nativo:** La prospettiva tridimensionale non usa librerie esterne o motori pronti, ma proietta 180 raggi matematici in tempo reale per calcolare la distanza delle pareti e simulare la profondità (stile *Wolfenstein 3D*).
* **Z-Sorting & Sprite Rendering:** Gestione avanzata degli oggetti tridimensionali (nemici, proiettili, PC) ordinati dinamicamente in base alla distanza dal giocatore per evitare bug di sovrapposizione visiva.
* **Graffiti e Testo Prospettico:** Scritte e meme scolastici proiettati direttamente sulle pareti che si ridimensionano in tempo reale seguendo la prospettiva del giocatore.
* **Compatibilità Hardware:** Il codice include un blocco di controllo `try-except` per l'inizializzazione del mixer audio. Se eseguito sui PC della scuola privi di dispositivi di output audio, il gioco si avvia automaticamente in modalità silenziosa evitando il crash.

---

## ⌨️ Comandi di Gioco

* **W, A, S, D** (o **Frecce**): Movimento del personaggio e rotazione della visuale.
* **MOUSE (Click sinistro)** / **SPAZIO**: Spara.
* **F**: Per sparare o per interagire con i PC scolastici.
* **R** (nella schermata finale): Riavvia istantaneamente la partita.

---

## 🚀 Come Eseguire il Progetto

### Requisiti
Assicurati di avere **Python** installato sul tuo computer e la libreria **Pygame**.

Se non hai Pygame, puoi installarlo tramite terminale con:
```bash
pip install pygame
