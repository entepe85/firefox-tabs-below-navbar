# firefox-tabs-below-navbar
userChrome.css customization to put Firefox's (and forks) Proton UI tabs below the navigation bar

![grafik](https://github.com/user-attachments/assets/1690925a-82f0-4cde-b574-48dabffbafa3)

## Customization

This userChrome.css assumes that your window controls are on the left. For window controls on the right, please adapt the userChrome.css as follows:

```css
#nav-bar {
    order: -1;
    /* padding-inline-start: 140px !important; */
    padding-inline-end: 140px !important;
}
/* ... */
.titlebar-buttonbox-container {
    height: 38px;
    position: absolute;
    /* left: 0; */
    right: 0;
    top: 0;
}
/* ... */
```

All other visible customizations, e.g. the positions of back and forward buttons and the spacers in the navbar area, were made through Firefox's own "Customize toolbar".
