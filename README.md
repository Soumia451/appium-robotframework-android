# Tests mobiles automatisés — Appium + Robot Framework (Android)

Projet réalisé dans le cadre de ma formation Testeur logiciel.

Automatisation de tests d'une application mobile Android (app démo SwagLabs) avec Appium et Robot Framework, exécutés sur émulateur Android.

## Objectifs

- Automatiser les parcours critiques d'une application mobile : connexion, ajout au panier, tunnel de commande
- Couvrir les cas passants et non passants (identifiants invalides, message d'erreur)
- Générer des rapports d'exécution détaillés (report.html, log.html)

## Scénarios couverts

- Connexion valide, ajout d'un produit au panier et saisie des informations de commande (checkout)
- Connexion avec identifiants invalides : vérification du message d'erreur affiché

## Stack technique

| Outil | Usage |
|-------|-------|
| Appium (UiAutomator2) | Automatisation mobile Android |
| Robot Framework + AppiumLibrary | Écriture des scénarios de test |
| Android Studio | Émulateur Android |
| Node.js | Serveur Appium |

## Structure du projet

    test.robot     # Scénarios de test (login, panier, checkout)
    .gitignore     # Exclut les rapports générés à chaque exécution

## Lancer les tests

    # Prérequis : Appium installé et démarré, émulateur Android lancé
    appium

    # Dans un autre terminal
    robot test.robot

Les rapports report.html, log.html et output.xml sont générés automatiquement après chaque exécution (ils ne sont pas versionnés).

## Autrice

Soumia Sadki — Testeuse QA junior · [LinkedIn](https://www.linkedin.com/in/soumia-sadki/)
