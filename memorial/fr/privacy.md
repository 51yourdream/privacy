# Politique de confidentialité de Virtual Memorial Space

**Date d'entrée en vigueur : 1er novembre 2026**

## 1. Introduction

Virtual Memorial Space (« l'App », « nous ») est une app iOS qui permet de créer des espaces commémoratifs privés, d'accomplir des rituels de souvenir et d'écrire des lettres. Cette politique de confidentialité explique quelles informations l'App traite, où elles sont stockées et quels choix s'offrent à vous.

L'App ne nécessite aucun compte. Vos contenus commémoratifs restent sur votre appareil. Notre serveur sert uniquement aux jetons commémoratifs, des jetons intégrés à l'App, facultatifs, utilisés pour des styles d'offrandes plus raffinés.

En utilisant l'App, vous reconnaissez avoir lu et compris cette politique de confidentialité.

## 2. Informations que nous ne collectons pas

L'App ne collecte pas et ne demande pas :

- Votre nom, adresse e-mail, numéro de téléphone ou un compte de connexion
- Les noms, photos, dates, descriptions, lettres ou messages de vos espaces commémoratifs
- L'accès à l'ensemble de votre photothèque, à l'appareil photo, au micro, aux contacts ou à la localisation
- Les données de votre carte de paiement
- Un identifiant publicitaire (IDFA). L'App ne vous suit pas à travers les apps ou sites web d'autres sociétés et n'affiche pas la demande de transparence du suivi des apps (ATT).
- Des données d'analyse ou d'utilisation. L'App ne contient aucun SDK d'analyse et aucune publicité.

## 3. Contenus commémoratifs stockés uniquement sur votre appareil

Les éléments suivants sont enregistrés dans l'espace de stockage privé de l'App sur votre iPhone ou iPad :

- Espaces commémoratifs : nom, type (par exemple un proche, un partenaire, un ami ou un animal), description, date de naissance, date de commémoration, thème et réglage de rappel
- Les photos que vous ajoutez à un espace commémoratif
- Les enregistrements de rituels : la bougie, la fleur ou l'offrande en papier utilisée, le nombre de jetons dépensés, l'heure et le message éventuellement ajouté
- Les lettres que vous écrivez, brouillons compris
- Les préférences : langue, effets réduits, affichage ou non des offrandes en papier traditionnelles, fin de l'accueil, un indicateur de synchronisation d'achat en attente et un compteur qui limite les demandes d'évaluation
- Le dernier solde de jetons reçu de notre serveur, utilisé uniquement pour l'affichage hors ligne

Ces contenus ne sont pas envoyés sur notre serveur, ne sont pas utilisés à des fins publicitaires et ne servent à aucune fonctionnalité ni à aucun entraînement d'intelligence artificielle (IA). Si la sauvegarde iCloud est activée, iOS peut inclure ces données dans la sauvegarde de l'appareil, gérée par Apple sous votre identifiant Apple. L'App n'a pas de synchronisation cloud propre.

**Photos.** Vous choisissez les photos via le sélecteur de photos du système. L'App ne reçoit que les photos sélectionnées et n'accède pas à l'ensemble de votre photothèque. Une copie compressée de chaque photo choisie est enregistrée dans l'espace de stockage de l'App.

## 4. Jetons commémoratifs et notre serveur

Les jetons commémoratifs sont des achats intégrés consommables. Pour que votre solde soit conservé après une réinstallation de l'App, il est stocké sur notre serveur (« appapi »), hébergé chez Vercel, qui conserve les données dans Vercel KV (Upstash Redis).

Le serveur conserve uniquement :

- Un identifiant utilisateur généré aléatoirement, non lié à votre nom, à votre adresse e-mail ni à votre identifiant Apple
- Une empreinte (hachage) du jeton d'accès émis pour cet identifiant. Le jeton lui-même n'est pas stocké sur le serveur.
- Votre solde de jetons
- Les enregistrements d'achat : identifiant du produit, identifiant de transaction Apple, nombre de jetons et heure
- Les enregistrements de dépense : identifiant de l'offrande (par exemple un type de bougie), nombre de jetons, la clé de requête qui évite un double débit, solde après dépense et heure
- Un journal des crédits, dépenses et remboursements avec leurs montants et les identifiants de transaction ou de dépense associés

Chaque requête envoyée au serveur contient aussi la version de l'App et un identifiant d'appareil (l'identifierForVendor d'iOS), utilisés pour vérifier la signature de la requête. Comme pour tout service web, notre hébergeur peut traiter votre adresse IP dans des journaux de requêtes courants afin de fournir et de protéger le service.

Le serveur ne conserve ni votre nom, ni votre adresse e-mail, ni aucune information sur les personnes ou animaux dont vous honorez la mémoire : aucun nom, photo, lettre ou message commémoratif.

L'identifiant utilisateur et le jeton sont stockés dans le trousseau iOS de votre appareil. Ils peuvent être synchronisés via le trousseau iCloud, afin que votre solde reste disponible après réinstallation de l'App ou sur un autre appareil connecté au même identifiant Apple.

## 5. Achats

- **Apple (App Store)** traite tous les paiements via votre identifiant Apple. Nous ne recevons jamais les données de votre carte de paiement. Politique de confidentialité d'Apple : https://www.apple.com/legal/privacy/
- **RevenueCat** valide les transactions. RevenueCat reçoit l'identifiant utilisateur aléatoire ci-dessus, des informations de transaction (comme l'identifiant du produit, l'identifiant de transaction Apple et l'heure d'achat) et des informations techniques de base comme la version de l'App, la version du système d'exploitation et le pays de l'App Store. Notre serveur demande à RevenueCat de confirmer les achats, et RevenueCat informe notre serveur des achats et des remboursements, afin que les jetons ne soient crédités qu'une seule fois et repris après un remboursement. Politique de confidentialité de RevenueCat : https://www.revenuecat.com/privacy

Les jetons commémoratifs n'ont aucune valeur monétaire réelle. Les remboursements sont gérés par Apple selon ses règles. Les conditions d'utilisation sont le contrat de licence standard d'Apple : https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Notifications (facultatives)

Si vous activez un rappel de date de commémoration pour un espace, l'App demande l'autorisation d'envoyer des notifications et programme des notifications locales sur votre appareil. Les rappels ne passent pas par notre serveur. Vous pouvez les désactiver dans l'App ou dans les Réglages d'iOS.

## 7. Utilisation des informations

Nous utilisons les informations ci-dessus uniquement pour :

- Afficher et conserver vos espaces commémoratifs, rituels et lettres sur votre appareil
- Créer votre portefeuille de jetons, créditer les jetons achetés une seule fois par transaction, débiter des jetons lorsque vous choisissez une offrande premium et reprendre des jetons après un remboursement
- Vérifier les requêtes et prévenir la fraude ou les doubles crédits
- Répondre à vos demandes d'assistance

Nous ne vendons ni ne louons de données personnelles, ne les utilisons pas à des fins publicitaires et ne créons pas de profils publicitaires.

## 8. Partage

Nous ne partageons des informations qu'avec les prestataires nécessaires au fonctionnement de l'App (Apple, RevenueCat et Vercel / Upstash pour l'hébergement et le stockage), ou lorsque la loi ou une procédure judiciaire valide l'exige.

## 9. Suppression de vos données

Dans les Réglages de l'App :

- **Supprimer toutes les données (Delete All Data)** supprime tous les contenus commémoratifs de cet appareil : espaces commémoratifs, photos, enregistrements de rituels, lettres et messages.
- **Supprimer les données des jetons (Delete Token Data)** supprime votre portefeuille sur notre serveur : l'enregistrement de l'identifiant utilisateur, le hachage du jeton, le solde, les enregistrements d'achat et de dépense ainsi que le journal. Votre solde est remis à zéro et ne peut pas être restauré. Pour éviter qu'un même achat soit crédité à nouveau, nous conservons uniquement l'identifiant de transaction Apple (avec son identifiant de produit), sans l'identifiant utilisateur. L'identifiant utilisateur et le jeton sont ensuite supprimés de votre trousseau.

Supprimer l'App efface ses contenus locaux de l'appareil, mais **ne supprime pas** votre portefeuille sur notre serveur. Pour le supprimer, utilisez « Supprimer les données des jetons » avant de supprimer l'App, ou contactez-nous. Les données locales supprimées peuvent subsister dans des sauvegardes iCloud antérieures de l'appareil jusqu'à ce qu'Apple les remplace ou les supprime.

Vous pouvez également nous demander de solliciter auprès de RevenueCat la suppression de l'enregistrement d'achat qu'il détient.

## 10. Sécurité et conservation

Les connexions avec notre serveur, Apple et RevenueCat utilisent le protocole HTTPS chiffré. Les requêtes sont signées, le serveur ne conserve qu'un hachage de votre jeton et votre identité est gardée dans le trousseau iOS. Aucune méthode de stockage ou de transmission n'est totalement sûre.

- Les contenus locaux sont conservés jusqu'à ce que vous les supprimiez ou supprimiez l'App.
- Les données du portefeuille sur le serveur sont conservées jusqu'à ce que vous utilisiez « Supprimer les données des jetons » ou nous demandiez leur suppression.
- Les identifiants de transaction Apple sans identifiant utilisateur sont conservés pour éviter les doubles crédits.
- Apple et RevenueCat conservent les enregistrements d'achat selon leurs propres politiques et obligations légales.

## 11. Confidentialité des enfants

Virtual Memorial Space ne s'adresse pas aux enfants. Nous ne collectons pas sciemment de données personnelles d'enfants de moins de 13 ans (ou de l'âge minimum requis dans votre pays). Si vous pensez qu'un enfant nous a fourni des données personnelles, contactez-nous et nous les supprimerons.

## 12. Traitement international

Nos prestataires d'hébergement et de stockage ainsi que RevenueCat peuvent traiter des données aux États-Unis ou dans d'autres pays que le vôtre. Nous nous appuyons sur les garanties de ces prestataires pour ce traitement.

## 13. Vos droits

Selon votre lieu de résidence, vous pouvez disposer d'un droit d'accès, de rectification, d'effacement ou de limitation du traitement de vos données personnelles. La plupart des données se trouvent sur votre appareil et restent sous votre contrôle. Pour les données de notre serveur, utilisez « Supprimer les données des jetons » ou contactez-nous. Nous pourrons vous demander des informations permettant de retrouver les enregistrements concernés.

## 14. Modifications de cette politique

Nous pouvons mettre à jour cette politique de confidentialité. La date en haut de page changera alors. Si l'App commence à collecter de nouveaux types de données, nous mettrons d'abord cette politique à jour.

## 15. Nous contacter

Pour toute question sur cette politique de confidentialité, contactez-nous :

- E-mail : lpjustdoit@163.com

---

## Autres langues

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
