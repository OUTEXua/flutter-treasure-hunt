# flutter-treasure-hunt
Flutter Treasure Hunt Challenge – an app where a static map hides treasures, and your mission is to bring them to life with interactive markers, details, and persistence.

Flutter Treasure Hunt – Test Assignment
Scenario
A small adventure club wants a simple mobile app where members can see treasures hidden around town.
Instead of a live map, the app uses a static image (an artificial map). Markers are placed on that image. Tapping a marker shows details and lets the user mark the treasure as “discovered.”

Requirements
1) Home Screen
Show a single image (e.g., assets/map.png) as the map.

Place at least 5 markers at predefined positions on top of the image.

Treasures are stored in a local hard‑coded list with their positions.

The image should be pannable/zoomable so users can explore (use InteractiveViewer).

Recommended approach (not mandatory):

Use a Stack where the base is the Image.asset(...), wrapped in InteractiveViewer.

Overlay markers with Positioned (or by computing offsets inside a LayoutBuilder).

Store marker positions as relative percentages of the image size (e.g., x=0.62, y=0.35), then convert to pixels at runtime so it scales on different screens.

2) Treasure Details
When a marker is tapped, show either a small pop‑up or navigate to a new screen with:

Treasure name

GPS‑style / textual location (free text you hard‑code, since this is a fake map)

Short description (e.g., “Hidden near the old oak tree”)

A checkbox labeled “Discovered”

3) Marking as Discovered
When a user checks “Discovered”, persist that state across app restarts.

Use shared_preferences for persistence.

4) Design Constraints
No backend or API calls — all data is local.

No map SDKs (e.g., no google_maps_flutter).

Allowed package: shared_preferences (you may add simple state management like provider, but keep it minimal).

Keep the UI clean and functional — grading focuses on clarity and working features.

Sample Data (adjust positions to your image)
Golden Oak — x=0.18, y=0.72 — “Hidden near a large oak tree”

River Rock Gem — x=0.55, y=0.60 — “Under the big rock by the river”

Market Square Coin — x=0.40, y=0.28 — “Buried in the old market square”

Lighthouse Pearl — x=0.80, y=0.20 — “Inside a secret compartment”

Hilltop Crown — x=0.68, y=0.10 — “At the very top of the hill”

How We Evaluate
We care most about thinking and integrity. Specifically:

Logic — clear, step‑by‑step reasoning and sensible architecture.

Approach — how you break down the problem, code clarity, naming, and structure.

No AI / external help — complete the task on your own. (Using official Flutter/Dart docs is fine.)

We may ask for your drafts/notes for the math test and may review your commit history for this task.

Submission
Preferred: Share a public GitHub repository link (or make it accessible to outex.ua@gmail.com).

Alternative: Upload a ZIP file of your solution only if you don’t provide a GitHub link.

Short Setup/Run instructions (see below)

Optional: brief notes explaining your decisions
