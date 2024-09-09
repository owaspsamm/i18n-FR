---
title: Durcissement de la Configuration
type: stream
url: ./model/operations/environment-management/stream-a/
business_function: Opérations
business_function_url: operations
practice: Gestion de l'environnement
stream: A
description: Opérations / Gestion de l'environnement
keywords: ["Business function", "Practice", "Opérations", "Gestion de l'environnement"]
aliases:
    - /fr/model/O-EM-A-1
    - /fr/model/O-EM-A-2
    - /fr/model/O-EM-A-3
    - /fr/model/O-EM-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Paramètres de configuration de base durcis de vos composants
        activity: |
            En vous basant sur votre bonne compréhension de l'importance de sécuriser les piles technologiques que vous utilisez, appliquez une configuration sécurisée aux éléments des piles en vous basant sur les directives disponibles (par ex., projets en source ouverte, documentation des fournisseurs, articles de blogs). Quand vos équipes développent des conseils sur la bonne configuration de leurs applications basés sur leurs diverses tentatives et sur les informations recueillies par les membres de l'équipe, encouragez-les à partager leurs connaissances dans toute l'organisation.

            Identifiez les éléments clés des piles technologiques communes et établissez des normes de configuration pour celles-ci, en vous basant sur les expériences des équipes de ce qui fonctionne.

            À ce niveau de maturité, vous n'avez pas encore de processus formel pour la gestion des bases de référence des configurations. Les configurations peuvent ne pas être appliquées de manière uniforme à travers les applications et les déploiements, et le suivi de la conformité est probablement absent.

        question: Durcissez-vous les configurations des composants clés de vos piles technologiques?
        quality_criteria:
            - Vous avez identifié les composants clés de chaque pile technologique utilisée
            - Vous avez un standard de configuration établi pour chaque composant clé

        answers:
            - Non
            - Oui, pour certains composants
            - Oui, pour au moins la moitié des composants
            - Oui, pour la plupart ou pour tous les composants

    level2:
        level: 2
        benefit: |
            Durcissement cohérent des composants de la pile technologique au sein de votre organisation
        activity: |
            Etablissez une ligne de référence de durcissement pour l'ensemble des composants de chaque pile technologique utilisée. Pour garantir une application cohérente des lignes de référence de durcissement, développez des guides de configuration pour les composants. Exigez que les équipes produits appliquent les lignes de référence de configuration à tous les nouveaux systèmes, ainsi qu'aux systèmes existants lorsque cela est faisable.

            Mettez les bases de réference de durcissement et les guides de configuration sous gestion de version et affectez un propriétaire à chacun. Les propriétaires ont la responsabilité permanente de les tenir à jour, en fonction de l'évolution des bonnes pratiques ou des changements apportés aux composants pertinents (par exemple, mises à jour des versions, nouvelles fonctionnalités).

            Dans des environnements plus larges, dérivez les configurations d'instances à partir d'une référence maintenue localement, avec les bases de référence pertinentes aux configuration appliquées. Employez des outils automatisés pour durcir les configurations.

        question: Avez-vous des références minimales de durcissement pour vos composants?
        quality_criteria:
            - Vous avez assigné un propriétaire pour chaque référence minimale
            - Le propriétaire maintient à jour les références minimales dont il a la charge
            - Vous stockez les références minimales dans un emplacement accessible
            - Vous formez les employés responsables des configurations à ces références minimales

        answers:
            - Non
            - Oui, pour certains composants
            - Oui, pour au moins la moitié des composants
            - Oui, pour la plupart ou pour tous les composants

    level3:
        level: 3
        benefit: |
            Transparence sur les configurations des composants pour éviter les non-conformités
        activity: |
            Surveillez activement les configurations de sécurité des piles de technologies déployées en effectuant des vérifications régulières par rapport aux niveaux de référence établis. Assurez-vous que les résultats des vérifications de configuration sont facilement disponibles par le biais de publications et de tableaux de bord.

            Lorsque vous détectez des configurations non conformes, traitez chaque occurrence comme une trouvaille liée à la sécurité et gérez les actions correctives au sein de votre pratique en place de gestion des défauts.

            D'autres améliorations peuvent être réalisées à l'aide de mesures automatisées, telles que des configurations d'"auto-guérison" et des alertes d'information sur la sécurité et la gestion d'événements (SIEM).

            Dans le cadre du processus de mise à jour des composants (par ex. les nouvelles versions, les correctifs venant du fournisseur), révisez les lignes de référence et les guides de configuration correspondants, mettez-les à jour si nécessaire pour maintenir leur pertinence et leur exactitude. Réexaminez les autres lignes de référence et guides de configuration au moins une fois par an.

            Réexaminez périodiquement votre processus de gestion des lignes de référence, en incorporant les retours et les leçons tirées des équipes qui appliquent et maintiennent les lignes de référence de configuration et les guides de configuration.

        question: Surveillez-vous et contrôlez-vous la conformité avec les références minimales de durcissement ?
        quality_criteria:
            - Vous effectuez des contrôles de conformité régulièrement, de préférence en utilisant l'automatisation
            - Vous stockez les résultats de la vérification de conformité dans un endroit accessible
            - Vous suivez un processus établi pour traiter les non-conformités signalées
            - Vous réexaminez chaque référence minimale au moins une fois par an et vous la mettez à jour lorsque cela est nécessaire

        answers:
            - Non
            - Oui, pour certains composants
            - Oui, pour au moins la moitié des composants
            - Oui, pour la plupart ou pour tous les composants

---
