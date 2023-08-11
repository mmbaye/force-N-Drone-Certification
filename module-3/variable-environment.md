## Cours : Ajouter une Variable d'Environnement sous Windows pour Agisoft Metashape

Dans ce cours, je vais vous guider étape par étape pour ajouter une variable d'environnement sous Windows, en utilisant Agisoft Metashape comme exemple. Les variables d'environnement sont des paramètres système qui permettent aux applications de trouver des emplacements et des paramètres importants pour leur fonctionnement. Voici comment ajouter une variable d'environnement pour Agisoft Metashape.

### **Étape 1 : Trouver le Chemin d'Installation d'Agisoft Metashape**

1. Ouvrez l'Explorateur de fichiers et naviguez jusqu'au dossier d'installation d'Agisoft Metashape. Par défaut, il est généralement situé dans le répertoire "C:\Program Files\Agisoft\Metashape Professional" ou "C:\Program Files\Agisoft\Metashape Standard".

### **Étape 2 : Copier le Chemin d'Installation**

1. Faites un clic droit sur la barre d'adresse dans l'Explorateur de fichiers pour mettre en surbrillance le chemin complet du dossier d'installation.
2. Appuyez sur "Ctrl" + "C" ou faites un clic droit puis sélectionnez "Copier".

### **Étape 3 : Ouvrir les Paramètres Système**

1. Cliquez avec le bouton droit sur l'icône "Ce PC" (ou "Ordinateur") sur votre bureau et choisissez "Propriétés".

### **Étape 4 : Accéder aux Paramètres Avancés du Système**

1. Dans la fenêtre "Propriétés de système", cliquez sur "Paramètres système avancés" dans le panneau de gauche.

### **Étape 5 : Ouvrir les Variables d'Environnement**

1. Dans la fenêtre "Propriétés système", cliquez sur le bouton "Variables d'environnement".

### **Étape 6 : Ajouter une Nouvelle Variable d'Environnement**

1. Sous la section "Variables d'utilisateur" ou "Variables système", sélectionnez "Nouvelle".
2. Dans le champ "Nom de la variable", entrez "AGISOFT_PATH" (ou un nom de votre choix).
3. Dans le champ "Valeur de la variable", collez le chemin d'installation que vous avez copié à l'étape 2.
4. Cliquez sur "OK" pour enregistrer la nouvelle variable.

### **Étape 7 : Modifier la Variable "Path"**

1. Dans la section "Variables système", sélectionnez la variable "Path" (ou "Chemin").
2. Cliquez sur "Modifier".
3. Cliquez sur "Nouveau" et ajoutez le chemin d'installation d'Agisoft Metashape (par exemple, "C:\Program Files\Agisoft\Metashape Professional").
4. Cliquez sur "OK" pour enregistrer les modifications.

### **Étape 8 : Enregistrer et Redémarrer**

1. Cliquez sur "OK" dans les fenêtres de paramètres système pour enregistrer les changements.
2. Redémarrez votre ordinateur pour que les modifications prennent effet.

Une fois que votre ordinateur a redémarré, Agisoft Metashape devrait être en mesure d'accéder aux emplacements spécifiés par la variable d'environnement. Cette méthode peut être utile si vous avez besoin d'indiquer à Metashape où se trouvent certaines ressources ou bibliothèques lors de son exécution.