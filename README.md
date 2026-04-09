# Širvintos keliauja

Interaktyvūs QR maršrutai po Širvintų rajono miestelius.

## Struktūra

```
/                        ← Pradžios ekranas (miestelių pasirinkimas)
/kernave/                ← Kernavės maršrutas (5 stotelės)
/sirvintos/              ← Širvintų maršrutas (5 stotelės)
/assets/icons/           ← Herbas ir PWA ikonos
/config.js               ← Google Maps API raktas
/manifest.webmanifest    ← PWA aprašas
/sw.js                   ← Service worker (offline palaikymas)
```

## Paleidimas

1. **config.js** – įrašyk Google Maps API raktą
2. **assets/icons/** – įdėk `icon-192.png` ir `icon-512.png` (PWA ikonoms)
3. Viską įkelk į GitHub repo, įjunk **GitHub Pages** (Settings → Pages → main branch)
4. Nukreipk `sirvintoskeliauja.lt` domeną į GitHub Pages

## Pridėti naują miestelį

1. Sukurk aplanką, pvz. `/gelvonai/`
2. Nukopijuok `/kernave/index.html` į `/gelvonai/index.html`
3. Pakeisk `STOPS` masyvą su naujomis stotelėmis
4. `/index.html` – pašalink `soon` klasę nuo Gelvonų kortelės

## QR kodai

Kiekviena stotelė turi unikalų kodą (pvz. `K001`, `K002`...).
QR kodas turi koduoti tik šį tekstą – generuok per qr-code-generator.com ar pan.

## Miesteliai

| Miestelis  | Aplankas     | Stotelės | Būsena   |
|------------|--------------|----------|----------|
| Širvintos  | /sirvintos/  | 5        | aktyvus  |
| Kernavė    | /kernave/    | 5        | aktyvus  |
| Gelvonai   | /gelvonai/   | -        | netrukus |
| Musninkai  | /musninkai/  | -        | netrukus |
| Čiobiškis  | /ciobiskis/  | -        | netrukus |
| Zibalai    | /zibalai/    | -        | netrukus |
| Jauniūnai  | /jauniunai/  | -        | netrukus |
| Alionys    | /alionys/    | -        | netrukus |
