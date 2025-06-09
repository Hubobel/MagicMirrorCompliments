## How to add the compliments to your MagicMirror
### Step 1: Check for supported languages
At the moment there are just four languages: 
- English ```en.json``` 
- **German ```de.json```**
- **Chuck Norris Facts ```chuck.json```**
- Dutch ```nl.json```
- Chuvash ```cv.json```

### Step 2: Change config
Open your config:
```bash
sudo nano ~/MagicMirror/config/config.js
```
Scroll till you can see the compliments module. It looks something like this:
```javascript
{
    module: "compliments",
    position: "lower_third"
},
```
Change it to:
nts is deprecated, please consider creating your own fork and using that url as ```remoteFile```.
```javascript
{
    module: "compliments",
    position: "lower_third",
    config: {
        remoteFile: "https://raw.githubusercontent.com/BluetriX/MagicMirrorCompliments/main/de.json"
    }
},
```
Change ```de.json``` to your own language like ```en.json``` or ```fr.json```. The abbreviation of your language can be found above.

## Credits
Dutch and English languages by [Micha den Heijer](https://github.com/michadenheijer), 
German language by https://daddyc.de,
Chuvash language by [mirontoli](https://github.com/mirontoli).
Chuck Norris Facts https://www.roundhousekick.de
# Visit MagicMirror!
[MagicMirror](https://github.com/MichMich/MagicMirror)
