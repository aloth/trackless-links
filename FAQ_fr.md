🇺🇸 [English](FAQ.md) | 🇩🇪 [Deutsch](FAQ_de.md) | 🇪🇸 [Español](FAQ_es.md) | 🇫🇷 **Français** | 🇯🇵 [日本語](FAQ_ja.md) | 🇨🇳 [中文](FAQ_zh-Hans.md)

# FAQ Trackless Links

**Foire aux questions et guide d'utilisation**

Bienvenue ! Ce guide vous aidera à tirer le meilleur parti de Trackless Links et répond aux questions les plus courantes.

---

## Contexte : pourquoi des URL propres comptent

Quand Tim Berners-Lee a inventé le World Wide Web en 1989, les URL étaient conçues comme de simples adresses : un moyen de retrouver un document sur un serveur. Une URL comme `boutique.com/chaussures` indiquait exactement où vous alliez.

Aujourd'hui, les URL sont devenues des outils de surveillance.

### L'économie cachée de vos clics

Chaque fois que vous cliquez sur un lien dans un e-mail, touchez une publication sur les réseaux sociaux ou suivez un résultat de recherche, du code supplémentaire est ajouté à l'URL. Ces paramètres de suivi transforment une simple adresse en un rapport détaillé sur vous :

```
shop.com/shoes?utm_source=newsletter&utm_campaign=spring_sale&utm_medium=email&fbclid=IwAR3x...&mc_eid=abc123
```

Cette unique URL révèle à plusieurs entreprises :
- Que vous venez d'une newsletter (et non du site directement)
- Que vous avez répondu à la campagne « spring sale »
- Que Facebook sait que vous avez cliqué sur ce lien précis
- Que la plateforme de marketing par e-mail a enregistré votre identifiant d'abonné

Rien de tout cela ne change la page que vous voyez. Cela change seulement ce que les entreprises apprennent sur vous.

### Comment fonctionnent les paramètres de suivi

Le point d'interrogation (?) dans une URL sépare l'adresse de la page de ses paramètres. Tout ce qui suit le point d'interrogation est constitué de métadonnées, et les entreprises ont normalisé tout cela en un véritable système de surveillance :

| Paramètre | Qui l'utilise | Ce qu'il révèle |
|-----------|---------------|-----------------|
| `utm_source` | Marketeurs en général | Le site ou la plateforme qui vous a envoyé |
| `utm_campaign` | Marketeurs en général | La publicité ou l'e-mail précis sur lequel vous avez cliqué |
| `fbclid` | Facebook/Meta | Votre identifiant Facebook et votre comportement de clic |
| `gclid` | Google | Votre profil publicitaire Google |
| `mc_eid` | Mailchimp | Votre identité d'abonné e-mail |
| `ttclid` | TikTok | Votre profil publicitaire TikTok |
| `msclkid` | Microsoft/Bing | Votre profil publicitaire Microsoft |

Quand vous partagez un lien avec des amis, vous partagez souvent aussi ces paramètres, permettant aux entreprises de pister non seulement vous, mais aussi tous ceux qui cliqueront sur le lien transféré.

### Le coût pour votre vie privée

Ce suivi se fait de manière invisible, mais les conséquences sont réelles :

**Profilage inter-sites** : Des entreprises comme Facebook et Google voient votre activité sur des millions de sites et bâtissent des profils détaillés de vos centres d'intérêt, de vos achats et de vos habitudes.

**Discrimination tarifaire** : Certains commerçants utilisent les données de suivi pour afficher des prix différents selon la disposition à payer perçue de chaque utilisateur.

**Bulles de filtres** : Les plateformes publicitaires utilisent votre historique de clics pour décider quel contenu vous montrer, ce qui peut limiter votre exposition à des points de vue variés.

**Fuites de données** : Toute entreprise qui stocke vos données de suivi est une cible potentielle. Moins on collecte de données, moins on peut en voler.

### Ce que fait Trackless Links

Trackless Links intercepte les URL avant leur chargement et supprime les paramètres de suivi. L'URL nettoyée vous mène toujours à la même page, sans diffuser votre empreinte numérique.

Avant : `amazon.com/dp/1119737281?tag=influencer-20&ref=pd_sl_abc&utm_source=instagram`

