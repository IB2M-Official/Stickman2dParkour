🕹️ Jeu de Plateforme HTML5
  Jeu en 2D avec détection de collision, animations, mini-map, et deux modes :
    🌱 Génération infinie avec seed :
      **https://ib2m-official.github.io/Stickman2dParkour/infinite**
    🛠️ Niveau custom défini dans levelData :
      **https://ib2m-official.github.io/Stickman2dParkour/1customlevel**

🚀 Fonctionnement
  🎮 Contrôles
    Flèches gauche/droite : déplacement
    Flèche bas : s'accroupir
    Espace : sauter
  
  🗺️ Modes de jeu
    Mode custom :
      Un niveau fixe défini dans levelData[] (plateformes avec position, taille, couleur, etc.)
    Mode infini avec seed :
      Génère des plateformes aléatoires à l'infini selon une seed, permettant de rejouer la même génération.

📦 Fichiers importants
   - sprite2.png : spritesheet du joueur
   - canvas, miniMapX, miniMapY : canvas HTML pour le jeu + mini-maps

⚙️ Modifier le niveau custom
  Dans le js :
    const levelData = [
    { x: 100, y: 600, width: 500, height: 15, color: '#888' },
    ...
    { x: 1000, y: 350, width: 100, height: 10, color: '#88f', isEnd: true }
  ];

  Ajoutez/modifiez des objets { x, y, width, height, color, isEnd }.
  Une seule plateforme doit contenir isEnd: true pour définir la fin du niveau.
