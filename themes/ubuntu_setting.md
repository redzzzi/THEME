# How to customize our own Ubuntu screen 😮💻
Before looking through the details, access the ```settings.json``` file !!<br><br>
🏷️[background img](#1-setting-for-background-image)

---

## 1. Setting for Background Image
<code>Find the lines below</code>

```json
"profiles": 
{
    "defaults": 
    {
```
<br>

<code>In "defaults", Add two kinds of codes below</code>
```json
"backgroundImage": "<path of the image>",
"backgroundImageOpacity": <opacity you want from 0 to 1>
```
<br>

```EXAMPLE```
```json
    "profiles": 
    {
        "defaults": 
        {
            "backgroundImage": "User/redzzzi/Pictures/wallpaper/manythings.jpg",
            "backgroundImageOpacity": 0.2,
            "colorScheme": "Solarized Dark",
            "opacity": 30,
            "padding": 8,
            "useAcrylic": true
        },
```

<br>

<p align="center"><img src="https://github.com/redzzzi/THEME/assets/127263392/265d4f32-29d2-4252-bba7-7d7ac901c0ea" width="700px"></p>

<p align="center">
    <a href="https://www.wallpaperflare.com/pattern-design-dark-texture-graphics-icon-neon-icons-wallpaper-gigt"><i>wallpaper source</i></a>
</p>