Après : `amazon.com/dp/1119737281`

Cela se produit automatiquement pour chaque lien dans Safari, redonnant aux URL ce qu'elles devaient être : de simples adresses, rien de plus.

---

## Pour bien démarrer

### Comment activer l'extension Safari ?

Après avoir installé l'application :

1. Ouvrez **Safari** sur votre appareil
2. Touchez l'icône **AA** (ou le bouton **Extensions** sur Mac) dans la barre d'adresse
3. Touchez **Gérer les extensions**
4. Trouvez **Trackless Links** et activez-la
5. Accordez les autorisations nécessaires

L'extension est désormais active et commencera à nettoyer les URL automatiquement.

### Pourquoi l'extension ne fonctionne-t-elle pas ?

Vérifiez que vous avez :
- Activé l'extension dans les réglages de Safari (voir ci-dessus)
- Accordé les autorisations nécessaires lorsque cela vous a été demandé
- L'extension a besoin d'une autorisation pour accéder au contenu des pages web

Sur Mac, vous devez également vérifier dans **Réglages Système > Confidentialité et sécurité > Extensions** et activer Trackless Links.

### Faut-il configurer quelque chose pour commencer ?

Non. Trackless Links fonctionne dès l'installation avec des réglages par défaut judicieux :
- Les paramètres de suivi sont supprimés automatiquement
- Plus de 20 redirections prédéfinies sont prêtes à l'emploi (vous activez celles que vous voulez)
- Tous les tweaks sont opt-in : n'activez que ce dont vous avez besoin

---

## Confidentialité et filtres de suivi

### Quels paramètres de suivi sont supprimés ?

Trackless Links supprime les codes de suivi courants comme :
- `utm_source`, `utm_medium`, `utm_campaign` (attribution marketing)
- `fbclid` (identifiant de clic Facebook)
- `gclid` (identifiant de clic Google)
- `msclkid` (identifiant de clic Microsoft/Bing)
- Et bien d'autres

Vous pouvez consulter la liste complète dans l'onglet **Filtres** et y ajouter vos propres paramètres.

### Comment ajouter un paramètre de suivi personnalisé ?

1. Ouvrez l'application Trackless Links
2. Allez dans l'onglet **Filtres**
3. Touchez le bouton **+**
4. Entrez le nom du paramètre (par exemple `mon_traqueur`)
5. Touchez **Enregistrer**

La prochaine fois que vous visiterez une URL contenant ce paramètre, il sera automatiquement retiré.

### Puis-je désactiver temporairement la suppression du suivi ?

Oui. Dans l'onglet **Filtres**, vous pouvez activer ou désactiver chaque filtre individuellement. Vous pouvez aussi désactiver toute la suppression en désactivant tous les filtres.

---

## Redirections

### Que sont les redirections et pourquoi les utiliser ?

De nombreux sites populaires collectent énormément de données sur leurs utilisateurs. Les redirections vous permettent d'être automatiquement renvoyé vers des alternatives respectueuses de votre vie privée, qui proposent le même contenu sans la surveillance.

**Frontends respectueux de la vie privée** : Des projets comme Nitter (pour Twitter/X), Invidious (pour YouTube) et Libreddit (pour Reddit) affichent les contenus des grandes plateformes sans vous connecter ni suivre votre comportement. Vous obtenez le contenu, eux n'obtiennent pas vos données.

**Préférences d'interface** : old.reddit.com propose l'interface classique appréciée par beaucoup. Certains sites d'actualités ont des versions mobiles plus épurées. Les redirections vous permettent d'atterrir toujours sur votre version préférée.

**Routage régional** : Redirigez automatiquement les domaines internationaux vers votre version locale, ou inversement.

### Comment activer une redirection prédéfinie ?

1. Ouvrez l'application et allez dans **Redirections**
2. Parcourez la liste des règles prédéfinies
3. Activez l'interrupteur à côté de la règle choisie
4. La redirection est active immédiatement, sans redémarrage

### Comment créer une redirection personnalisée ?

