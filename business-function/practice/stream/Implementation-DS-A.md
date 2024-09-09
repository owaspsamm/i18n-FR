---
title: Processus de Déploiement
type: stream
url: ./model/implementation/secure-deployment/stream-a/
business_function: Implémentation
business_function_url: implementation
practice: Déploiement Sécurisé
stream: A
description: Implémentation / Déploiement Sécurisé
keywords: ["Business function", "Practice", "Implémentation", "Déploiement Sécurisé"]
aliases:
    - /fr/model/I-SD-A-1
    - /fr/model/I-SD-A-2
    - /fr/model/I-SD-A-3
    - /fr/model/I-SD-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Un risque limité d'erreur humaine pendant le processus de déploiement minimisant les problèmes de sécurité
        activity: |
            Définissez toutes les étapes du processus de déploiement et découpez-le en un ensemble d'instructions claires devant être suivies soit par une personne, soit par un outillage automatisé. La définition du processus de déploiement devrait porter sur l'ensemble du processus de bout en bout afin qu'il puisse être suivi de façon cohérente à chaque fois et produise le même résultat. La définition est stockée de façon centralisée et est accessible à tout le personnel concerné. Ne stockez pas ou ne distribuez pas de multiples copies, certaines pouvant devenir obsolètes.

            Déployez les applications en production soit en utilisant un processus automatisé, soit manuellement par un personnel autre que les développeurs. Assurez-vous que les développeurs n'ont pas besoin d'un accès direct à l'environnement de production pour le déploiement d'applications.

            Examinez tous les outils de déploiement en veillant à ce qu'ils soient activement maintenus par les vendeurs et à jour avec les derniers correctifs de sécurité. Durcissez la configuration de chaque outil pour qu'il soit aligné avec les conseils des fournisseurs et avec les bonnes pratiques de l'industrie. Étant donné que la plupart de ces outils nécessitent un accès à l'environnement de production, leur sécurité est extrêmement critique. Assurez l'intégrité des outils eux-mêmes et des flux de travail qu'ils suivent, et configurez des règles d'accès à ces outils selon le principe des moindres privilèges.

            Faites en sorte que le personnel ayant accès à l'environnement de production reçoive un minimum de formation ou de certification pour garantir leurs compétences en la matière.

        question: Utilisez-vous des processus de déploiement reproductibles?
        quality_criteria:
            - Vous avez assez d'informations pour exécuter les processus de déploiement
            - Votre documentation de déploiement est à jour
            - Votre documentation de déploiement est accessible aux parties prenantes concernées
            - Vous vous assurez que seul un personnel qualifié identifié peut déclencher un déploiement
            - Vous durcissez les outils utilisés dans le processus de déploiement

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Un processus de déploiement efficace avec des outils de sécurité intégrés
        activity: |
            Automatisez le processus de déploiement pour couvrir les différentes étapes, de sorte qu'aucune étape de configuration manuelle n'est nécessaire et que le risque d'erreur humaine isolée est éliminé. Assurez-vous et vérifiez que le déploiement est cohérent à travers toutes les étapes.

            Intégrez des vérifications de sécurité automatisées dans votre processus de déploiement, par ex. en utilisant des outils de test de sécurité d'analyse dynamique (DAST) et d'analyse de vulnérabilité. Vérifiez également l'intégrité des artefacts déployés là où cela a du sens. Enregistrez les résultats de ces tests de manière centralisée et prenez toutes les actions nécessaires. Assurez-vous que, dans le cas où des défauts seraient détectés, le personnel concerné est informé automatiquement. Dans le cas où des problèmes dépassant le niveau critique prédéfini sont identifiés, stoppez ou inversez le déploiement automatiquement, ou introduisez un flux d'approbation manuel séparé afin que la décision de déployer soit enregistrée, avec une explication de l'exception.

            Comptabilisez et auditez tous les déploiements à toutes les étapes. Ayez un système en place pour enregistrer chaque déploiement, y compris les informations sur qui l'a mené, la version du logiciel qui a été déployée, ainsi que toutes les variables pertinentes spécifiques au déploiement.

        question: Les processus de déploiement sont-ils automatisés et utilisent-ils des contrôles de sécurité?
        quality_criteria:
            - Les processus de déploiement sont automatisés à toutes les étapes
            - Le déploiement comprend des procédures de test de sécurité automatisées
            - Vous alertez le personnel responsable des vulnérabilités identifiées
            - Vous avez des logs disponibles pour vos déploiements passés pour une période de temps définie

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Assurer l'intégrité des artefacts qui vont être déployés en production
        activity: |
            Tirez parti de la signature de binaires au moment de la génération et incluez une vérification automatique de l'intégrité du logiciel déployé en vérifiant ses signatures par rapport aux certificats de confiance. Cela peut inclure des binaires développés et générés en interne, ainsi que des artefacts tiers. Ne déployez pas d'artefact dont la signature ne peut pas être vérifiée, y compris ceux dont les certificats sont invalides ou ont expiré.

            Si la liste des certificats de confiance inclut ceux de développeurs tiers, vérifiez-les périodiquement et de les maintenez leur conformité avec la gouvernance générale de l’organisation concernant les fournisseurs tiers de confiance.

            Approuvez manuellement le déploiement au moins une fois lors d'un déploiement automatisé. Chaque fois qu'un test humain est beaucoup plus précis qu'un test automatisé pendant le déploiement, optez pour cette option.

        question: Validez-vous de façon cohérente l'intégrité des artefacts déployés ?
        quality_criteria:
            - Vous empêchez ou annulez le déploiement si vous détectez une rupture d'intégrité
            - La vérification est faite en utilisant des signatures créées pendant la phase de génération
            - Si la vérification des signatures n'est pas possible (par exemple dans le cas d'un logiciel généré en externe), vous introduisez des mesures compensatoires

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
