# Argus native UI verification

Screenshots were captured from isolated, hidden Windows development test instances through the repository's window probe. Only the Argus window was captured. All process names, hardware, addresses and service descriptions shown come from synthetic repository fixtures. The fixture's version badge is not the built application's release version.

The translation-only build is commit `3330cd6d706af057cb3a015410313a0ff672b1dd`. The fixed source branch is `fix/native-audit`. The combined screenshots use a local merge of those two branches; that merge is not included in either source PR.

| Image | State |
|---|---|
| `translation-settings.png`, `translation-shortcuts.png` | Russian proofreading, existing layout |
| `connections-before.png`, `services-before.png`, `battery-before.png` | Existing widths and battery text layout, with proofread Russian |
| `connections-after.png`, `services-after.png` | Fixed columns, all 11 TCP states, all 7 service states and all 6 startup types; 13 px font, 1240 × 860 window |
| `battery-after.png` | Wrapping textual status, 13 px font, 1240 × 860 window |
| `battery-large-text.png` | 20 px font, 1240 × 860 window |
| `battery-small-window.png` | 20 px font, 800 × 600 window; vertically scrollable content |

These are visual and regression-test artifacts, not a benchmark. No installer, driver installation, service configuration or Task Manager replacement was exercised on the development machine.
