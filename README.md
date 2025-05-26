# OimBot - Bot Fortnite Lobby

## Description
OimBot est un bot Fortnite Lobby qui permet de gérer et d'animer votre lobby Fortnite. Il offre de nombreuses fonctionnalités comme la gestion des cosmétiques, l'émulation d'actions, la gestion des amis et bien plus encore.

## Mise à jour importante
Ce projet a été mis à jour pour utiliser la bibliothèque [rebootpy](https://github.com/xMistt/rebootpy) au lieu de fortnitepy qui n'est plus maintenue. Cette mise à jour garantit la compatibilité avec les dernières versions de l'API Fortnite.

## Prérequis
- Python 3.7+
- Compte Fortnite
- Informations d'authentification DeviceAuth (device_id, account_id, secret)

## Installation

### Cloner le dépôt
```bash
git clone https://github.com/killianrms/oimbot.git
cd oimbot
```

### Installer les dépendances
```bash
pip install -e .
```

## Configuration
1. Créez un fichier `info.json` à la racine du projet avec le contenu suivant :
```json
{
    "device_id": "votre_device_id",
    "account_id": "votre_account_id",
    "secret": "votre_secret",
    "FullAccess": ["NomUtilisateur1", "NomUtilisateur2"],
    "AdminUsers": ["AdminUtilisateur1"]
}
```

### Obtenir vos informations DeviceAuth
Pour obtenir vos informations DeviceAuth (device_id, account_id, secret), vous pouvez utiliser un outil comme [DeviceAuthGenerator](https://github.com/xMistt/DeviceAuthGenerator) ou suivre ces étapes :

1. Connectez-vous à votre compte Fortnite sur le site officiel
2. Utilisez un outil d'authentification pour extraire les informations DeviceAuth
3. Copiez ces informations dans votre fichier `info.json`

## Utilisation
Pour démarrer le bot :
```bash
python -m oimbot
```

## Commandes principales
Le bot répond à diverses commandes dans le chat du jeu. Voici quelques exemples :

- `!skin <nom>` - Change le skin du bot
- `!emote <nom>` - Fait exécuter une emote au bot
- `!backpack <nom>` - Change le sac à dos du bot
- `!pickaxe <nom>` - Change la pioche du bot
- `!ready` - Met le bot en état "prêt"
- `!unready` - Met le bot en état "pas prêt"
- `!privacy <public/private/friends/private_allow_friends_of_friends>` - Change la confidentialité du groupe
- `!help` - Affiche la liste des commandes disponibles

## Fonctionnalités
- Gestion complète des cosmétiques (skins, emotes, pioches, etc.)
- Contrôle de l'état du bot (prêt, pas prêt)
- Gestion de la confidentialité du groupe
- Système de permissions (utilisateurs admin et full access)
- Réponses automatiques aux invitations
- Et bien plus encore !

## Contribution
Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou à soumettre une pull request.

## Licence
Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.

## Crédits
- Développé par Aeroz
- Utilise la bibliothèque [rebootpy](https://github.com/xMistt/rebootpy) par xMistt
- Inspiré par les travaux de Terbau sur fortnitepy

Si vous avez besoin d'aide avec ce package, rejoignez le discord : discord.gg/lobbybot