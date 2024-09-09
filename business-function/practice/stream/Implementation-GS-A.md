---
title: Processus de Génération
type: stream
url: ./model/implementation/secure-build/stream-a/
business_function: Implémentation
business_function_url: implementation
practice: Génération Sécurisée
stream: A
description: Implémentation / Génération Sécurisée
keywords: ["Business function", "Practice", "Implémentation", "Génération Sécurisée"]
aliases:
    - /fr/model/I-SB-A-1
    - /fr/model/I-SB-A-2
    - /fr/model/I-SB-A-3
    - /fr/model/I-SB-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Un risque limité d'erreur humaine lors du process de génération minimisant les problèmes de sécurité
        activity: |
            Définissez le processus de génération en le divisant en un ensemble d'instructions claires devant être suivies soit par une personne, soit par un outil automatisé. La définition du processus de génération décrit l'ensemble du processus de bout en bout afin que la personne ou l'outil puisse le suivre de façon cohérente chaque fois et produise le même résultat. La définition est stockée de façon centralisée et est accessible à tous les outils ou personnes concernées. Évitez d'en stocker plusieurs copies car elles peuvent devenir incohérentes ou périmées.

            La définition du processus n'inclut aucun secret (particulièrement ceux nécessaires pendant le processus de génération).

            Examinez tous les outils de génération en veillant à ce qu'ils soient activement maintenus par les fournisseurs et à jour avec les derniers correctifs de sécurité. Durcissez la configuration de chaque outil pour qu'il soit aligné avec les conseils des fournisseurs et les bonnes pratiques de l'industrie.

            Détermine une valeur pour chaque artefact générépour l'utiliser ultérieurement pour vérifier son intégrité, comme une signature ou une valeur de hachage. Protégez cette valeur et, si l'artefact est signé, le certificat privé de signature .

            Assurez-vous que les outils de génération sont régulièrement mis à jour et correctement durcis.

        question: Votre processus complet de génération est-il formellement décrit?
        quality_criteria:
            - Vous avez assez d'informations pour recréer les processus de génération
            - Votre documentation sur la génération est à jour
            - Votre documentation de la génération est stockée dans un emplacement accessible
            - Des sommes de contrôle sur les artefacts produits sont créées pendant la génération pour permettre une vérification ultérieure
            - Vous durcissez les outils utilisés lors du processus de génération

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Un processus de génération efficace avec des outils de sécurité intégrés
        activity: |
            Automatisez le processus de génération pour que les compilations puissent être exécutées de manière cohérente à tout moment. Le processus de génération ne devrait généralement nécessiter aucune intervention, réduisant encore la probabilité d'erreurs humaines.

            L'utilisation d'un système automatisé augmente la dépendance à la sécurité des outils de génération et rend le durcissement et le maintien des outils encore plus critique. Portez une attention particulière aux interfaces de ces outils, telles que les portails web et la façon dont ils peuvent être verrouillés. L'exposition d'un outil de génération au réseau pourrait permettre à un acteur malveillant d'altérer l'intégrité du processus. Cela pourrait permettre, par exemple, d'intégrer du code malveillant dans un logiciel.

            Le processus automatisé peut avoir besoin d'accéder à des informations d'identification et à des secrets requis pour construire le logiciel, tels que le certificat de signature de code ou à certains répertoires. Gérez cela avec précaution. Signez les artefacts générés en utilisant un certificat qui identifie l'organisation ou l'unité commerciale qui l'a construit, afin que vous puissiez vérifier l'intégrité.

            Enfin, ajoutez des vérifications de sécurité automatisées appropriées (par exemple en utilisant des outils SAST) dans la chaîne afin de tirer parti de l'automatisation et des avantages liés à la sécurité.

        question: Le processus de génération est-il entièrement automatisé ?
        quality_criteria:
            - Le processus de génération à proprement parler ne nécessite aucune interaction humaine
            - Vos outils de génération sont durcis conformément aux bonnes pratiques et aux conseils du fournisseur
            - Vous chiffrez les secrets requis par les outils de génération et contrôlez les accès selon le principe du moindre privilège

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Garantie que le logiciel généré est conforme aux niveaux de référence de sécurité
        activity: |
            Définissez des contrôles de sécurité appropriés à effectuer pendant le processus de génération, ainsi que des critères minimums pour passer la génération- ceux-ci peuvent différer selon les profils de risque des différentes applications. Incluez les vérifications de sécurité respectives dans la génération et imposez la fin de son processus au cas où les critères prédéfinis ne seraient pas respectés. Déclenchez des avertissements pour les problèmes en dessous du seuil et enregistrez-les dans un système centralisé pour les suivre et prendre des mesures. Si c'est raisonnable, implémentez un mécanisme d'exception pour contourner ce comportement si le risque d'une vulnérabilité particulière a été accepté ou atténué. Toutefois, assurez-vous que ces cas sont approuvés de façon explicite avant tout et consignez leur occurrence avec une justification.

            Si des limitations techniques empêchent l'organisation d'arrêter la génération automatiquement, assurez les mêmes effets par le biais d'autres mesures telles qu'une politique claire et un audit régulier.

            Gérez la signature de code sur un serveur centralisé séparé qui n'expose pas le certificat au système exécutant la génération. Dans la mesure du possible, utilisez une méthode déterministe qui produit des artefacts reproductibles octet par octet.

        question: Avez-vous mis en place des contrôles de sécurité automatisés dans vos processus de génération?
        quality_criteria:
            - La génération échoue si l'application ne répond pas à une référence minimale de sécurité prédéfinie
            - Vous avez défini une sévérité maximale pour les vulnérabilités
            - Vous enregistrez les avertissements et les échecs dans un système centralisé
            - Vous sélectionnez et configurez les outils pour évaluer chaque application par rapport à ses exigences de sécurité au moins une fois par an

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
