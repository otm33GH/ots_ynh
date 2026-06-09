Le secret est chiffré avec un algorithme AES 256 bits symétrique dans le navigateur avant d'être envoyé au serveur. Une URL contenant l'identifiant du secret et le mot de passe est ensuite générée. Le mot de passe n'est jamais transmis au serveur, qui ne sera donc jamais en mesure de déchiffrer les secrets qu'il délivre sans effort considérable. Le secret est également supprimé dès la première lecture.

## Fonctionnalités

- Les secrets sont chiffrés avec algorithme AES 256 bits dans le navigateur.
- Le serveur ne reçoit jamais le secret en clair.
- Le secret est supprimé à la première lecture.

**Les secrets sont stockés en mémoire. Ils sont perdus au redémarrage du serveur, lors d'une mise à jour, ou d'une restauration.**