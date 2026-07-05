📄 README.md — piOP v1.0 — Operator‑Modul (RAW‑neutral)
Neutraler Operator • 0‑MANN • Slave‑Modus • NC‑kompatibel • SYNC‑fähig
🟦 1. Identität
piOP ist ein Operator‑Modul, das:

keine eigenen Werte trägt

keine Logik ausführt

keine Engine besitzt

keine Achsen besitzt

keine Marker besitzt

keine GEN/EICH/ID besitzt

piOP ist ein 0‑MANN‑Operator.

🟦 2. Zweck
piOP dient als:

Operator‑Platzhalter

Operator‑Slave

Operator‑Durchleitungsmodul

Operator‑Neutralraum

Es ist kompatibel mit:

NC

RAW

SYNC

RESPO

tri5mix

ERROR

🟦 3. Modi (alle 3 Operator‑Zustände)
1) piOP‑ROOT — RAW‑Operator
Inhalt: leer

Achsen: keine

Marker: keine

MODE: RAW

Rolle: Slave

Trigger: piOP‑ROOT.trigger

NC.link: NC.link‑Root

RAW‑Operator, Grundneutralität.

2) piOP‑NC — Neutralraum‑Operator
Inhalt: leer

Achsen: 12/4/v (mitlaufend)

Marker: keine

MODE: NC

Rolle: Slave

Trigger: piOP‑NC.trigger

NC.link: NC.link‑Flow

NC‑Operator, Flow‑Neutralität.

3) piOP‑SYNC — Kernel‑Operator
Inhalt: leer

Achsen: 19 (mitlaufend)

Marker: keine

MODE: SYNC

Rolle: Slave

Trigger: piOP‑SYNC.trigger

NC.link: NC.link_SyncPoint

SYNC‑Operator, Kernel‑Stabilität.

🟦 4. Vergleich — Alle piOP‑Modi
Modus	Inhalt	Rolle	Achsen	MODE	Trigger	NC.link
piOP‑ROOT	leer	Slave	keine	RAW	ROOT.trigger	Root
piOP‑NC	leer	Slave	12/4/v	NC	NC.trigger	Flow
piOP‑SYNC	leer	Slave	19	SYNC	SYNC.trigger	SyncPoint


🟦 5. Warum piOP leer ist (und korrekt bleibt)
piOP ist ein Operator‑Modul, das:

passiv bewertet

mitläuft

neutralisiert

stabilisiert

nicht eingreift

nicht berechnet

nicht interpretiert

Darum ist ein leeres README = korrekt.

Ein Operator muss leer sein, um neutral zu bleiben.

🟦 6. Status
RAW‑neutral

NC‑kompatibel

SYNC‑fähig

RESPO‑fähig

ERROR‑kompatibel

tri5mix‑kompatibel

0‑MANN

Slave‑Modus
