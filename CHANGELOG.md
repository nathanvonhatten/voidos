# Changelog

## 0.2 — beta

A performance pass, redesigned dialogs, a custom accent color, and a smarter notification panel.

**Performance**
- Startup work, hot-path allocations and idle wakeups trimmed
- App icons prewarm right after the index loads (and again if the icon-size slider changes), instead of decoding mid-scroll
- Icons fade in instead of popping in when they have to be rendered fresh

**Notifications**
- Group chats stack by member name instead of one line per message
- Tapping a notification opens its own conversation, not just the app
- Swipe either direction to dismiss a single notification
- Panel height is adjustable: Small, Medium or Large

**App list**
- Long-press menu redrawn with icons and a divider before Uninstall
- Added App info and Uninstall to the long-press menu
- Uninstall now asks you to confirm first, before Android's own confirm screen
- Fixed Uninstall: a missing system permission could stop Android's own confirmation from ever appearing
- A–Z rail ticks with haptic feedback while dragging between letters, and the jump bubble fades in and out

**Apps**
- Tags are now removable chips instead of a comma-separated line

**Appearance**
- Custom accent color: pick any hue, not just the six presets
- Settings icon redrawn as the Void OS mark
- New toggle: tint the settings and list icons with the accent color instead of grey

## 0.1 — first beta

**Home screen**
- Empty black home; up to 7 favorites, hold to reorder
- One optional widget slot
- Notifications collapse into a single pill, expanding to a panel grouped by app
- Dots on favorites with something new
- Adjustable wallpaper visibility, down to solid black

**Search**
- No search bar: type on the keyboard and results appear
- Matches app names, your custom names, and tags
- Enter opens the best match
- Optional contact and system-settings search
- Frequently opened apps win ties; app names only, no timestamps

**App list**
- A–Z rail, tap or drag
- Long-press an app to favorite, rename, tag or hide it

**Notifications**
- Read-only and in memory only; never stored
- Show always, never, or auto-hide after a set time
- Per app: sender and message, count only, or off
- Ongoing, media and progress notifications filtered out

**Appearance**
- Six accent colors, used only for dots, badges, the cursor and the A–Z rail
- Four fonts
- Size sliders for favorites, icons, and list and search
- Notification opacity; dark text for light wallpapers
- App icons keep their own colors

**Privacy**
- No internet permission
- No analytics, accounts or ads
- Contacts requested only if you turn on contact search
- System backup off

**Setup**
- First-run guide, reachable again from Settings
- Default home app shortcut
- Open-source licenses
