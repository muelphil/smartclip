```js
startService.applications = startService.applications.filter(e => ['Firefox', 'Word', 'Excel','IntelliJ IDEA 2023.3'].indexOf(e.name) !== -1).slice(0, 4)
```

```js
const themes = ['beach', 'coral-teal-night', 'road-work', 'lavender-haze', 'jungle-green',  'portal', 'burgundy-gold-twilight'];
let i = 0;
setInterval(() => {
    theme = themes[i % themes.length];
    window.settings.base.colorScheme = theme;
    i = i+1;
}, 2000)
``` 

https://ezgif.com/maker/