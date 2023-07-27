# How to customize our own Ubuntu screen 😮💻
Before looking through the details, access the ```settings.json``` file !!<br><br>
🏷️[background img](#1--for-background-image)

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
