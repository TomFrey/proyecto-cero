# proyecto-cero

## Neues Projekt aufsetzen
- Neues Repository auf GitHub erstellen (proyecto-xyz)
- Neuen Ordner unter Projekte/proyectoXyz erstellen
- Proyecto-cero zip downloaden von GitHub und im Order Projekte/proyectXyz entzippen
- Entzippter Ordner in  proyecto-xyz umbenennen

- In der Konsole in den Ordner Projekte/proyectoXyz/proyecto-xyz wechseln und:
git init <br> 
git add . <br> 
git commit -m "first commit" <br> 
git branch -M main <br> 
git remote add origin https://github.com/TomFrey/proyecto-xyz.git <br> 
git push -u origin main <br> 


## Projekt builden
Wenn ein neues Package mit yarn hinzugefügt wird (yarn add --dev <package>), 
dann verschwindet der node_modules Ordner.
Projekt wieder builden mit 'npm install gulp'.

- rm -rf node_modules
- yarn install (updates .pnp.cjs --> yarn im PlugAndPlay Modus)
- npm install gulp (erstellt node_modules)
- gulp


### gulp
Startet die Listener
Anwendung läuft unter: http://localhost:8888
Nicht vergessen MAMP starten

### gulp build
Minimiert die css und js Files und kopiert alles in einen dist Ordner

### gulp deployToTest
Das Projekt wird auf den Test Server gestellt

### gulp deployToProduction
Das Projekt wird auf den Server gestellt
