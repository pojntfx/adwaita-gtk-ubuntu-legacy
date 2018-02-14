# Ubuntu LTS 18.04 Unofficial Adwaita GTK Theme Evaluation

> To test out whether it may be a better idea to use Adwaita instead of Ambiance in LTS if Communitheme won't be done in time.
> Uses the build system of an early version of the [Ubuntu GTK Communitheme](https://github.com/Ubuntu/gtk-communitheme).

## What has been changed from upstream Adwaita?

- Colors are the ones used in [Unity8](https://docs.google.com/presentation/d/1FtHFW67ycl6uvxZqKIZwyinVyOuV9NxXDuJv1SwQ70k/edit#slide=id.g13b3c671fc_1_0)
- Font weight has been reduced in the titles
> The goal is to keep this is as maintainable as possible, so no big edits here.

## Where is the shell theme?

> Will be added soon. Until then, using the stock Adwaita one with the Ubuntu typeface should be fine.

## Screenshots

> Will be added soon. Check out the [Ubuntu Community Hub Thread](https://community.ubuntu.com/t/adwaita-theme-with-unity8-colours-and-other-variants/4041) for mockups etc.

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