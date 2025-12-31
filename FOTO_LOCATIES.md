# 📸 Foto Locaties Overzicht

Dit document toont waar alle foto's in je project staan, zodat je ze lokaal kunt vervangen.

## 🏠 Homepage (`src/pages/home/page.tsx`)

### Hero Sectie (`src/pages/home/components/HeroSection.tsx`)
- **Achtergrond foto**: Zoek naar `background-image` of `<img>` tag in HeroSection

### CarPlay Sectie (`src/pages/home/components/CarPlaySection.tsx`)
- **Product foto's**: Zoek naar `<img>` tags in CarPlaySection

### Sterrenhemel Sectie (`src/pages/home/components/StarRoofSection.tsx`)
- **Product foto's**: Zoek naar `<img>` tags in StarRoofSection

### Sfeerverlichting Sectie (`src/pages/home/components/AmbientLightingSection.tsx`)
- **Product foto's**: Zoek naar `<img>` tags in AmbientLightingSection

### Achteruitcamera Sectie (`src/pages/home/components/BackupCameraSection.tsx`)
- **Product foto's**: Zoek naar `<img>` tags in BackupCameraSection

---

## 📱 CarPlay Pagina (`src/pages/carplay/page.tsx`)
- **Hero foto's**: Zoek naar `<img>` tags bovenaan de pagina
- **Feature foto's**: Zoek naar `<img>` tags in de features sectie
- **Gallery foto's**: Zoek naar `<img>` tags in de gallery sectie

---

## ⭐ Sterrenhemel Pagina (`src/pages/sterrenhemel/page.tsx`)
- **Hero foto's**: Zoek naar `<img>` tags bovenaan de pagina
- **Product foto's**: Zoek naar `<img>` tags in de content secties
- **Gallery foto's**: Zoek naar `<img>` tags in de gallery sectie

---

## 💡 Sfeerverlichting Pagina (`src/pages/sfeerverlichting/page.tsx`)
- **Hero foto's**: Zoek naar `<img>` tags bovenaan de pagina
- **Product foto's**: Zoek naar `<img>` tags in de content secties
- **Gallery foto's**: Zoek naar `<img>` tags in de gallery sectie

---

## 📷 Achteruitcamera Pagina (`src/pages/achteruitcamera/page.tsx`)
- **Hero foto's**: Zoek naar `<img>` tags bovenaan de pagina
- **Product foto's**: Zoek naar `<img>` tags in de content secties
- **Gallery foto's**: Zoek naar `<img>` tags in de gallery sectie

---

## 📱 Android Schermen Pagina (`src/pages/android-schermen/page.tsx`)
- **Hero foto's**: Zoek naar `<img>` tags bovenaan de pagina
- **Product foto's**: Zoek naar `<img>` tags in de content secties
- **Gallery foto's**: Zoek naar `<img>` tags in de gallery sectie

---

## 👥 Over Ons Pagina (`src/pages/about/page.tsx`)
- **Hero foto**: Zoek naar `<img>` tag in de hero sectie
- **Team foto's**: Zoek naar `<img>` tags in de team sectie (3 foto's)
- **Werkplaats foto**: Zoek naar `<img>` tag bij locatie sectie

---

## 📞 Contact Pagina (`src/pages/contact/page.tsx`)
- **Hero foto's**: Zoek naar `<img>` tags bovenaan de pagina

---

## 🎨 Realisaties Pagina (`src/pages/realisaties/page.tsx`)
- **Project foto's**: Zoek naar `<img>` tags in de gallery grid
- **Voor/Na foto's**: Zoek naar `<img>` tags in de comparison secties

---

## 🔧 Hoe Foto's Vervangen:

### Methode 1: Lokale Foto's in Public Folder
1. Plaats je foto's in de `public/images/` folder
2. Vervang de URL in de code met: `/images/jouw-foto.jpg`

**Voorbeeld:**
```tsx
// Van:
<img src="https://readdy.ai/api/search-image?query=..." />

// Naar:
<img src="/images/mijn-foto.jpg" />
```

### Methode 2: Lokale Foto's in Src Folder
1. Plaats je foto's in `src/assets/images/`
2. Import de foto bovenaan het bestand:
```tsx
import mijnFoto from '../../assets/images/mijn-foto.jpg';
```
3. Gebruik de import:
```tsx
<img src={mijnFoto} />
```

---

## 📁 Aanbevolen Folder Structuur:

```
public/
  images/
    home/
      hero-bg.jpg
      carplay-1.jpg
      sterrenhemel-1.jpg
    carplay/
      hero.jpg
      feature-1.jpg
    sterrenhemel/
      hero.jpg
      gallery-1.jpg
    about/
      team-1.jpg
      team-2.jpg
      team-3.jpg
    realisaties/
      project-1.jpg
      project-2.jpg
```

---

## 💡 Tips:

- **Foto formaten**: Gebruik `.jpg` voor foto's, `.png` voor logo's
- **Foto grootte**: Optimaliseer foto's voor web (max 500KB per foto)
- **Foto afmetingen**: Houd rekening met de aspect ratio in de code
- **Foto namen**: Gebruik duidelijke namen zoals `hero-background.jpg`

---

## 🔍 Foto's Vinden in Code:

Zoek in elk bestand naar:
- `<img src="`
- `background-image:`
- `readdy.ai/api/search-image`

Deze tonen waar foto's worden gebruikt.
