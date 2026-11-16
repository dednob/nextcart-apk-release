# NextCart release feed

`version.json` describes the latest NextCart Android release on Google Play.
The app reads it on launch and prompts users to update when `build` is newer
than the installed build.

| Field | Meaning |
| --- | --- |
| `version` | Version name shown to users |
| `build` | Build number (versionCode) of the latest Play release |
| `min_build` | Installs below this build get a prompt they can't dismiss |
| `notes` | What's new, shown in the prompt |

It's updated automatically by the release workflow after each production
upload. Raise `min_build` by hand to force an update.
