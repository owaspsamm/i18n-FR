---
title: Exigences Logicielles
type: stream
url: ./model/design/security-requirements/stream-a/
business_function: Conception
business_function_url: design
practice: Exigences de Sécurité
stream: A
description: Conception / Exigences de Sécurité
keywords: ["Business function", "Practice", "Conception", "Exigences de Sécurité"]
aliases:
    - /fr/model/D-SR-A-1
    - /fr/model/D-SR-A-2
    - /fr/model/D-SR-A-3
    - /fr/model/D-SR-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Comprendre les principales exigences de sécurité lors du développement
        activity: |
            Effectuez un examen des exigences fonctionnelles du projet logiciel. Identifier les exigences de sécurité pertinentes (c.a.d. les attentes) pour cette fonctionnalité en raisonnant par rapport au niveau de confidentialité, d'intégrité ou de disponibilité souhaité du service ou des données apportées par le projet logiciel. Les exigences précisent l'objectif (p. ex. “Les données personnelles du processus d’enregistrement devraient être transférées et stockées de façon sécurisée”), mais pas le moyen réel pour atteindre cet objectif (p. ex., « utiliser TLSv1.2 pour un transfert sécurisé »).

            En même temps, passez en revue les fonctionnalités du point de vue de l'attaquant pour comprendre comment elles pourraient être détournées. De cette façon, vous pouvez identifier des exigences de protection supplémentaires pour le projet logiciel considéré.

            Les objectifs de sécurité peuvent être liés à des fonctionnalités de sécurité spécifiques que vous devez ajouter à l'application (p. ex., « Identifier l’utilisateur de l’application en tout temps ») ou à la qualité et au comportement global de l’application (p. ex., « Veiller à ce que les données personnelles soient correctement protégées en transit »), ce qui ne conduit pas nécessairement à de nouvelles fonctionnalités. Suivez les bonnes pratiques d'écriture des exigences de sécurité. Rendez-les spécifiques, mesurables, opérationnelles, pertinentes et bornées en durée (SMART). Faites attention à ne pas ajouter des exigences trop générales qui ne se rapporteraient pas à l’application considérée (par ex. L’application devrait apporter des protections contre le Top 10 de l’OWASP). Bien qu’elles puissent être vraies, elles n’apportent pas de valeur à la discussion.

        question: Les équipes projet spécifient-elles les exigences de sécurité durant le développement ?
        quality_criteria:
            - Les équipes dérivent les exigences de sécurité des exigences fonctionnelles et des préoccupations du client ou de l'organisation
            - Les exigences de sécurité sont spécifiques, mesurables et raisonnables
            - Les exigences de sécurité sont conformes aux exigences minimales organisationnelles

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Alignement des exigences de sécurité avec d'autres types d'exigences
        activity: |
            Les exigences de sécurité peuvent provenir d'autres sources, y compris les politiques et la législation, les problèmes connus au sein de l'application, et les enseignements provenant des métriques et des retours de terrain. À ce niveau, une élicitation plus systématique des exigences de sécurité doit être obtenue en analysant différentes sources de ces exigences. Veiller à ce que ces sources fournissent des intrants appropriés pour faciliter l'élicitation des exigences. Par exemple, organisez des entretiens ou des séances de créativité (par exemple dans le cadre de la politique et de la législation), analysez les historiques des journaux ou des systèmes de vulnérabilité.

            Utilisez une notation structurée des exigences de sécurité à travers les applications et un formalisme approprié qui s'intègre bien à la façon dont vous spécifiez d'autres exigences (fonctionnelles) pour le projet. Cela peut signifier, par exemple, étendre les documents d'analyse, écrire des récits, etc.

            Lorsque des exigences sont spécifiées, il est important de s'assurer que ces exigences sont prises en compte lors du développement de produits. Mettez en place un mécanisme pour stimuler ou obliger les équipes projet à répondre à ces exigences dans le produit. Par exemple, annotez les exigences avec des priorités, ou influencez le traitement des exigences pour faire respecter un appétit de sécurité suffisant (tout en respectant l'équilibre avec les autres exigences non fonctionnelles).

        question: Définissez-vous, structurez-vous et incluez-vous la gestion des priorités dans les artefacts du processus de collecte des exigences de sécurité?
        quality_criteria:
            - Les exigences de sécurité tiennent compte des connaissances spécifiques au domaine lors de l'application des politiques et des orientations au développement de produits
            - Des experts du domaine sont impliqués dans le processus de définition des exigences
            - Vous avez une notation structurée validée concernant les exigences de sécurité
            - Les équipes de développement ont un champion de sécurité dédié à l'examen des exigences et des résultats en matière de sécurité

        answers:
            - "No"
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

    level3:
        level: 3
        benefit: |
            Gestion efficace et effective des exigences de sécurité au sein de votre organisation
        activity: |
            Mettez en place un ensemble d'exigences de sécurité sur lesquelles les projets pourront s'appuyer pour établir une liste d'exigences appropriées et exhaustives. Cet ensemble prend en compte les différents types d'exigences et les différentes sources d'exigences. Il devrait être en phase avec les habitudes et la culture organisationnelles, et devrait fournir une méthodologie et une orientation efficaces dans l'élicitation et la création des exigences.

            Ce cadre aide les équipes projet à augmenter l'efficience et l'efficacité de l'ingénierie des exigences. Il peut fournir une catégorisation des exigences courantes et un certain nombre d'exigences réutilisables. Rappelez-vous que, même si la copie mécanique est inefficace, le fait d'avoir de potentielles exigences pertinentes comme support est souvent productif.

            Ce cadre donne également des conseils clairs sur la qualité des exigences et formalise la façon de les décrire. Pour les récits, par exemple, des conseils concrets peuvent permettre de décrire les critères de réussite, de définir les critères de départ, de formaliser les récits et les critères d'acceptation.

        question: Utilisez-vous un cadre standard d'exigences pour faciliter la clarification des exigences de sécurité?
        quality_criteria:
            - Un cadre d'exigences de sécurité est disponible pour les équipes de projet
            - Le cadre définit des catégories pour les exigences communes et les exigences basées sur des normes
            - Le cadre de référence donne des orientations claires sur la qualité des exigences et sur la façon de les décrire
            - Le cadre est adaptable aux exigences spécifiques de l'entreprise

        answers:
            - "No"
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