1. Allez dans l'onglet **Redirections**
2. Touchez le bouton **+**
3. Saisissez :
   - **Motif** : L'URL DE laquelle vous souhaitez rediriger (par exemple `reddit.com`)
   - **Remplacement** : Vers où rediriger (par exemple `old.reddit.com`)
   - **Titre** (facultatif) : Un nom convivial pour la règle
4. Touchez **Enregistrer**

Vous pouvez utiliser des correspondances exactes ou des expressions régulières (regex) pour des motifs avancés.

### Puis-je utiliser des groupes de capture regex et des variables ?

Oui. Encadrez la portion de motif que vous souhaitez conserver entre parenthèses `()` et référencez-la dans le remplacement via `$1`, `$2`, etc.

**Exemple : ouvrir les liens professionnels dans Microsoft Edge**

- Motif : `(https?://.*mondomaineboulot.*)`
- Remplacement : `microsoft-edge:$1`

Cela capture l'URL correspondante complète dans le groupe 1 et la colle après `microsoft-edge:`, pour que le lien s'ouvre dans Edge plutôt que dans Safari.

**Exemple : forcer le domaine Amazon France**

- Motif : `https://www\.amazon\.com/(.*)`
- Remplacement : `https://www.amazon.fr/$1`

Vous pouvez utiliser plusieurs groupes de capture dans la même règle (`$1`, `$2`, ...). Trackless Links se comporte ainsi comme Velja pour le routage des liens vers tel ou tel navigateur ou application selon le domaine.

### Puis-je réorganiser mes règles de redirection ?

Oui. L'ordre est important car la première règle qui correspond l'emporte. Pour réorganiser :

1. Allez dans **Redirections**
2. Maintenez une règle enfoncée et faites-la glisser
3. Votre priorité est enregistrée automatiquement

### Ma redirection ne fonctionne pas. Que se passe-t-il ?

Vérifiez ces points fréquents :

