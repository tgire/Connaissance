1/Définir le dossier de partage hôte (sous Windows):

Il faut donc choisir sous Virtualbox comme indiqué dans l'image ci-dessous :
-Le chemin du dossier: par exemple 'C:\Users\Toto\Downloads'
-Un nom pour ce partage : par exemple 'drive'

2/Définir le dossier de partage machine virtualisée (sous Linux):

Démarrer votre machine virtuel de type linux, nous allons créer un dossier de partage sous le home par exemple.On va le nommer 'share' pour le tutoriel.

3/Lier les 2 dossiers, permettre le partage:

Ouvrez un terminal, on va monter le dossier de partage drive:

1

sudo mount -t vboxsf drive ~/share

'drive' est le nom du partage de dossier de partage dont on parlait précédemment
Le symbole "~" signifie home sous linux, on aurait pu mettre /home à la place.
Rendez vous sur le dossier 'share', le dossier est enfin partagé, enjoy!!
4/Délier les 2 dossiers (optionnel):

Pour démonter le dossier share, tapez simplement en terminal:

1

sudo umount ~/share

http://www.seeyar.fr/partage-dossier-virtualbox/
