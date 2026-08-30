# Politique de confidentialité de Discretio Secure Vault

**Statut : BROUILLON / EXEMPLE — texte provisoire préparé pour la soumission au Play Store, en attente de relecture juridique finale. Ne pas considérer comme un document juridique définitif.**

*Dernière mise à jour : [DATE]*

*[Read this policy in English](PRIVACY_POLICY.md)*

Cette politique de confidentialité décrit comment Discretio Secure Vault (« l'application », « nous ») — nom de package `com.vault.trueaes` — traite les informations lorsque vous utilisez l'application.

## Résumé

Discretio est un coffre-fort chiffré, hors ligne et entièrement local à l'appareil. **Nous n'exploitons aucun serveur, et l'application ne télécharge, ne synchronise ni ne transmet jamais vos fichiers, notes, photos, dossiers, mots de passe ou tout autre contenu du coffre-fort où que ce soit.** Tout ce que vous stockez dans le coffre-fort est chiffré (AES-256-GCM pour les fichiers, AES-256-XTS pour les conteneurs cachés) et reste sur votre appareil. Nous n'avons ni système de compte ni backend, nous n'avons donc aucun moyen de voir, d'accéder, de récupérer ou de transmettre le contenu de votre coffre-fort à qui que ce soit, y compris nous-mêmes.

La seule donnée qui quitte jamais votre appareil est décrite dans la section « Achats » ci-dessous, et cette donnée est transmise à Google, pas à nous.

## Données que nous collectons

Nous — les développeurs de Discretio — ne collectons, ne stockons et n'avons accès à aucune donnée personnelle, contenu du coffre-fort ou données d'usage. L'application n'intègre actuellement aucun service d'analyse, de rapport de plantage ou de publicité.

## Données traitées par des services tiers

L'application intègre Google Play Billing pour traiter les achats intégrés. Ce service est soumis à la propre politique de confidentialité de Google, indiquée ci-dessous.

### Achats (Google Play Billing)

- Les achats intégrés (par exemple, le déverrouillage de fonctionnalités premium) sont traités entièrement par Google Play Billing.
- Nous ne recevons ni ne stockons votre moyen de paiement, les détails de votre carte ou votre adresse de facturation — ces informations sont gérées par Google. Nous recevons uniquement la confirmation qu'un droit a été acheté, information stockée localement sur votre appareil pour déverrouiller la fonctionnalité correspondante.
- Google Play Billing peut traiter des informations de compte et de transaction conformément à la [politique de confidentialité de Google](https://policies.google.com/privacy?hl=fr).

## Autorisations demandées par l'application, et pourquoi

| Autorisation | Objectif |
|---|---|
| Caméra / Microphone | Utilisée uniquement lorsque vous choisissez d'utiliser la fonction de capture sécurisée intégrée pour photographier/enregistrer directement dans le coffre-fort chiffré. Rien n'est capturé sans que vous n'ouvriez activement cette fonction. |
| Biométrie / Empreinte digitale | Utilisée uniquement pour déverrouiller l'application/le coffre-fort avec le matériel biométrique de votre appareil, en alternative à votre mot de passe principal. Les données biométriques elles-mêmes sont gérées entièrement par le système Android et n'atteignent jamais l'application ni nous. |
| Stockage / Photos et vidéos (autorisations média) | Utilisée uniquement lorsque vous choisissez d'importer un fichier/photo/vidéo existant dans le coffre-fort, ou d'en exporter/partager un. |
| Notifications | Utilisée pour des notifications locales, sur l'appareil (par exemple liées au verrouillage automatique/service en arrière-plan du coffre-fort). Nous n'utilisons pas de notifications push depuis un serveur, car nous n'avons pas de serveur. |
| Internet / État du réseau | Utilisée exclusivement par le SDK Google Play Billing décrit ci-dessus. Le code de chiffrement, de stockage et de gestion des fichiers du coffre-fort n'effectue jamais de requête réseau. |

## Conservation et suppression des données

Comme rien de ce que vous stockez dans le coffre-fort ne nous est jamais envoyé, il n'y a rien de notre côté à conserver ou à supprimer. Les données de votre coffre-fort résident uniquement sur votre appareil (ou tout stockage local/amovible que vous avez configuré), chiffrées au repos, jusqu'à ce que vous les supprimiez vous-même ou désinstalliez l'application.

## Confidentialité des enfants

L'application n'est pas destinée aux enfants, et nous ne collectons sciemment aucune information personnelle, quel que soit l'âge de l'utilisateur — cela découle automatiquement du fait que l'application ne dispose d'aucun mécanisme de collecte de données.

## Sécurité

Le contenu du coffre-fort est chiffré sur l'appareil avec AES-256-GCM (fichiers individuels) ou AES-256-XTS (conteneurs cachés compatibles VeraCrypt), avec des clés dérivées de votre mot de passe principal via Argon2id/PBKDF2. Le matériel de clé principale est généré aléatoirement et n'existe jamais que dans la mémoire native, jamais écrit en clair sur le disque. Consultez le code source public de l'application pour plus de détails techniques.

## Clause de non-responsabilité

Discretio Secure Vault est fourni « tel quel », sans garantie d'aucune sorte. En raison de la conception « zero-knowledge » décrite ci-dessus, nous n'avons aucun moyen d'accéder à vos données ou à votre mot de passe principal, de les consulter, de les sauvegarder ou de les récupérer, quelles que soient les circonstances — y compris en cas de mot de passe oublié, d'usage abusif de l'application, de perte ou de dommage de l'appareil, ou de dysfonctionnement de l'application. Vous êtes seul responsable de mémoriser votre mot de passe principal (ou de conserver en lieu sûr le code de récupération à usage unique optionnel de l'application, si vous choisissez d'en générer un) et de conserver vos propres sauvegardes — utilisez régulièrement la fonction de sauvegarde chiffrée de l'application (Paramètres → Sauvegarde chiffrée), car la perte, l'endommagement ou la désinstallation de l'appareil peuvent sinon entraîner la perte définitive de tout le contenu de votre coffre-fort. Dans toute la mesure permise par la loi, le développeur ne pourra être tenu responsable de toute perte de données ou autre dommage résultant de l'utilisation de cette application.

## Modifications de cette politique

Si cette politique évolue, nous mettrons à jour la date de « Dernière mise à jour » ci-dessus et, pour les changements substantiels, nous le mentionnerons dans les notes de version de l'application.

## Contact

Les questions concernant cette politique peuvent être soulevées via la page GitHub Issues du projet :
https://github.com/madleysk/TrueAESVault/issues

*(Adresse e-mail de contact provisoire — à remplacer avant la publication finale : `[INSERT CONTACT EMAIL]`)*

---

*Ce document est un exemple de brouillon préparé en vue d'une soumission au Google Play Store et doit être relu, affiné et remplacé par une version finale — incluant une date de « dernière mise à jour » réelle et des coordonnées de contact vérifiées — avant la publication de l'application.*
