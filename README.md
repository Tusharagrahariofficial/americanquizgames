# American Quiz Games 🌎

> **Tagline:** Play, Learn, and Explore the World.  
> **Brand Name:** American Quiz Games  
> **Stack:** Next.js (App Router), React 19, TypeScript, Tailwind CSS, Lucide Icons, Canvas Confetti

An interactive, responsive, and SEO-friendly online geography quiz and educational gaming platform built for students, teachers, geography enthusiasts, and trivia buffs.

---

## 🚀 Live Features Overview

1. **Instant Solo Access**: Play all geography quizzes immediately directly in browser without mandatory sign-ups or paywalls.
2. **Synthesized Web Audio Engine**: Clean, latency-free sound effects (correct arpeggio, error buzz, streak fanfare) generated via the native Web Audio API with zero external audio download dependencies, toggleable anytime.
3. **12 Working Games & Interactive Maps**:
   - **America Capitals Quiz** (`/games/america-capitals`): All sovereign nations across North, Central, and South America and the Caribbean with streak multipliers and trivia.
   - **Flags of the Americas** (`/games/flags-of-americas`): High-definition SVG flags with color analysis and vexillological history.
   - **Layers of the Earth Game** (`/games/layers-of-earth`): Interactive geological cross-section diagram exploring the crust, lithosphere, asthenosphere, mantle, outer core, and inner core.
   - **Mexico States Quiz** (`/games/mexico-states`): Interactive SVG map covering all 31 sovereign states of Mexico + Mexico City (CDMX) with study and quiz modes.
   - **Word Mapping Game** (`/games/word-mapping`): Unscramble geographical terms, rivers, and mountain ranges with hint letter reveals.
   - **Country Flags Multiplayer** (`/games/flags-multiplayer`): Rapid-fire 2-player buzzer duel with local split-screen mode + online room PIN code support.
   - **Latin America Map Quiz** (`/games/latin-america-map`): Interactive SVG vector atlas of Central & South America with dynamic nation pinpointing.
   - **US State Capitals Games** (`/games/us-state-capitals`): 50-state curriculum standard with timed quiz sprint and interactive study flashcards.
   - **Around the World Games** (`/games/around-the-world`): 7-continent expedition across UNESCO heritage sites, mountain ranges, and planetary extremes.
   - **Travel Geography Game** (`/games/travel-geography`): Airport IATA hub codes (JFK, ORD, MEX, GRU), timezone flight math, and meridian coordinates.
   - **GeoGrid Game** (`/games/geogrid`): The viral 3x3 category matrix game with row & column criteria, country validation, and rarity scoring.
   - **GeoHistory Game** (`/games/geohistory`): Chronological borders, ancient empires (Inca, Aztec, Gran Colombia), and historical peace treaties.
4. **Daily Geography Sprint**: Consistent daily quiz seeded by the current calendar date on the homepage with streak awards.
5. **Hall of Fame & Leaderboards** (`/leaderboard`): Local storage persistence + optional Supabase cloud score synchronization with editable player nicknames and badges.
6. **Classroom & COPPA Ready**: No personal data collection from minors; works on Chromebooks, iPads, laptops, and smartboards.
7. **SEO Optimization**: Dynamic `sitemap.xml`, `robots.txt`, OpenGraph metadata, and JSON-LD `Quiz` and `WebPage` structured data.

---

## 📂 Page Routes

| Route | Page Name | Description |
|---|---|---|
| `/` | Homepage | Hero, Daily Challenge, 6 Categories, Featured Games, Classroom Highlights |
| `/games` | All Games Directory | Live search, category chips, difficulty filters, and game cards |
| `/games/america-capitals` | America Capitals Quiz | North, Central, South & Caribbean capitals with region filter |
| `/games/flags-of-americas` | Flags of the Americas | Authentic SVG vector flag identification & history |
| `/games/layers-of-earth` | Layers of the Earth Game | Interactive planetary interior cutaway with depth & temperatures |
| `/games/mexico-states` | Mexico States Quiz | Clickable SVG map of Mexico with 32 federal entities |
| `/games/word-mapping` | Word Mapping Game | Geographic anagram solver & landmass connection puzzle |
| `/games/flags-multiplayer` | Country Flags Multiplayer | Local 2-player buzzer duel + online room PIN mode |
| `/games/latin-america-map` | Latin America Map Quiz | Dynamic vector map of Central & South American nations |
| `/games/us-state-capitals` | US State Capitals Games | All 50 states, state nicknames, flashcards & speed sprint |
| `/games/around-the-world` | Around the World Games | 7-continent passport expedition & UNESCO world wonders |
| `/games/travel-geography` | Travel Geography Game | Airport IATA codes, timezone math & flight routing |
| `/games/geogrid` | GeoGrid Game | 3x3 intersecting category matrix with rarity score |
| `/games/geohistory` | GeoHistory Game | Historical treaties, empire borders & timeline sequencing |
| `/leaderboard` | Leaderboard & Hall of Fame | Per-game rankings, medals, and custom player nicknames |
| `/about` | About Us | Educational mission, pedagogy, and curriculum standards |
| `/contact` | Contact Us | Inquiries form & classroom adoption FAQ |
| `/privacy-policy` | Privacy Policy | COPPA and GDPR compliant educational privacy policy |
| `/terms` | Terms of Service | Acceptable use & classroom projection rights |

---

## 🛠️ Local Development & Testing

### 1. Installation
The project is located at:
`C:\Users\Admin\.gemini\antigravity\scratch\american-quiz-games`

```bash
cd american-quiz-games
npm install
```

### 2. Run Automated Test Suite
Executes the gameplay, scoring, streak multipliers, and GeoGrid validation tests:
```bash
npm test
```

### 3. Run Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### 4. Build Production Bundle
```bash
npm run build
npm run start
```

---

## ⚙️ Optional Supabase Configuration

To enable cloud-synced leaderboards and live remote multiplayer rooms, add your Supabase credentials to `.env.local`:

```env
NEXT_PUBLIC_SUPABASE_URL=https://your-project.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
```

*Note: If these variables are not provided, the website automatically falls back to local storage and local multiplayer seamlessly.*
