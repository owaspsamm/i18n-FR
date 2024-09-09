---
title: Organisation et Culture
type: stream
url: ./model/governance/education-and-guidance/stream-b/
business_function: Gouvernance
business_function_url: governance
practice: Éducation & Orientation
stream: B
description: Gouvernance / Éducation & Orientation
keywords: ["Business function", "Practice", "Gouvernance", "Éducation & Orientation"]
aliases:
    - /fr/model/G-EG-B-1
    - /fr/model/G-EG-B-2
    - /fr/model/G-EG-B-3
    - /fr/model/G-EG-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Intégration de premier niveau de la sécurité dans l'organisation de développement
        activity: |
            Implémentez un programme où chaque équipe de développement de logiciels a un membre considéré comme un « Champion de la sécurité » qui fait le lien entre la Sécurité de l'Information et les développeurs. Selon la taille et la structure de l’équipe, le « Champion de la sécurité » peut être un développeur, un testeur ou un gestionnaire de produits. Le « Champion de la sécurité » dispose d'un nombre déterminé d’heures par semaine pour les activités liées à la sécurité de l’information. Il participe à des réunions périodiques pour accroître la sensibilisation et l'expertise dans différentes disciplines de la sécurité. Les « Champions de la sécurité » suivent des formations supplémentaires pour les aider à se développer en tant qu’experts en matière de sécurité logicielle. Vous devrez peut-être personnaliser la façon dont vous créez les rôles de « Champion de la sécurité » et les incluez dans la hiérarchie pour des raisons culturelles.

            Les objectifs de la fonction sont d'augmenter l'efficacité opérationnelle de la sécurité et de la conformité applicatives et de renforcer la relation entre les différentes équipes et la Sécurité de l'Information. Pour atteindre ces objectifs, les « Champion de la sécurité » aident à la recherche, à la validation et à l'affectation de priorités aux défauts logiciels liés à la sécurité et à la conformité. Ils sont impliqués dans toutes les évaluations des risques, les évaluations des menaces, et revues d'architecture pour aider à identifier les possibilités de corriger les défauts de sécurité en rendant l'architecture de l'application plus résiliente et en réduisant la menace sur la surface de d'attaque.

            En plus d'apporter un soutien à la Sécurité de l'Information, les « Champions de la sécurité » fournissent périodiquement des informations à propos de toutes les questions liées à la sécurité à l’équipe projet afin que tout le monde soit conscient des problèmes et des efforts d'amélioration actuels et futurs. Ces revues sont mises à profit pour aider à la résolution de problèmes plus complexes en engageant toute l'équipe de développement.

        question: Avez-vous identifié un Champion de Sécurité pour chaque équipe de développement?
        quality_criteria:
            - Les Champions de Sécurité reçoivent une formation appropriée
            - Les équipes de sécurité et de développement des applications reçoivent des informations périodiquement de la part des champions de sécurité sur l'état général des initiatives et des correctifs de sécurité
            - Le Champion de la Sécurité revoie les résultats des tests effectués en externe avant de les ajouter au backlog de l'application

        answers:
            - "No"
            - Oui, pour certaines équipes
            - Oui, pour au moins la moitié des équipes
            - Oui, pour la plupart ou toutes les équipes

    level2:
        level: 2
        benefit: |
            Bonnes pratiques de sécurité spécifiques adaptées à l'organisation
        activity: |
            L'organisation met en place un centre d'excellence pour le développement sécurisé, avec des architectes et des développeurs expérimentés représentant les différentes lignes d'affaires et les piles technologique. L'équipe a une charte officielle et définit les normes et les bonnes pratiques pour l'amélioration des pratiques de développement de logiciels. L'objectif est d'atténuer la difficulté pour les professionnels de la sécurité de l'information liée à la vitesse des changements dans la technologie, les langages de programmation et les environnements de développement et les bibliothèques associées d'être pleinement informés de toutes les nuances techniques qui ont un impact sur la sécurité. Même les développeurs ont souvent du mal à suivre tous les changements et les nouveaux outils destinés à rendre le développement de logiciels plus rapide, meilleur et plus sûr.

            Ceci garantit que tous les efforts de programmation actuels suivent les bonnes pratiques de l'industrie et que les normes de développement et de mise en œuvre de l'organisation incluent tous les paramètres de configuration critiques. Ceci aide à identifier, former et soutenir les « Champions de produits », responsable d'aider les différentes équipes à implémenter les outils qui automatisent, rationalisent ou améliorent différents aspects du SDLC. Ceci identifie les équipes de développement avec des niveaux de maturité plus élevés au sein de leur SDLC et les pratiques et outils qui permettent ces réalisations, dans le but de les reproduire pour d'autres équipes.

            Le groupe fournit une expertise en la matière, en aidant les équipes de sécurité de l'information à évaluer les outils et les solutions pour améliorer la sécurité des applications et en s'assurant que ces outils sont non seulement utiles mais aussi compatibles avec la façon dont différentes équipes développent des applications. Les équipes cherchant à apporter des changements architecturaux significatifs à leur logiciel consultent ce groupe pour éviter d'avoir un impact négatif sur le SDLC ou sur les contrôles de sécurité en place.

        question: L'organisation dispose-t-elle d'un centre d'excellence en logiciel sécurisé (SSCE)?
        quality_criteria:
            - Le SSCE a une charte définissant son rôle dans l'organisation
            - Les équipes de développement passent en revue tous les changements architecturaux importants avec le SSCE
            - Le SSCE publie les normes et les directives liées au SDLC relatives à la sécurité applicative
            - Les Champions Produit sont responsables de la promotion de l'utilisation d'outils de sécurité spécifiques

        answers:
            - "No"
            - Oui, nous avons commencé à l'implémenter
            - Oui, pour une partie de l'organisation
            - Oui, pour toute l'organisation

    level3:
        level: 3
        benefit: |
            Développement collectif du savoir-faire en matière de sécurité parmi toutes les équipes de produits
        activity: |
            La sécurité est la responsabilité de tous les employés, pas seulement de l'équipe de la sécurité de l'information. Déployez des plateformes de communication et de partage des connaissances pour aider les développeurs à construire des communautés autour de différentes technologies, outils et langages de programmation. Dans ces communautés, les employés partagent des informations, discutent des problèmes avec d'autres développeurs et font des recherches dans la base de connaissances pour trouver des réponses à des questions discutées précédemment.

            Formez des communautés autour des rôles et des responsabilités et permettez aux développeurs et aux ingénieurs de différentes équipes et unités commerciales de communiquer librement et de bénéficier de l'expertise de chacun. Encouragez la participation et mettez en place un programme pour promouvoir ceux qui aident le plus de collaborateurs en tant que leaders de pensée et faites en sorte que le management les reconnaisse. En plus d'améliorer la sécurité des applications, cette plateforme peut aider à identifier les futurs membres du Centre d'Excellence en Sécurité Logicielle, ou « Champion de la sécurité », en fonction de leur expertise et de leur volonté d'aider les autres.

            Les équipes du Centre d'Excellence en Sécurité Logicielle et de la Sécurité des Applications examinent régulièrement le portail d'information pour avoir un aperçu des nouvelles technologies et de celles à venir, ainsi que des occasions d'aider la communauté du développement par de nouvelles initiatives, outils, programmes et ressources de formation. Utilisez le portail pour diffuser des informations sur les nouvelles normes, outils et ressources vers tous les développeurs afin d'améliorer continuellement la maturité du SDLC et la sécurité des applications.

        question: Existe-t-il un portail centralisé où les développeurs et les professionnels de la sécurité des applications de différentes équipes et unités opérationnelles peuvent communiquer et partager des informations ?
        quality_criteria:
            - L'organisation promeut l'utilisation d'un portail unique entre différentes équipes et unités commerciales
            - Le portail est utilisé pour diffuser des informations en temps utile telles que la notification d'incidents de sécurité, les mises à jour d'outils, les changements de normes architecturales et autres annonces connexes
            - Le portail est largement reconnu par les développeurs et les architectes en tant que référentiel central des informations de sécurité des applications spécifiques à l'organisation
            - Tout le contenu est considéré comme étant persistant et interrogeable
            - Le portail fournit un accès aux métriques de sécurité spécifiques à une application

        answers:
            - "No"
            - Oui, nous avons commencé à l'implémenter
            - Oui, pour une partie de l'organisation
            - Oui, pour toute l'organisation

---
