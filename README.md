# Ubuntu LTS 18.04 Unofficial Adwaita GTK Theme Evaluation

> To test out whether it may be a better idea to use Adwaita instead of Ambiance in LTS if Communitheme won't be done in time. Adwaita has a more modern codebase and, in my experience, is prefered over the now 8-year-old Ambiance. See the Screenshots below for a comparison. This uses the build system of an early version of the [Ubuntu GTK Communitheme](https://github.com/Ubuntu/gtk-communitheme).

## What has been changed from upstream Adwaita?

- The colors used in [Unity8](https://docs.google.com/presentation/d/1FtHFW67ycl6uvxZqKIZwyinVyOuV9NxXDuJv1SwQ70k/edit#slide=id.g13b3c671fc_1_0) have been applied to buttons, the headerbar, backgrounds (they are grey in upstream Adwaita) etc.
- Font weight has been reduced in the titles
> The goal is to keep this is as maintainable as possible, so no big edits here. The first variant uses the Unity8 light blue color as the main highlight color.

## Where is the shell theme?

> Will be added soon. Until then, using the upstream Adwaita one with the Ubuntu typeface should be fine.

## Screenshots

> May be outdated. Check out the [Ubuntu Community Hub Thread](https://community.ubuntu.com/t/adwaita-theme-with-unity8-colours-and-other-variants/4041) for mockups etc.

### GTK3 Widget Factory (Light Version with the light blue Unity8 accent as the primary color)

![GTK Widget Factory (Light Version with the light blue Unity8 accent as the primary color)](./screenshots/gtk3-widget-factory-light-lightblue.png)

### GTK3 Widget Factory (Dark Version with the light blue Unity8 accent as the primary color)

![GTK Widget Factory (Dark Version with the light blue Unity8 accent as the primary color)](./screenshots/gtk3-widget-factory-dark-lightblue.png)

### GTK3 Widget Factory (Ambiance for comparision)

![GTK Widget Factory (Ambiance for comparision)](./screenshots/gtk3-widget-factory-light-ambiance.png)

### Settings (Dark Version with the light blue Unity8 accent as the primary color)

![GTK Widget Factory (Dark Version with the light blue Unity8 accent as the primary color)](./screenshots/settings-dark-lightblue.png)

### Settings (Light Version with the light blue Unity8 accent as the primary color)

![GTK Widget Factory (Light Version with the light blue Unity8 accent as the primary color)](./screenshots/settings-light-lightblue.png)

## Build Setup

> You will need to have the ```sassc``` package installed in order to compile this.

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