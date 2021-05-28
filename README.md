# thumbledore

> This script is a work-in-progress --- it doesn't yet work *quite* the way it should. Full disclosure: I do not know what I am doing.

Besides promoting bad posture, the layout of standard keyboards is hardly optimal. The most glaring problem is, in my opinion, the lack of a split spacebar, which forces one of your thumbs to idle around while your weakest finger contorts to reach Control, Backspace and Enter. The addition of a secondary thumb key on keyboards would be an easy fix, with massive potential benefit.

But alas, we have to work with what we've got. Although I have been enticed by exotic keyboards like the Kinesis Advantage, what has held me back is portability: you'd have to lug around a secondary keyboard wherever you go. Besides — let's not chuck any electronics in the landfill.


## Tweaks

Within the constraints imposed on us by standard keyboards, I think the following tweaks *make sense*:

1. *Holding* `Alt_L` or `Alt_R` exposes a secondary layer on the keyboard that contains a numpad and some extra symbols. To keep things simple, it doesn't matter whether you press the right or left one, except:
2. `Alt_L + space` is `BackSpace`, while `Alt_R + space` is `Delete`. Notice how the movement of your thumbs mirrors the direction of the removal.
3. *Tapping* `Alt_R` on its own triggers an `Enter`. `Alt_R` would be a `Tab`.
4. The original `Tab` triggers the `Compose` key. This way, you would type special characters by typing intuitive keys in succession (e.g. `" + e` → `ë`). See the compose table at `/usr/share/X11/locale/$LANG/Compose`. On the secondary layer, `Tab` triggers the `dead_greek` key. This is a similar dead key, but for easily typing Greek characters (e.g. `f` → `φ`).
5. *Holding* `CapsLock` turns it into a `Super` modifier. This is convenient for controlling a window manager: it's the single key for all non-application-specific keybindings.
6. *Tapping* `CapsLock` triggers `Escape`, for modal applications like `vim`.
7. `Ctrl` stays where it is, while `Alt_L` swaps places with the `Super` key. `Alt` and `Control` are often used by applications that prefer key chording for shortcuts (rather than modes): let's put them cozily together in the bottom left corner.


This has the following benefits:

- Achievable using any run-of-the-mill keyboard.
- Only uses standard tools. The tweaks I propose here could also be achieved with the excellent [kmonad](github.com/david-janssen/kmonad), but that approach — while certainly easier to understand once it is up and running — isn't as plug-and-play.
- Encourages using only keys that would be available on any 65% keyboard. Fumbling around for special function keys is no good.


## Related software

- [kmonad](https://github.com/david-janssen/kmonad)
- [xcape](https://github.com/alols/xcape)
- [caps2esc](https://gitlab.com/interception/linux/plugins/caps2esc)
- [space2ctrl](https://github.com/r0adrunner/Space2Ctrl)
- [klfc](https://github.com/39aldo39/klfc)
- [keynav](https://www.semicomplete.com/projects/keynav/)
- [map2](https://github.com/shiro/map2)
- [at-home-modifier-evdev](https://gitlab.com/at-home-modifier/at-home-modifier-evdev)
- [evscript](https://github.com/unrelentingtech/evscript)
- [evcape](https://github.com/wbolster/evcape)
- [ergo](https://github.com/lcarsos/ergo)


## Related reading

- <https://wiki.archlinux.org/index.php/X_keyboard_extension>
- <https://www.charvolant.org/doug/xkb/>
- <https://www.x.org/releases/X11R7.7/doc/xorg-docs/input/XKB-Enhancing.html>
- <http://www.pixelbeat.org/docs/xkb_remap/>