- La règle est-elle **activée** ? (interrupteur sur on)
- Le motif est-il correct ? (commencez par tester une correspondance exacte simple)
- Une autre règle correspond-elle avant ? (vérifiez l'ordre des règles)
- Testez-vous bien dans Safari ? (l'extension ne fonctionne que dans Safari, pas dans d'autres navigateurs)

---

## Tweaks

### Que sont les tweaks ?

Les sites modernes restreignent souvent ce que vous pouvez faire dans votre propre navigateur. Ils désactivent la sélection de texte pour empêcher la copie, lancent automatiquement les vidéos pour gonfler les statistiques d'engagement et affichent des pop-ups intrusives pour vous empêcher de partir.

Les tweaks vous redonnent le contrôle. Trackless Links inclut plus de 20 modifications de navigateur réparties en six catégories.

Tous les tweaks sont opt-in : c'est vous qui choisissez ceux à activer.

### Liste complète des tweaks

#### Lecture et interaction

| Tweak | Ce qu'il fait |
|-------|--------------|
| **Autoriser la sélection et la copie de texte** | Réactive la sélection, la copie, le collage et les menus contextuels sur les sites qui tentent de les bloquer. Indispensable pour la recherche et la prise de notes. |
| **Désactiver les boîtes de dialogue de sortie** | Évite les pénibles « Voulez-vous vraiment quitter cette page ? » lors de la navigation ou de la fermeture d'un onglet. |
| **Désactiver l'ouverture forcée de nouveaux onglets** | Empêche les sites de forcer l'ouverture des liens dans de nouveaux onglets (target="_blank"). Les liens s'ouvrent par défaut dans le même onglet. |
| **Ignorer les fragments de texte** | Supprime les fragments #:~:text= de style Chrome dans les URL afin que les pages ne défilent pas automatiquement vers le texte surligné. |
| **Autoriser le glisser-déposer** | Restaure le glisser de texte et le glisser-déposer par défaut sur les sites qui les bloquent. |

#### Gestion des bandeaux de cookies (expérimental)

Trackless Links propose une gestion intelligente du consentement aux cookies avec trois modes :

| Mode | Comportement |
|------|-------------|
| **Off** | Aucune intervention sur les bandeaux de cookies |
| **Masquer uniquement** | Masque visuellement les bandeaux sans cliquer sur quoi que ce soit |
| **Refus automatique** | Clique automatiquement sur les boutons « refuser » ou « essentiels uniquement », puis masque les bandeaux restants |

La fonction de refus automatique gère plusieurs langues et fonctionne avec Google, les principaux frameworks de consentement et de nombreux sites populaires.

#### Contrôles des médias

| Tweak | Ce qu'il fait |
|-------|--------------|
| **Toujours afficher les contrôles play/pause** | Force les contrôles natifs du navigateur sur les lecteurs audio et vidéo, même quand les sites les masquent. |
| **Bloquer la lecture automatique** | Empêche les vidéos et l'audio de démarrer automatiquement au chargement de la page. |
| **Appliquer la vitesse par défaut** | Règle tous les médias sur votre vitesse de lecture préférée (de 0,5x à 3,0x). |
| **Verrouiller la vitesse de lecture** | Empêche les sites de réinitialiser la vitesse que vous avez choisie. |
| **Mettre en pause au chargement de la page** | Met en pause chaque élément audio et vidéo au chargement d'une page. |
| **Activer le Picture-in-Picture** | Restaure la fonctionnalité PiP sur les sites qui tentent de la désactiver. Sur YouTube, balayez vers l'écran d'accueil ou verrouillez votre appareil pour lancer le PiP automatiquement, ou maintenez la vidéo enfoncée environ une demi-seconde. |

#### Confidentialité et nettoyage

| Tweak | Ce qu'il fait |
|-------|--------------|
| **Nettoyer les URL copiées** | Supprime automatiquement les paramètres de suivi de tout lien que vous copiez dans le presse-papiers. |
| **Contourner les redirecteurs courants** | Déballe les URL raccourcies (comme t.co, bit.ly) et va directement à la destination. |
| **Ouvrir dans Safari** *(nouveau en 4.1)* | Force les liens des domaines configurés à s'ouvrir dans Safari plutôt que dans l'application installée. Inclut une liste par domaine avec Instagram, X (Twitter), YouTube, TikTok, Reddit, LinkedIn, Pinterest et Spotify. Toutes les entrées sont désactivées par défaut. Vous pouvez aussi ajouter vos propres domaines. |

#### Tweaks supplémentaires

| Tweak | Ce qu'il fait |
|-------|--------------|
| **Désactiver les limites de zoom** | Supprime les restrictions de zoom sur les sites peu adaptés au mobile. |
| **Forcer le mode sombre** | Applique une inversion de couleurs intelligente pour créer des thèmes sombres sur n'importe quel site. Préserve images et vidéos tout en transformant textes et arrière-plans. |
| **Désactiver les animations** | Réduit ou supprime les animations et transitions CSS. Utile pour l'accessibilité et la concentration. |

#### Avancé (peut casser certains sites)

| Tweak | Ce qu'il fait |
|-------|--------------|
| **Forcer les barres de défilement visibles** | Rend les barres de défilement toujours visibles au lieu de les masquer automatiquement. Peut entrer en conflit avec certaines mises en page. |
| **Bloquer window.close()** | Empêche les sites de fermer votre onglet ou votre fenêtre via JavaScript. |

### Comment activer les tweaks ?

1. Allez dans l'onglet **Tweaks**
2. Parcourez les options disponibles
3. Activez ou désactivez chaque tweak
4. Les changements s'appliquent immédiatement

### Pourquoi un tweak ne fonctionne-t-il pas sur un site précis ?

Certains sites combattent activement les modifications. Si un tweak ne fonctionne pas :

- Le site utilise peut-être des techniques anti-modification agressives
- Essayez de désactiver d'autres extensions pour écarter tout conflit
- Signalez le problème sur GitHub. Nous améliorons constamment la compatibilité.

### Quelle est la différence entre « Forcer les contrôles des médias » et « Bloquer la lecture automatique » ?

- **Forcer les contrôles des médias** : Affiche les contrôles standard vidéo/audio du navigateur même quand le site les masque
- **Bloquer la lecture automatique** : Empêche les vidéos et l'audio de démarrer automatiquement au chargement d'une page

Vous pouvez les utiliser ensemble pour un contrôle maximal.

---

## Crédibilité des sources

### Qu'est-ce que la crédibilité des sources ?

La crédibilité des sources est un système d'avertissement optionnel qui vous aide à identifier les sites connus pour leur désinformation, leurs fake news ou leurs théories du complot avant d'y perdre votre temps.

Trackless Links s'appuie sur **CRED-1**, un jeu de données ouvert et évalué par des pairs recensant les domaines signalés. Lorsqu'il est activé, Safari peut afficher un bandeau d'avertissement avant ou pendant votre visite sur ces sites.

### La crédibilité des sources est-elle activée par défaut ?

Non. La crédibilité des sources est **désactivée par défaut**.

Vous pouvez l'activer quand vous le souhaitez dans l'onglet **Crédibilité**. La fonction optionnelle **Mises à jour automatiques de CRED-1** est elle aussi désactivée par défaut et doit être activée séparément.

### Comment fonctionnent les mises à jour automatiques de CRED-1 ?

Si vous activez les mises à jour automatiques de CRED-1, Trackless Links vérifie périodiquement la dernière version publiée de CRED-1 et met à jour le jeu de données présent sur votre appareil.

Détails importants :
- Les mises à jour automatiques sont **opt-in**
- L'application embarque toujours un jeu de données CRED-1 prépackagé pour que la crédibilité fonctionne sans téléchargement initial
- Les vérifications et les recherches restent **sur l'appareil** lors d'une navigation normale ; Trackless Links n'envoie pas votre historique
- Vous pouvez désactiver les mises à jour automatiques à tout moment depuis l'onglet **Crédibilité**

## Recherche dans les archives

### Qu'est-ce que la recherche dans les archives ?

Le web n'est pas permanent. Des pages sont supprimées, des articles sont modifiés et des sites entiers disparaissent. La Wayback Machine d'Internet Archive et des services similaires conservent des instantanés du web, créant un véritable historique de ce qui existait à un moment donné.

La recherche dans les archives vous donne un accès instantané à ces versions conservées :

- Retrouvez du contenu supprimé ou voyez à quoi ressemblait une page avant sa modification
- Accédez à des pages quand un site est temporairement indisponible
- Étudiez l'évolution des sites et de leurs propos au fil du temps
- Vérifiez des citations et références qui pourraient avoir été altérées

### Comment chercher dans une archive ?

**Depuis Safari :**
1. Touchez l'icône **AA** ou le bouton **Extensions**
2. Sélectionnez **Trackless Links**
3. Touchez le service d'archives souhaité (par exemple, Wayback Machine)
4. La page actuelle sera recherchée dans cette archive

**Depuis n'importe quelle application (feuille de partage) :**
1. Partagez un lien depuis n'importe quelle application
2. Choisissez **Rechercher dans l'archive**
3. Sélectionnez votre service d'archives préféré

### Puis-je ajouter d'autres services d'archives ?

Oui. Vous pouvez ajouter des services personnalisés :

1. Allez dans **Tweaks**, puis **Recherche dans les archives**, puis **Configurer les services**
2. Touchez **+** pour ajouter un service
3. Saisissez le motif d'URL du service d'archives
4. Le service est désormais disponible dans la fenêtre contextuelle

### Faut-il activer « Supprimer les paramètres de requête » ?

Recommandé : Oui. Cette option supprime les codes de suivi et autres paramètres avant la recherche dans les archives, ce qui améliore souvent les correspondances. Désactivez-la uniquement si vous devez chercher une URL avec des paramètres spécifiques intacts.

---

## Intégration à la feuille de partage

### Comment utiliser la feuille de partage pour nettoyer des liens ?

Quand vous partagez des liens depuis d'autres applications, les paramètres de suivi voyagent avec eux. L'extension feuille de partage vous permet de nettoyer les liens avant de les partager :

1. Dans n'importe quelle application (Safari, Reddit, X, etc.), touchez le bouton **Partager**
2. Faites défiler et trouvez **Nettoyer avec Trackless Links**
3. L'URL nettoyée est copiée dans votre presse-papiers

Vous pouvez maintenant partager un lien propre qui ne révèle pas où vous l'avez trouvé et ne traque pas tous ceux qui cliqueront dessus.

### Puis-je partager vers des archives depuis d'autres applications ?

Oui. Utilisez la même feuille de partage :

1. Touchez **Partager** sur n'importe quel lien
2. Choisissez **Rechercher dans l'archive**
3. Sélectionnez votre service d'archives
4. Safari s'ouvrira avec les résultats de la recherche

---

## Synchronisation iCloud

### Comment fonctionne la synchronisation iCloud ?

Vos réglages de confidentialité voyagent avec vous. Lorsque vous activez la synchronisation iCloud, votre configuration est synchronisée automatiquement entre iPhone, iPad et Mac via votre compte iCloud personnel :

- **Filtres** (paramètres de suivi)
- **Redirections** (règles personnalisées et état d'activation)
- **Tweaks** (tous les réglages)
- **Services d'archives** (ceux que vous avez configurés)

Les statistiques de confidentialité (comme le nombre de traqueurs bloqués) restent propres à chaque appareil et ne sont pas synchronisées.

### Faut-il activer la synchronisation iCloud ?

Elle est facultative. La synchronisation iCloud est désactivée par défaut. Pour l'activer :

1. Allez dans **Réglages** dans l'application
2. Trouvez **Synchronisation iCloud**
3. Activez-la

Vos réglages se synchroniseront alors entre tous les appareils connectés au même compte iCloud.

### Mes modifications ne se synchronisent pas entre mes appareils. Que se passe-t-il ?

Vérifiez ceci :

- La synchronisation iCloud est-elle **activée** sur les deux appareils ?
- Les deux appareils sont-ils connectés au **même compte iCloud** ?
- iCloud Drive est-il activé dans les **Réglages Système** (Mac) ou les **Réglages** (iOS) ?
- Les deux appareils sont-ils connectés à internet ?
- Essayez de forcer la fermeture puis de rouvrir l'application

Si la synchronisation ne fonctionne toujours pas, essayez de la désactiver puis de la réactiver.

### Puis-je utiliser Trackless Links sans iCloud ?

Oui. La synchronisation iCloud est entièrement facultative. L'application fonctionne parfaitement en stockant tous les réglages localement sur chaque appareil.

---

## Astuces

### Comment voir quels paramètres de suivi ont été supprimés ?

Consultez les **Statistiques** sur le tableau de bord principal. Elles affichent :
- Le total d'URL nettoyées
- Les redirections appliquées

### Puis-je exporter mes réglages ?

Les réglages sont stockés dans iCloud (si activé) ou localement sur votre appareil. Toutes les données restent sous votre contrôle et ne sont jamais envoyées à des serveurs tiers.

### Trackless Links ralentit-il la navigation ?

Non. L'extension est extrêmement légère et traite les URL en quelques millisecondes avant la fin du chargement des pages. Vous ne remarquerez aucun impact sur les performances.

### Puis-je utiliser Trackless Links avec d'autres extensions Safari ?

Oui. Trackless Links est conçue pour cohabiter avec d'autres extensions. En cas de conflits, essayez d'ajuster l'ordre d'exécution dans les réglages d'extensions de Safari.

### Quelle est la différence entre Trackless Links et Trackless Links Pro ?

| Fonctionnalité | Trackless Links | Trackless Links Pro |
|----------------|----------------|---------------------|
| iPhone et iPad | Oui | Oui |
| Application Mac | Non | Oui |
| Synchronisation iCloud | Oui | Oui |
| Tarif | Achat unique (iOS uniquement) | Achat universel (toutes plateformes) |

Trackless Links Pro est un achat universel. Achetez-la une seule fois et utilisez-la sur iPhone, iPad et Mac.

---

## Dépannage

### Je ne trouve pas l'extension dans Safari

Vérifiez que :
- Vous avez installé l'application depuis l'App Store
- Vous avez ouvert l'application au moins une fois
- Les extensions Safari sont activées dans vos réglages système

### Les liens ne sont pas nettoyés

Vérifiez :
- L'extension est-elle **activée** dans Safari ?
- Avez-vous accordé les autorisations nécessaires ?
- Y a-t-il des filtres **activés** dans l'onglet Filtres ?

### Ma redirection personnalisée ne fonctionne pas

- Revérifiez la syntaxe du motif (commencez par une correspondance exacte)
- Assurez-vous que la règle est **activée**
- Vérifiez qu'aucune autre règle ne correspond avant (l'ordre des règles est important)
