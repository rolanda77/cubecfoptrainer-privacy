# Mentions légales et politique de confidentialité – CFOP Trainer

[Deutsch (version de référence)](README.md) · [English](README.en.md) · **Français** · [Italiano](README.it.md) · [Español](README.es.md)

*Traduction de courtoisie. En cas de divergence, seule la version allemande fait foi.*

## Mentions légales (Impressum)

Informations conformément au § 5 DDG (loi allemande sur les services numériques, anciennement § 5 TMG) :

Roland Albrecht
Im Jägeracker 42
79312 Emmendingen
Allemagne

Contact : rca@quantentunnel.de

## Politique de confidentialité

Date : 18/10/2026

### 1. Responsable du traitement

Roland Albrecht
E-mail : rca@quantentunnel.de

La personne mentionnée ci-dessus, en tant que développeur de l'application « CFOP/Fridrich-Algorithmen-Trainer » (ci-après « l'application »), est responsable au sens du Règlement général sur la protection des données (RGPD) des traitements décrits ci-dessous.

### 2. En bref

L'application ne collecte, ne conserve et ne transmet **aucune donnée personnelle au développeur ni à des tiers**. Il n'y a :

- aucun compte utilisateur ni connexion,
- aucune connexion Internet (l'application ne demande pas l'autorisation correspondante et ne communique avec aucun serveur),
- aucun service d'analyse, de pistage ou de publicité (pas de Google Analytics, pas de SDK de rapports de plantage ou de publicité),
- aucune transmission de données à des tiers, puisque aucune donnée ne quitte l'appareil.

Toutes les données générées dans l'application restent exclusivement en local sur l'appareil de l'utilisatrice ou de l'utilisateur. Cela vaut aussi pour la connexion Bluetooth facultative à un smart cube : elle s'établit uniquement directement entre l'appareil et le cube, sans accès à la localisation (section 5).

### 3. Quelles données sont enregistrées localement sur l'appareil ?

Pour assurer ses fonctions d'entraînement (entraînement aux algorithmes, cours guidé, révisions par répétition espacée), l'application enregistre les données suivantes **exclusivement en local, dans une base de données sur l'appareil concerné** :

