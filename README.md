# Ubuntu LTS 18.04 Unofficial Adwaita GTK Theme Evaluation

> To test out whether it may be a better idea to use Adwaita instead of Ambiance in LTS if Communitheme won't be done in time.
> Uses the build system of an early version of the [Ubuntu GTK Communitheme](https://github.com/Ubuntu/gtk-communitheme).

## Screenshots



## Build Setup

> You will need to have the ``` sassc ``` package installed in order to compile this.

```bash
meson build --prefix=/usr
cd build
sudo ninja install
```

## Recompile after changes

```bash
sudo ninja install
```

> After running the above in the build folder, press <kbd>Alt + F2</kbd>, then type 'rt', then press <kbd>Enter</kbd> to apply the theme. Use GNOME Tweaks to apply the theme and the GTK Inspector to switch between the light and dark variants of it. It also enables you to quickly test out changes.