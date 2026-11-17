# parley-build

macOS-only steps for the Parley iPhone app (~/ios/Parley), run on GitHub Actions:

- `gh workflow run mac.yml -f what=icon`  -> artifact `icon`: Assets.car + partial.plist (from icon/AppIcon.png)
- `gh workflow run mac.yml -f what=shots` -> artifact `shots`: App Store screenshots from the simulator build in
  release asset `sim` (ParleySim.zip), using the app's PARLEY_DEMO screenshot mode.
