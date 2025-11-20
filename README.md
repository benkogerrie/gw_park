# GW-Park Website

Moderne website voor GW-Park - Gewerbeparks für den Mittelstand.

## Over het project

Deze website presenteert GW-Park's concept voor moderne gewerbeparks in duurzame houtbouw. De site is gebouwd als statische website met Vite.

## Technologie

- **Vite** - Build tool en development server
- **TypeScript** - Type-safe JavaScript
- **HTML/CSS** - Moderne, responsive website
- **Web3Forms** - Contact formulier handling

## Lokaal draaien

**Vereisten:** Node.js (versie 18 of hoger)

1. Installeer dependencies:
   ```bash
   npm install
   ```

2. Start development server:
   ```bash
   npm run dev
   ```

3. Open je browser op `http://localhost:3000`

## Build voor productie

```bash
npm run build
```

De gebouwde bestanden staan in de `dist` folder.

## Preview productie build

```bash
npm run preview
```

## Contact Formulier Setup

Het contactformulier gebruikt Web3Forms voor het verzenden van emails. Om het werkend te maken:

1. Ga naar [Web3Forms](https://web3forms.com/)
2. Voer je email adres in (bijv. `info@gw-park.de`)
3. Krijg je gratis access key
4. Vervang `YOUR_ACCESS_KEY_HERE` in `index.html` met je access key
5. Commit en push de wijziging

**Gratis:** Tot 250 submissions per maand, geen creditcard nodig.

## Deployment

Deze site is geconfigureerd voor deployment op Cloudflare Pages.

### Cloudflare Pages Setup

1. Ga naar [Cloudflare Dashboard](https://dash.cloudflare.com/)
2. Log in of maak een account aan
3. Ga naar **Pages** in het linker menu
4. Klik op **Create a project**
5. Kies **Connect to Git**
6. Autoriseer Cloudflare om toegang te krijgen tot je GitHub account
7. Selecteer de repository: `benkogerrie/gw_park`
8. Configureer build settings:
   - **Framework preset:** None
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
   - **Root directory:** `/` (laat leeg)
   - **Deploy command:** (leeg laten)
9. Klik op **Save and Deploy**

Je site krijgt automatisch een URL zoals: `https://gw-park.pages.dev`

## Content Management (Decap CMS)

Bezoek `https://gw-park.de/admin` om teksten te bewerken via Decap CMS.

**Let op:** Voor GitHub authenticatie moet je een OAuth App aanmaken in GitHub Settings → Developer settings → OAuth Apps.

## Project structuur

- `index.html` - Hoofd HTML bestand met alle content en styling
- `index.tsx` - Entry point voor development
- `vite.config.ts` - Vite configuratie
- `tsconfig.json` - TypeScript configuratie
- `content/site/` - JSON bestanden voor CMS content
- `public/admin/` - Decap CMS configuratie
- `pictures/` - Afbeeldingen voor de website

## Licentie

© 2024 GW-Park. Alle rechten voorbehouden.
