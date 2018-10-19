# React native (RN) : quelques infos utiles 📱

## A propos de moi

Je suis un développeur freelance passionné par les applications mobile. Vous pouvez me contacter à jb@santoyamo.pro.

## Inspecter l'élément comme en HTML

Pour inspecter l'élément comme on a l'habitude de le faire en CSS.

`npm install -g react-devtools`
`react-devtools`

On aura ensuite un inspecteur (bien activer le mode debug sur son projet RN).

![Image react native debugger](https://screen.chauvin.tech/React_Developer_Tools_2018-10-19_14-41-01.png)

Facile ensuite de modifier le style, et de comprendre la structure des éléments React.

## Installer l'application Expo dans le simualteur

Pour installer l'app Expo dans le simulateur sans passer par l'App Store.
- Télécharger le dernier build : http://expo.io/--/api/v2/versions/download-ios-simulator-build[http://expo.io/--/api/v2/versions/download-ios-simulator-build]
- Extraire le contenu : `mkdir Exponent-X.XX.X.app && tar xvf Exponent-X.XX.X.tar.gz -C Exponent-X.XX.X.app`. 
- Lancer le simulateur 
- Utiliser la commande suivante pour installer Expo dans le simulateur : `run xcrun simctl install booted [Exponent-X.XX.X.app]`.
