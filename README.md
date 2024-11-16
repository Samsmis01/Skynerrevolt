<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Web</title>

    <!-- Style pour l'arrière-plan et réduire la taille de la police -->
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            font-family: Arial, sans-serif; /* Police par défaut */
        }

        .background {
            background-image: url('https://images.pexels.com/photos/289262/pexels-photo-289262.jpeg'); /* Lien de la nouvelle image */
            background-size: cover; /* Couvre tout l'arrière-plan */
            background-position: center; /* Centre l'image */
            height: 100vh; /* Prend toute la hauteur de la fenêtre */
            color: white; /* Couleur du texte */
            display: flex; /* Pour centrer le contenu */
            flex-direction: column; /* Aligne verticalement */
            justify-content: center; /* Centre verticalement */
            align-items: center; /* Centre horizontalement */
            text-align: center; /* Centre le texte */
        }

        h1 {
            font-size: 24px; /* Taille de la police réduite */
        }

        img {
            width: 200px;
            height: auto; /* Pour garder les proportions de l'image */
        }

        /* Style du bouton */
        .button {
            padding: 15px 30px;
            font-size: 18px;
            font-weight: bold;
            color: white;
            background: linear-gradient(45deg, red, yellow, blue); /* Dégradé des couleurs */
            border: none;
            border-radius: 50px; /* Coins arrondis */
            cursor: pointer;
            transition: background 0.4s ease, transform 0.3s ease;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.3); /* Ombre du bouton */
        }

        /* Effet au survol */
        .button:hover {
            background: linear-gradient(45deg, blue, yellow, red); /* Inverser les couleurs */
            transform: scale(1.1); /* Agrandir le bouton au survol */
        }

        .button:active {
            transform: scale(0.95); /* Réduire légèrement le bouton lorsqu'il est cliqué */
        }

        a {
            text-decoration: none; /* Supprimer le soulignement du lien */
        }

    </style>
</head>
<body>
    <div class
