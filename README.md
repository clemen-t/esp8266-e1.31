# Controleur Pixel Wifi

## Objectif du projet
- Développement d'un controleur wifi basé sur un ESP8266
- Code open source
- Up to 4 universes
- Développement d'un PCB

## Hardware
  - ESP8266
  - LEDs pixels (WS2811 / WS2812)

## Avancement
- Fonctionne avec 1 universe (24/04/17)

## Programmation
* Programmer un ESP8266 avec l'IDE Arduino
  - installer l'IDE Arduino
  - Aller dans `fichier > préférences`, Dans la case "Additional Boards Manager URLs", entrez l'adresse suivante
    ```
    http://arduino.esp8266.com/staging/package_esp8266com_index.json
    ```
  - Puis, aller dans `outils > Type de carte > Boards manager`, rechercher `esp8266`
  - Cliquer sur "install"
  - Dans `outils > type de carte`, Vous devriez voir apparaitre une nouvelle option `Generic ESP8266 Module`
* Flasher le code dans l'ESP8266 (Cette partie sera mise à jour lorsque notre propre code sera fonctionnel)
  -  Telecharger le code disponible sur ce dépot :
  -  Ouvrer l'exemple `  ` avec l'IDE Arduino
  -  Ouvrir le terminal Arduino et le serveur DHCP attribu une adresse IP, celle ci est affiché sur le terminal

* Xlights (Ce tuto n'a pas but de développer en détail le logiciel xLights)
  - ,

### Todos
  + Software
    - 4 Universes
  + Hardware
    - PCB

### lien
- https://www.fais-le-toi-meme.fr/fr/electronique/tutoriel/programmes-arduino-executes-sur-esp8266-arduino-ide
-





