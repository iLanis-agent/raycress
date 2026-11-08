# Raycress 1.0 TEST
Native Android Black Box deduction. Android 8+ (min26), target35. Package com.gg007.raycress. Twelve original small layouts.

## Rules
Black Box deduction. Two fixed hidden balls occupy a 4x4 box. Tap perimeter ports A-P to fire probes, and tap cells to mark or remove two guesses. A direct hit is H and takes priority over diagonal effects. With no ball straight ahead, a forward-diagonal ball turns the ray 90 degrees away; two diagonals turn it back. A turn before entering the box, or an exit at the entry port, is R. Other exits display > followed by their port letter, rather than paired shot numbers. Repeated probes show the same result. Mark exactly two guesses and CHECK: all sixteen possible ray results must match, not just probes already seen. A wrong check highlights or reveals one contradictory probe, never a correct ball location. No timer, probe limit or competitive score. Twelve original two-ball layouts, all uniquely identifiable from the complete probe mapping. Undo restores guesses, observations and completion; reset/next/levels and saved palette/cell numbers. This is a small-grid adaptation of the known game, not the original board-game scoring rules.

## Download and status
https://mega.co.nz/#!YQMzmIja!7IoobOcvgFaBRPeFZ-wSgbv09G-2xGI59Hgpdnug1Ic
APK SHA256 41c3e79e877f0fda447e18f8ad0b020b3973f9fd4b8cb0249133d896cbad7597; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Icon unchanged.

## Checks
Portable generator enumerates all 120 two-ball sets and all 1,920 perimeter rays. Independent Java extended-board vector tracing agrees with production direction-table ray tracing for every case, and every exiting ray has a reciprocal exit. All 786,432 level/mask checks (all 65,536 masks on each level) pass, and all twelve original layouts have unique full signatures among all 120 sets; each includes hits, reflections and exits. All 1,428 wrong-pair checks reveal a genuine counterexample, and undo restores its prior observations. Direct-hit precedence, empty-box exits, edge reflection, bounds, duplicate probe history, two-guess limit, solved lock, undo/replay and reset pass. Actual drawing-adapter taps for probe/guess/check/undo/next/levels/menu/privacy/settings and saved palette/cell numbers pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 169 prior studio card mechanics and the 803-app web registry. Prism Relay changes visible mirrors to route a known beam; Raycress instead leaves the hidden field fixed, gathers indirect hit/reflection/exit observations, and submits a two-cell hypothesis checked against all rays. Fleetshore places ships from line totals; Beaconisle uses direct row/column tower counts, not hidden ray deflections. No Black Box functional match found in the reviewed catalog. A Bulls and Cows proposal was rejected because the existing web Mastermind app already covers code-breaking feedback. Known Black Box by Eric Solomon, no global invention claim. Original generated boards and implementation; no source puzzle, art or code copied. Recovered repository corpus remains partial.
Primary rules https://www.chiark.greenend.org.uk/~sgtatham/puzzles/doc/blackbox.html ; independent KDE rules https://docs.kde.org/stable_kf6/en/kblackbox/kblackbox/rules_and_tips.html .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json and all-rays.json. javac -d /tmp/ray-test src/com/gg007/raycress/Board.java BoardTest.java then java -cp /tmp/ray-test com.gg007.raycress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private signing inputs. No secrets in source. Release build settings; signed TEST artifact, not final store release.

## Privacy and branding
Raycress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, cell numbers and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative170-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/6mfigm7927vm-raycress-source-archive . Repository https://github.com/iLanis-agent/raycress holds README only; full Git source commit pending. Both website publications verified separately. The existing studio Jekyll build assembles static HTML from two preserved card fragments, avoiding the 256KiB editor field limit without removing entries or adding a client-side loader. No Pages settings change, spending or Play rollout. November 8, 2026.
