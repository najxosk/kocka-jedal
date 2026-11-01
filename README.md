# Kocka jedál 🎲

Mini web-app: **3D kocka, ktorá hodí nápad, čo jesť.** Po slovensky, na mobil aj počítač.

## Live
👉 **https://najxosk.github.io/kocka-jedal/**

## Čo to robí
- 🍖 Klasická kocka (mäsité jedlá)
- 🥦 Vegetariánska kocka
- 🎲 Kocka sa roztočí → rozpadne sa → z jej stredu vypadne jedlo
- 📝 Nepadne to isté dvakrát za sebou (pamätá posledných 10 hodov)

## Ako spustiť
- **Online:** otvor link vyššie v prehliadači (Chrome/Safari)
- **Offline / lokálne:** otvor `index.html` v prehliadači
- **Ako appka na mobile:** Chrome → ⋮ → *Pridať na plochu*

## Technológia
- Jeden statický HTML súbor (`index.html`), žiadne závislosti, žiadny server
- CSS 3D transformácie pre kocku, čistý JavaScript bez knižníc
- Dáta v `localStorage` (zoznam posledných hodov)

## Štruktúra kódu
- `KLASIKA` / `VEG` — polia jedál `[emoji, názov, poznámka]`
- `roll()` — hlavná logika hodu (výber + animácia)
- `resetCube()`, CSS `.show` triedy — animácia rozpadu a vypadnutia jedla

## Roadmap
- [ ] Viac kociek: filmy, seriály, kamaráti, pár
- [ ] Kombinovanie viacerých kociek
- [ ] Vylepšenie vzhľadu / zvuku

## Pre vývojárov / AI agentov
- Pridaj jedlo jednoducho: vlož riadok do pola `KLASIKA` alebo `VEG`
- Testovanie: otvor `window.GAME` v konzole — `.get()`, `.roll()`, `.set('veg')`
- Appka beží čisto na strane klienta — zmeny v `index.html` stačí prepísať na GitHub
