# Coilcress 1.0 TEST
Native Android Snake non-touching path shading puzzle. Android 8+ (min26), target35. Package com.gg007.coilcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Snake shading puzzle on a 4x4 grid. Shade one orthogonally connected, one-cell-wide path between the two fixed gold endpoints. Gold endpoints stay shaded and have exactly one side-neighbor; all other snake cells have exactly two. No branches, cycles or detached pieces. The four row clues and four column clues count all snake cells, including endpoints. Different parts of the snake cannot touch by sides or corners. A diagonal touch is allowed only between cells exactly two steps apart around the same bend; this does not forbid an ordinary right-angle turn. Tap non-endpoint cells to shade or clear them. Twelve original uniquely solvable shadings, automatic full-rule checking, unlimited undo/reset, next and level selection. Saved palette and optional snake-cell dots; no timer, score or explicit empty-cell notes.

## Download and status
https://mega.co.nz/#!sJNi3KyC!Mc237MefO9ItyOcF09enEh9UwKLokQu9kHA4eJaWGyc
APK SHA256 06b7539d18b0c8de42f5d2a3e4b3812593799e9aeba3b558f6a38657644bff38; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent ordered-path enumeration with sequence-distance contact checks versus production selected-cell degrees, bitset connectivity and diagonal-common-neighbor checks passed 786,432 complete-board comparisons plus 786,432 endpoint-shape comparisons. All 65,536 shadings tested on each of twelve boards; each has exactly one solution. Tests cover a legal bend corner, full straight row, forbidden solid 2x2, endpoint locks, bounds, undo, reset and solved lock. Portable generator seed 510309 reproduces twelve distinct original shadings, length 6-10. Actual drawing-adapter cell taps, solve/undo/replay, next, levels, menu, privacy and saved palette/snake-cell marks pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 182 prior studio descriptions and 803 web registry records. Branchvale already covers Slant, so that candidate was rejected. Snakefern uses two numbered snakes and sight constraints; Trackcress uses fixed rail shapes and allows neighboring tracks; Cindertrail is a move-and-collect route. Coilcress instead shades an induced single path with nonlocal corner-contact exclusions and row/column counts. Its selected-cell degree and sequence-distance contact validator differs from those games. The registry Neon Snake is an arcade game, not this deduction mechanic. No standard Snake shading match found in the reviewed corpus; repository corpus remains partial. Known Snake adaptation, not a global invention claim. Original generated boards, code and visuals, no copied puzzle layouts, code or art.
Rules https://www.gmpuzzles.com/blog/2019/06/snake-by-ashish-kumar-bonus/ ; independent rules https://www.logic-puzzles.ropeko.ch/php/db/puzzle.php?id=862 .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/coilcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.coilcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Coilcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, snake cell marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 183-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/e4ldr5puw53i-coilcress-source-archive . Repository https://github.com/iLanis-agent/coilcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
