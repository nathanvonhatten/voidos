# Changelog

## 0.3 — beta

Keyboard shortcuts for getting around, widget previews and resizing, a smarter favorites default, a custom bold text color, crisper app icon edges, and a swipeable guide to it all.

**Shortcuts guide**
- A short, swipeable guide to type-to-search, the space bar, swiping to clear a notification, backspace, long-press, hold-and-drag and adding a widget, each with a small animation — shown once after setup on a fresh install, and once again after any update that touches it
- Reachable any time from Settings > About > Shortcuts guide

**Home screen**
- Space bar opens and closes the notifications panel, same as tapping the pill

**Search**
- Backspace on an empty search box now returns to the home screen

**App list**
- Backspace now returns to the home screen, same as the list button

**Settings**
- Backspace now goes back a page, same as the arrow (typing in a search box still just deletes)

**Widget**
- Add a widget now shows a preview image and a Small/Medium/Large size estimate for each one
- Resizable widgets can be resized: hold the widget, Resize widget, drag, Done

**Favorites**
- First run (and Reset) now starts with fewer favorites on a narrower screen, instead of always trying for 7

**Appearance**
- The "Dark text" toggle is now a Text section: a full color picker (hue, saturation, lightness, or a hex code, with its own Reset color) plus a Bold text toggle, for search results, the app list and anything else drawn straight on the wallpaper
- Fixed: the top search result ignored the chosen text color; it now matches the rest of the list
- Default font changed to Roboto, now bundled like the other three fonts instead of whatever the phone's own default happens to be

**Notifications**
- New color pickers for the sender, message and app name in the notification panel
- The "Notifications" label on the home screen pill now follows the custom text color too

**App icons**
- Corners and the hairline outline are now baked into each icon with a real anti-aliased edge, instead of relying on the system's own rounding, which was showing jagged, stair-stepped corners on this screen
- Screen background is a near-black instead of pure black, which softens the glow some screens show around bright, saturated icons sitting right against true black

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