- statistiques d'entraînement et d'exercice par cas d'algorithme (par ex. nombre d'essais, taux de réussite),
- données de planning et d'échéance des révisions par répétition espacée (date de la prochaine révision de chaque cas),
- progression dans le cours guidé (niveaux et cas déjà débloqués ou consolidés),
- variantes de séquences de mouvements enregistrées par l'utilisatrice ou l'utilisateur pour certains cas,
- langue choisie pour l'application (allemand, anglais, français, italien ou espagnol) ainsi que les autres paramètres de l'application (par ex. réglage par défaut de la vue autocollants, affichage de la série quotidienne).
- en cas d'utilisation d'un smart cube (section 5) : nom et adresse Bluetooth du dernier cube connecté avec les paramètres correspondants (connexion automatique, utilisation de l'orientation du cube) ainsi que, pour chaque essai, l'indication s'il a été réalisé au toucher ou avec le smart cube.

Ces données sont stockées sur l'appareil au moyen d'une base de données Room locale (SQLite) et du stockage local des paramètres (SharedPreferences). Il ne s'agit pas d'une transmission au développeur : personne d'autre que la personne qui utilise l'appareil n'a accès à ces données.

### 4. Fonction de sauvegarde (fichier de sauvegarde local)

Dans les paramètres, l'application permet en option de créer un fichier de sauvegarde local contenant les statistiques de réussite, l'historique des essais avec le planning et les échéances des révisions, la progression dans le cours, les variantes d'algorithmes favorites et les algorithmes enregistrés par l'utilisateur, ainsi que de recharger un fichier de sauvegarde créé auparavant. Le fichier est enregistré ou lu exclusivement via la boîte de dialogue de sélection de fichiers fournie par le système d'exploitation, à un emplacement choisi par l'utilisatrice ou l'utilisateur – l'application ne choisit aucun emplacement automatiquement et ne transmet jamais le fichier au développeur ni à des tiers. Si l'utilisatrice ou l'utilisateur choisit un dossier synchronisé avec un service cloud (par ex. une intégration Drive ou OneDrive de l'appareil), le traitement ultérieur de ce fichier relève de la politique de confidentialité du fournisseur cloud concerné, et non de celle de cette application.

### 5. Connexion Bluetooth à un smart cube (facultative)

À partir d'Android 12, l'application peut être connectée de manière facultative à un Rubik's cube Bluetooth (« smart cube », actuellement GAN i4 et GoCube) qui transmet à l'application les mouvements effectués sur le cube. Cette fonction est volontaire ; sans elle, l'application reste entièrement utilisable au toucher.

- **Connexion uniquement locale :** l'application recherche les smart cubes à proximité via Bluetooth Low Energy et se connecte directement au cube choisi. Aucun serveur, aucun compte fabricant et aucune connexion Internet n'interviennent.
- **Données traitées :** l'application reçoit du cube uniquement des événements de mouvement (quelle face a été tournée dans quel sens, avec horodatage), des événements d'orientation (position du cube dans l'espace), le niveau de batterie ainsi que le nom de l'appareil, le modèle et des informations matérielles. Ces données ne servent qu'à l'exercice en cours ; seules les données d'entraînement habituelles de la section 3 en sont conservées (séquence de mouvements, temps et note d'un essai, complétés par la source de saisie).
- **Cube enregistré :** pour pouvoir se reconnecter au même cube au démarrage suivant, l'application enregistre son nom et son adresse Bluetooth localement sur l'appareil. Cette entrée peut être supprimée à tout moment via « Supprimer » dans le menu smart cube. Ces informations ne font pas partie du fichier de sauvegarde (section 4).
- **Aucun accès à la localisation :** l'application utilise uniquement l'autorisation « Appareils à proximité » (section 8) et déclare explicitement au système qu'elle ne déduit aucune localisation de la recherche Bluetooth. Les autres appareils Bluetooth trouvés ne sont ni affichés ni enregistrés.
- **Aucune transmission :** ni les données du cube ni l'adresse Bluetooth enregistrée ne quittent l'appareil.

### 6. Aucune transmission de données, aucun serveur, aucun compte

L'application n'a pas besoin de l'autorisation d'accès à Internet et ne la possède pas. Aucune donnée n'est donc jamais transmise via l'application au développeur, à Google ou à d'autres tiers. Il n'y a ni compte utilisateur, ni inscription, ni synchronisation cloud.

### 7. Aucun service d'analyse, de pistage ou de publicité

L'application ne contient aucun logiciel d'analyse (par ex. Firebase Analytics), aucun service de rapports de plantage (par ex. Crashlytics) et aucun SDK publicitaire. Aucun profil d'utilisation n'est créé, aucune localisation n'est déterminée et aucun identifiant publicitaire n'est lu.

### 8. Autorisations de l'application

L'application ne demande aucune autorisation particulière d'accès à l'appareil (par ex. pas d'accès à la caméra, à la localisation, aux contacts, au microphone ni à Internet), à une exception près : pour la connexion facultative à un smart cube (section 5), elle utilise à partir d'Android 12 l'autorisation « Appareils à proximité » (`BLUETOOTH_SCAN` avec l'indication qu'aucune localisation n'est déduite, et `BLUETOOTH_CONNECT`). Elle n'est demandée que lorsque l'utilisatrice ou l'utilisateur recherche un cube ou s'y connecte dans le menu smart cube et peut être révoquée à tout moment dans les paramètres Android ; le reste de l'application fonctionne aussi sans elle. La fonction de sauvegarde (section 4) utilise la boîte de dialogue de sélection de fichiers du système (Storage Access Framework), qui ne nécessite aucune autorisation supplémentaire.

### 9. Durée de conservation et suppression

Les données mentionnées à la section 3 restent enregistrées localement sur l'appareil jusqu'à ce qu'elles soient :

- réinitialisées par les fonctions intégrées à l'application (par ex. « Réinitialiser » dans les statistiques ou « Supprimer mes algorithmes » dans les paramètres), ou
- entièrement supprimées de l'appareil par la désinstallation de l'application.

Le smart cube enregistré (section 5) peut en outre être supprimé à tout moment via « Supprimer » dans le menu smart cube.

Comme aucune donnée n'est enregistrée en dehors de l'appareil, il ne subsiste aucune autre copie des données après la désinstallation – à l'exception d'un fichier de sauvegarde créé par l'utilisatrice ou l'utilisateur (section 4), qui reste indépendamment de l'application à l'emplacement choisi et peut être supprimé par ses soins si besoin.

### 10. Droits de la personne concernée

Comme l'application ne transmet aucune donnée personnelle au développeur, toutes les données mentionnées à la section 3 se trouvent exclusivement sous l'accès direct et le contrôle total de l'utilisatrice ou de l'utilisateur (accès, rectification et effacement se font directement via l'application ou par sa désinstallation). Pour toute question relative à la protection des données concernant l'application, le contact indiqué à la section 1 reste néanmoins disponible à tout moment.

### 11. Mineurs

L'application ne s'adresse pas spécifiquement aux enfants et ne collecte aucune donnée personnelle, quel que soit l'âge de l'utilisatrice ou de l'utilisateur.

### 12. Modifications de cette politique de confidentialité

Cette politique de confidentialité peut être adaptée si nécessaire, par exemple lorsque de nouvelles fonctions de l'application l'exigent. La version en vigueur est disponible à l'adresse indiquée dans la fiche Play Store.

### 13. Contact

Pour toute question concernant cette politique de confidentialité ou l'application, veuillez écrire à :

rca@quantentunnel.de
