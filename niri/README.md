# cosmic-ext-niri

This is cosmic running on niri!

## Install

Either clone the repo and run `just install-niri` or install manually:
- `start-cosmic-ext-niri` somewhere in your `PATH`, e.g. /usr/local/bin
- `cosmic-ext-niri.desktop` into `/usr/share/wayland-sessions/cosmic-ext-niri.desktop`

Additionally you'll need to add this to your niri config:
```kdl
spawn-at-startup "cosmic-ext-alternative-startup"
```

I also recommend adding the following lines for the full cosmic experience to your `binds`:
```kdl
Mod+T { spawn "cosmic-term"; }
Mod+D { spawn "cosmic-launcher"; }
Mod+Shift+D { spawn "cosmic-app-library"; }
Mod+Alt+L { spawn "cosmic-greeter"; }
```
