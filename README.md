# SteamBox


> Experimental. Expect bugs.

## Online play

**The only place where you can play online (multiplayer, Steam friends, Steam servers) is the `OPEN STEAM` button.**
It starts the real Steam client inside the app. Sign in there, open your Library and launch the game from Steam itself.

Games started from the launcher's own library run in offline/local mode and have no online features.

## Download

Get the files from the [latest release](https://github.com/LeeHinze/SteamBox-/releases/latest):

| File | What it is |
| --- | --- |
| `SteamLibrary_0.1.376.0_x64.msix` | The app |
| `SteamLibraryUWP-dev.cer` | Certificate (needed to install the app) |
| `Microsoft.VCLibs.x64.14.00.appx` | Dependency |
| `Microsoft.NET.CoreRuntime.2.2.appx` | Dependency |
| `Microsoft.NET.CoreFramework.Debug.2.2.appx` | Dependency |

## Install

### Xbox (Developer Mode)

1. Turn on Developer Mode on the console and open the **Device Portal** from a browser on your PC.
2. Go to **Add** (Home) and upload, in this order:
   1 The three `.appx` dependencies
   2 `SteamLibrary_0.1.376.0_x64.msix`
3. Open **Steam Library** from the console's Dev Home.

## How to use it

### The launcher (library)

- The GUI is made for a mouse, so on a controller you use the **cursor**:
  - Press **L3** or **R3** (click a stick) to show the mouse cursor.
  - **Left stick** moves it, **A** clicks.
  - Press **B** (or L3 / R3 again) to hide it.
- **Right stick** scrolls any list, with or without the cursor.
- When you click a text field, the Xbox on-screen keyboard opens.
- A USB or Bluetooth keyboard and mouse also work.

### OPEN STEAM (online play)

Steam's windows are shown on the TV with a pointer controlled by the controller:

| Input | Action |
| --- | --- |
| Left stick | Move the pointer |
| A | Click |
| Right stick | Scroll (mouse wheel) |
| B | Esc |
| View | Tab |
| Menu | Enter |
| X | Backspace |
| D-pad | Arrow keys |

- Starting Steam can take a while. A "Starting Steam" screen shows until the first window appears.
- Steam always opens on the **Library** page.
- When a game starts from Steam, Steam's web helper closes to save memory and comes back when the game ends.
- If a game crashes or quits within 2 minutes, a red report panel shows for 1 minute. Press **A** to close it.
- Only one 32-bit program can run at a time.

### Inside games started from Steam

To use the controller as a mouse, **hold LB and press D-pad left**. Press it again to turn it off (short rumble: strong = on).

| Input | Action |
| --- | --- |
| Left stick | Move the pointer |
| A / RT | Left click |
| X / LT | Right click |
| Right stick | Mouse wheel |
| B | Esc |
| Menu | Enter |
| View | Tab |
| Y | Backspace |
| D-pad | Arrow keys |

If a game does not use the controller in its first 8 seconds, the controller acts as keyboard and mouse:
left stick = W A S D, right stick = look, RT / LT = left / right click, A = Space, B = Ctrl, X = E, Y = R, LB = Q, RB = F,
L3 = Shift, R3 = V, D-pad = arrows, Menu = Esc, View = Tab.

## Reporting a bug

Open an issue and include:

1. The version (the `.msix` file name) and whether it was on Xbox or PC.
2. The game, how you started it (library or `OPEN STEAM`) and what happened.
3. The text from **Settings -> Game logs -> Copy to clipboard**, taken right after the problem.
4. For input problems, which device you used and whether pointer mode was on.

