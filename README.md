# firefox-tabs-below-navbar
userChrome.css customization to move Firefox's (and forks) Proton UI tabs below the navigation bar and the tab close button to the left. 

**PSA: This works well on GNOME, macOS and Windows 11. It's largely untested on other platforms / within other desktop environments.**

![2024-08-12_Screenshot-userChrome css](https://github.com/user-attachments/assets/136a6895-d5b3-43d7-aae7-09037eb7a5e7)

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
