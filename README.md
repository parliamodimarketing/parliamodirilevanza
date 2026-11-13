# Parliamo di rilevanza

Che cosa rende un brand rilevante? Questa pagina raccoglie le voci di chi i brand li guida ogni giorno: manager e professioniste intervistate da Barbara Lorenzini per il libro *Essere bravi non basta*.

Si clicca su un nome e la risposta si apre su un post-it, insieme alla domanda a cui la persona stava rispondendo.

Fa parte di [Parliamo di Marketing](https://www.parliamodimarketing.it/) e accompagna la [Matrice della Rilevanza](https://www.parliamodimarketing.it/matrice-della-rilevanza/).

## Le voci

| Nome | Brand | Ruolo |
|---|---|---|
| Margherita Galluzzo | WeRoad | Brand Marketing Director |
| Enrica Vitale | Vorwerk | Direttore Marketing Bimby® Italia |
| Chiara Panesi | Automobili Lamborghini | Customer Journey Designer |
| Allegra Panichi | Cortilia | Brand Coordinator |
| Fabrizio Nucifora | Pasta Armando | Brand Sales & Marketing Director |

Le risposte sono riportate con le parole delle intervistate, così come compaiono nel libro *Essere bravi non basta* (Barbara Lorenzini, 2026). La risposta di Allegra Panichi parte dal secondo paragrafo dell'intervista. La risposta di Fabrizio Nucifora è stata raccolta dopo l'uscita del libro, apposta per questa pagina, e trascritta dalla registrazione.

## Com'è fatta

Tutto sta in un solo file, `index.html`: testi, stile e il piccolo script che apre e chiude le risposte. Non servono librerie né passaggi di compilazione. I caratteri (Bricolage Grotesque e Newsreader) vengono caricati da Google Fonts.

## Pubblicarla con GitHub Pages

1. Carica `index.html` e `README.md` nella cartella principale del repository.
2. Vai su **Settings → Pages**.
3. In **Branch** scegli `main` e la cartella `/ (root)`, poi clicca **Save**.
4. Dopo un paio di minuti la pagina è online all'indirizzo `https://<nome-utente>.github.io/<nome-repository>/`.

## Aggiungere una voce

1. Apri `index.html` e cerca il commento `===== VOCE:`.
2. Copia un blocco intero, dal commento `<!-- ===== VOCE: ... -->` fino al `</li>` di chiusura.
3. Incollalo subito prima del commento `===== SPAZIO LIBERO`, che deve restare sempre l'ultimo.
4. Nel blocco copiato cambia:
   - l'`id` del `<li>` (minuscolo, senza spazi né accenti, per esempio `rossi`);
   - lo stesso id in `aria-controls="r-rossi"` e `id="r-rossi"`;
   - nome e cognome, brand, domanda, risposta e firma;
   - se vuoi, il colore del post-it (`--carta`) e la rotazione (`--rot`, tra `-1.5deg` e `1.5deg`).
5. La frase chiave della risposta va dentro `<strong>…</strong>`.
6. Salva e fai il commit: GitHub Pages aggiorna la pagina da solo.

Colori dei post-it: `#eaf7dd`, `#f4f8c4`, `#c9eab9`, `#dcf2e3`.

## Link diretti a una voce

Aggiungendo `#` e l'id in fondo all'indirizzo, la pagina si apre già sulla risposta di quella persona:

- `…/#galluzzo`
- `…/#vitale`
- `…/#panesi`
- `…/#panichi`
- `…/#nucifora`

Sono comodi per un post o per un messaggio all'intervistata.

## Accessibilità

Le risposte si aprono anche da tastiera. I lettori di schermo sanno quale risposta è aperta e quale è chiusa. Chi ha disattivato le animazioni nelle impostazioni del sistema non vede il movimento dei post-it.

---

Barbara Lorenzini · [parliamodimarketing.it](https://www.parliamodimarketing.it/)
