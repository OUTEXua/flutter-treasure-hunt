# flutter-treasure-hunt
Flutter Treasure Hunt Challenge – an app where a static map hides treasures, and your mission is to bring them to life with interactive markers, details, and persistence.

Flutter Treasure Hunt – Test Assignment
# 🗺️ Flutter Treasure Hunt — Test Assignment

A small adventure club wants a simple mobile app where members can see treasures hidden around town.
Instead of a live map, the app uses a **static image**. Tapping a marker shows details and lets the user mark the treasure as **“discovered.”**

---

## 📦 At a Glance
- **Platform:** Flutter (mobile)
- **Data:** local, hard-coded
- **Persistence:** `shared_preferences`
- **Map:** static image (`assets/map.png`)
- **No:** backends, map SDKs

<details>
<summary><b>Submission</b> (click to expand)</summary>

- **Preferred:** Public GitHub repo (or grant access to <code>outex.ua@gmail.com</code>)  
- **Alternative:** ZIP upload (only if no GitHub link)
- Include: source code, <code>assets/</code> with map, short run instructions, optional notes
</details>

---

## ✅ Requirements

### 1) Home Screen
- Show a single image (e.g., `assets/map.png`) as the map  
- Place **≥ 5 markers** at predefined positions on top of the image  
- Store treasures in a **local hard-coded list** with positions  
- Allow **pan & zoom** (use `InteractiveViewer`)

**Hint (optional):**
- Use a `Stack` — base: `Image.asset(...)` wrapped in `InteractiveViewer`  
- Overlay markers via `Positioned` (or compute offsets in `LayoutBuilder`)  
- Store positions as **relative percentages** (`x=0.62`, `y=0.35`) and convert to pixels at runtime

### 2) Treasure Details
On marker tap, show a pop-up or navigate to a details screen with:
- Name
- GPS-style/text location (free text; it’s a fake map)
- Short description (e.g., “Hidden near the old oak tree”)
- A checkbox **“Discovered”**

### 3) Marking as Discovered
- Persist the **Discovered** state across app restarts  
- Use **`shared_preferences`**

### 4) Design Constraints
- **No backend or API calls** — all data is local  
- **No map SDKs** (e.g., no `google_maps_flutter`)  
- Allowed: **`shared_preferences`** and simple state management (e.g., `provider`)  
- Keep UI **clean and functional** — we grade clarity & working features

---

## 🧪 Sample Data (adjust to your image)

```text
1. Golden Oak          — x=0.18, y=0.72 — "Hidden near a large oak tree"
2. River Rock Gem      — x=0.55, y=0.60 — "Under the big ro
