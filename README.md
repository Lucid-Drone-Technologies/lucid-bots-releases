# Lucid Bots controller releases

Builds of the three apps that run on Lucid Bots controllers (SIYI UniRC 7 / 7 Pro):

| App | Package | What it is |
|---|---|---|
| Lucid Bots Control | `com.lucidcontroller` | The home app pilots open |
| Flight View | `org.mavlink.qgroundcontrol` | The flight screen, opened from Lucid Bots Control |
| Simulator | `com.dronesim.simulator` | Sherpa X Flight Trainer, opened from Lucid Bots Control |

Each release here is one matched set of all three, plus `manifest.json`.
Lucid Bots Control reads `releases/latest/download/manifest.json`, shows
"Update available" on its home screen, and installs whatever is behind.

All three APKs are signed with the Lucid Bots release key
(certificate SHA-256 `1110f2376380787f40f2b2ccc60db08326fc14069b0634f7651b0f241c7f746e`).

Releases are made with `lucid-app/scripts/make-release.py` in the controller repo.
