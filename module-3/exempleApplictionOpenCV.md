# Cours Python pour le traitement d'images de drones en utilisant la bibliothèque OpenCV. 

Ce cours couvre des opérations de base telles que le chargement d'une image, la conversion en niveaux de gris, la détection de contours et la superposition d'annotations. Assurez-vous d'avoir installé la bibliothèque OpenCV en utilisant la commande `pip install opencv-python`.



```python
import cv2
import numpy as np

# Chargement de l'image depuis un fichier
image_path = 'chemin/vers/votre/image.jpg'
image = cv2.imread(image_path)

# Affichage de l'image originale
cv2.imshow('Image originale', image)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Conversion de l'image en niveaux de gris
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

# Affichage de l'image en niveaux de gris
cv2.imshow('Image en niveaux de gris', gray_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Détection de contours sur l'image en niveaux de gris
edges = cv2.Canny(gray_image, threshold1=30, threshold2=70)

# Affichage des contours détectés
cv2.imshow('Contours détectés', edges)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Recherche et superposition de contours sur l'image originale
contours, _ = cv2.findContours(edges, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
cv2.drawContours(image, contours, -1, (0, 255, 0), 2)

# Affichage de l'image avec les contours superposés
cv2.imshow('Contours superposés', image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

Ce code vous donne un aperçu des étapes de base pour charger une image, la convertir en niveaux de gris, détecter les contours et superposer les contours sur l'image originale. Pour un traitement d'images plus avancé, vous pouvez également explorer d'autres fonctionnalités d'OpenCV telles que la détection d'objets, la segmentation, la manipulation de pixels, etc.

N'oubliez pas que le traitement d'images de drones peut être assez complexe en fonction de vos besoins spécifiques, notamment si vous travaillez avec des images géoréférencées, des calibrations de caméras, la correction de distorsion, etc. Ce cours est simplement une introduction aux concepts de base.