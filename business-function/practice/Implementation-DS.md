---
title: Déploiement Sécurisé
url: ./model/implementation/secure-deployment/
business_function: "Implémentation"
business_function_url: "implementation"
keywords: ["Business function", "Practice", "Déploiement Sécurisé"]
aliases:
    - /fr/model/I-SD
type: practice

practice_maturity_1_description: Les processus de déploiement sont entièrement documentés.
practice_maturity_2_description: Les processus de déploiement comprennent la vérification de sécurité des jalons.
practice_maturity_3_description: Le processus de déploiement est entièrement automatisé et intègre la vérification automatisée de tous les jalons essentiels.

stream_a: Processus de Déploiement

stream_a_maturity_1_activity: Formaliser le processus de déploiement et sécuriser les outils et les processus utilisés.
stream_a_maturity_2_activity: Automatiser le processus de déploiement à toutes les étapes et introduire des tests de vérification de la sécurité raisonnables.
stream_a_maturity_3_activity: Vérifier automatiquement l'intégrité de tous les logiciels déployés, indépendamment du fait qu'ils ont été développés en interne ou en externe.

stream_b: Gestion des Secrets

stream_b_maturity_1_activity: Introduire des mesures de protection de base pour limiter l'accès à vos secrets de production.
stream_b_maturity_2_activity: Injecter dynamiquement les secrets lors du processus de déploiement à partir de stockages durcis et auditer tout accès humain à ceux-ci.
stream_b_maturity_3_activity: Améliorer le cycle de vie des secrets d'application en les générant régulièrement et en en garantissant une utilisation appropriée.
---

L'une des dernières étapes de la fourniture de logiciels sécurisés est de garantir que la sécurité et l'intégrité des applications développées ne sont pas compromises lors du déploiement. La pratique du Déploiement Sécurisé (DS) se focalise sur ce point. À cette fin, le premier flux de la pratique se concentre sur la suppression des erreurs manuelles en automatisant le processus de déploiement autant que possible et en conditionnant son succès aux résultats des vérifications de sécurité intégrées. Il favorise également la séparation des pouvoirs en rendant des non-développeurs dûment formés responsables du déploiement.

Le second flux va au-delà de la mécanique du déploiement et se concentre sur la protection de la vie privée et de l'intégrité des données sensibles, tels que mots de passe, jetons et autres secrets, requis pour que les applications puissent fonctionner dans des environnements de production. Sous sa forme la plus simple, les secrets de production concernés sont déplacés depuis les dépôts et des fichiers de configuration vers des coffres numériques dûment gérés. Dans des formes plus élaborées, les secrets sont générés dynamiquement au moment du déploiement et des processus dédiés détectent et atténuent la présence de tout secret non protégé dans l'environnement.

