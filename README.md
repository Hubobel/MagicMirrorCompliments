## So fügen Sie die Komplimente zu Ihrem MagicMirror hinzu
### Step 1: welches File soll benutzt werden.
folgende Files stehen momentan zur Verfügung: 

- **German ```de.json```**
- **Chuck Norris Facts ```chuck.json```**
- **eine Kombi aus Facts, Philosophie und Glückwünschen ```kombi.json```**


### Step 2: Change config
Open your config:
```bash
sudo nano ~/MagicMirror/config/config.js
```

Scrollen Sie, bis Sie das compliments module sehen können. Es sieht in etwa so aus
```javascript
{
    module: "compliments",
    position: "lower_third"
},
```
Change it to:

```javascript
{
    module: "compliments",
    position: "bottom_bar", 
    config: {
      remoteFile: "https://raw.githubusercontent.com/Hubobel/MagicMirrorCompliments/main/kombi.json",
      specialDayUnique: true,
      classes: "thin medium bright"
    },
```

Chuck Norris Facts https://www.roundhousekick.de
Filosophie: https://www.swr3.de

# Visit MagicMirror!
[MagicMirror](https://github.com/MichMich/MagicMirror)
