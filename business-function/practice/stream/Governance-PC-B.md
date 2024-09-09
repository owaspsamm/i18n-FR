---
title: Gestion de la Conformité
type: stream
url: ./model/governance/policy-compliance/stream-b/
business_function: Gouvernance
business_function_url: governance
practice: Politique & Conformité
stream: B
description: Gouvernance / Politique & Conformité
keywords: ["Business function", "Practice", "Gouvernance", "Politique & Conformité"]
aliases:
    - /fr/model/G-PC-B-1
    - /fr/model/G-PC-B-2
    - /fr/model/G-PC-B-3
    - /fr/model/G-PC-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Politiques et normes de sécurité en phase avec les facteurs de conformité externes
        activity: |
            Créez une liste complète de toutes les exigences de conformité, y compris les déclencheurs qui pourraient aider à déterminer quelles applications sont concernées. Les exigences de conformité peuvent s'appliquer en fonction de facteurs tels que l'emplacement géographique, les types de données ou les obligations contractuelles avec les clients ou les partenaires commerciaux. Examinez chaque exigence de conformité identifiée avec les experts compétents et le département en charge des aspects législatifs afin de s'assurer que cette obligation est comprise. Étant donné que de nombreuses obligations de conformité varient en fonction de la manière dont les données sont traitées, stockées ou transmises à travers l'environnement informatique, les facteurs de conformité devraient toujours indiquer les possibilités de réduire la charge globale de conformité en modifiant la façon dont les données sont manipulées.

            Envisagez la publication d'une matrice de conformité pour aider à identifier quels facteurs pourraient déclencher une exigence réglementaire spécifique pour une application donnée. Faites en sorte que la matrice indique quelles exigences de conformité s'appliquent au niveau de l'organisation et non au niveau d'une application donnée. La matrice fournit au moins une compréhension de base des exigences de conformité utiles pour examiner les obligations entourant différentes applications.

            Étant donné que de nombreuses normes de conformité sont axées sur les bonnes pratiques de sécurité, il est possible que de nombreuses exigences en matière de conformité fassent déjà partie de la bibliothèque de politique et de normes publiée par l'organisation. Par conséquent, une fois que vous avez examiné les exigences de conformité, mettez-les en correspondance avec les politiques et normes existantes applicables. Lorsqu’il y a des divergences, mettez à jour les politiques et les normes pour inclure les exigences de conformité à l’échelle de l’organisme. Puis seulement, commencez à créer des normes spécifiques de conformité qui ne s’appliquent qu’aux exigences individuelles de conformité. L'objectif est d'avoir une matrice de conformité qui indique quelles politiques et normes ont des informations plus détaillées sur les exigences de conformité. en plus de veiller à ce que les politiques et les normes individuelles fassent référence aux exigences de conformité applicables.

        question: Avez-vous une image complète de vos obligations de conformité externe?
        quality_criteria:
            - Vous avez identifié toutes les sources d'obligations de conformité externe
            - Vous avez capturé et harmonisé les obligations de conformité depuis toutes les sources

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Compréhension partagée avec les équipes produit de la manière d'être en conformité avec les facteurs externes
        activity: |
            Élaborez une bibliothèque d'exigences d'application et de scripts de tests afin d'établir et de vérifier la conformité réglementaire des applications. Certaines d'entre elles sont liées à des exigences de conformité ciblées telles qu'au PCI ou au RGPD, alors que d'autres sont de nature plus générale et répondent à des exigences de portée mondiale en matière de conformité telles que l'ISO. La bibliothèque est disponible à toutes les équipes de développement d'applications. Elle comprend des conseils pour déterminer toutes les exigences applicables, y compris les considérations visant à réduire la charge et la portée de la conformité. Mettez en œuvre un processus pour réévaluer périodiquement les exigences de conformité de chaque application. La nouvelle évaluation comprend l’examen de toutes les fonctionnalités de l’application et les possibilités de réduire la portée afin de minimiser le coût global de la conformité.

            Les exigences incluent suffisamment d'informations pour que les développeurs comprennent les exigences fonctionnelles et non-fonctionnelles des différentes obligations de conformité. Elles contiennent des références aux politiques et aux normes et font explicitement référence à la réglementation. S'il reste des interrogations au sujet de la mise en œuvre d'une exigence particulière, le texte original du règlement peut aider à interpréter l'exigence de manière plus précise. Chaque exigence comprend un ensemble de scripts de test pour vérifier la conformité. En plus de permettre à l'Assurance Qualité de faciliter la vérification de la conformité, ils peuvent aider à clarifier les exigences de conformité pour les développeurs et à rendre le processus de conformité transparent. Les exigences ont un format qui permet de les importer dans les référentiels individuels d'exigences. Clarifiez davantage pour les développeurs les exigences de conformité et veillez à ce que le processus de conformité soit totalement transparent.

        question: Avez-vous un ensemble standard d'exigences de sécurité et de procédures de vérification qui traitent des obligations externes de conformité de l'organisation?
        quality_criteria:
            - Vous associez chaque obligation de conformité externe à un ensemble bien défini d'exigences applicatives
            - Vous définissez des procédures de vérification, y compris des tests automatiques, pour vérifier la conformité aux exigences de conformité

        answers:
            - "No"
            - Oui, pour certaines obligations
            - Oui, pour au moins la moitié des obligations
            - Oui, pour la plupart ou toutes les obligations

    level3:
        level: 3
        benefit: |
            Comprendre la conformité de votre organisation avec les facteurs externes
        activity: |
            Élaborez un programme de mesure et d'établissement de rapport sur l'état de la conformité entre les différentes applications. Les exigences des application et les scripts de test aident à déterminer le statut de la conformité. Tirez parti de l'automatisation des tests pour détecter rapidement les régressions dans la conformité des applications fréquemment mises à jour et assurez-vous que la conformité est maintenue à travers les différentes versions des applications. Chaque fois que les tests entièrement automatisés ne sont pas envisageables, les équipes d'assurance qualité, d'audit interne ou de sécurité de l'information évaluent périodiquement la conformité grâce à une combinaison de tests manuels et d'entrevues.

            Tandis que la conformité totale est toujours l'objectif ultime, incluez le suivi des actions de correction et des mises à jour périodiques dans le programme. Examinez périodiquement les activités d'amélioration de la conformité pour vérifier que les équipes progressent de façon appropriée et que les stratégies de corection seront efficaces pour atteindre la conformité. Pour améliorer davantage le processus, élaborez une série de rapports types et de fiches d'évaluation de la conformité. Ces mesures aident les différentes équipes à comprendre l’état actuel de la conformité et l’organisation à gérer plus efficacement l’aide pour combler les lacunes en matière de conformité.

            Examinez les écarts par rapport à la conformité nécessitant des dépenses ou un développement importants avec les experts en la matière et comparez-les au coût lié à la réduction des fonctionnalités de l'application, à la réduction du périmètre ou à la suppression des exigences de conformité. Les écarts à long terme en matière de conformité requièrent une approbation du management et une acceptation formelle des risques liés à la conformité, de sorte qu’ils reçoivent l’attention appropriée de la part de la direction de l’organisation.

        question: Faites-vous une analyse régulière du respect des obligations de conformité externes et utilisez-vous cette information pour guider les efforts visant à combler les lacunes en matière de conformité?
        quality_criteria:
            - Vous avez des métriques établis et bien définis de conformité
            - Vous mesurez et partagez régulièrement les métriques de conformité des applications
            - Les parties prenantes utilisent les informations remontées sur l'état de conformité pour identifier les lacunes en matière de conformité et mettre des priorités sur les actions de réduction des écarts

        answers:
            - "No"
            - Oui, mais la remontée d'information est ad-hoc
            - Oui, nous remontons les informations régulièrement
            - Oui, nous remontons les informations au moins une fois par an

---
