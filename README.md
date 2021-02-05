# Jeu Labyrinthe

**[Français](#français)** · **[English](#english)**

---

## Français

Petit jeu de labyrinthe fait avec Pygame, écrit au lycée. On choisit un personnage (Itachi ou Luffy) et on doit traverser 10 niveaux en évitant les murs, avant que le temps ou les vies ne tombent à zéro.

### Comment jouer

- Flèches directionnelles pour se déplacer.
- Menu Settings : choix du personnage et de la difficulté (Easy / Normal / Hard, qui change le nombre de vies, le temps et la vitesse).
- Menu Levels : accès direct à un niveau précis.
- Chaque collision avec un mur retire une vie.

### Lancer le jeu

Nécessite Python 3 et pygame (`pip install pygame`).

Le chemin vers le dossier `waw/` est codé en dur dans `JeuLabyrinthe.py` et `Personnage.py` (`os.chdir(...)`). Avant de lancer le jeu, remplacez ce chemin par celui du dossier sur votre machine.

```bash
git clone https://github.com/AdemmBr/Jeu-Labytinthe.git
cd Jeu-Labytinthe/waw
# éditer le os.chdir(...) dans JeuLabyrinthe.py et Personnage.py
python JeuLabyrinthe.py
```

### Organisation

```
waw/
├── JeuLabyrinthe.py   menu et boucle de jeu
├── Personnage.py      classes Blocks, Player, et éléments d'interface
├── Niveaux/           10 niveaux, un fichier texte par niveau (: = chemin, m = mur)
├── Police/            police utilisée pour le menu
└── (images des personnages, du fond et du labyrinthe)
```

---

## English

Small maze game made with Pygame, written in high school. Pick a character (Itachi or Luffy) and make your way through 10 levels, avoiding walls, before time or lives run out.

### How to play

- Arrow keys to move.
- Settings menu: pick your character and difficulty (Easy / Normal / Hard, which changes lives, time and speed).
- Levels menu: jump straight to a specific level.
- Hitting a wall costs one life.

### Running it

Requires Python 3 and pygame (`pip install pygame`).

The path to the `waw/` folder is hardcoded in `JeuLabyrinthe.py` and `Personnage.py` (`os.chdir(...)`). Before running, replace it with the folder's actual path on your machine.

```bash
git clone https://github.com/AdemmBr/Jeu-Labytinthe.git
cd Jeu-Labytinthe/waw
# edit the os.chdir(...) call in JeuLabyrinthe.py and Personnage.py
python JeuLabyrinthe.py
```

### Layout

```
waw/
├── JeuLabyrinthe.py   menu and game loop
├── Personnage.py      Blocks, Player and UI helper classes
├── Niveaux/           10 levels, one text file per level (: = path, m = wall)
├── Police/            font used for the menu
└── (character, background and maze images)
```
