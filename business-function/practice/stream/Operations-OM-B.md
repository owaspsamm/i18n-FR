---
title: Démantèlement des Systèmes / Gestion de l'Existant
type: stream
url: ./model/operations/operational-management/stream-b/
business_function: Opérations
business_function_url: operations
practice: Gestion opérationnelle
stream: B
description: Opérations / Gestion opérationnelle
keywords: ["Business function", "Practice", "Opérations", "Gestion opérationnelle"]
aliases:
    - /fr/model/O-OM-B-1
    - /fr/model/O-OM-B-2
    - /fr/model/O-OM-B-3
    - /fr/model/O-OM-B

maturity_levels:
    level1:
        level: 1
        benefit: |
            Identification des actifs ou composants logiciels inutilisés
        activity: |
            Identifiez les applications inutilisées d'une façon ad hoc, soit par observation par hasard, soit en effectuant occasionnellement une revue. Lorsque vous identifiez des applications non utilisées, enregistrez ces constatations pour des actions ultérieures. Si vous avez établi un processus formel pour le démantèlement des applications non utilisées, assurez-vous que les équipes en sont informées et l'utilisent.

            Gérez la migration client / utilisateur à partir d'anciennes versions de vos produits pour chaque produit et chaque groupe de client / utilisateur. Lorsqu'une version du produit n'est plus utilisée par aucun groupe client / utilisateur, arrêtez le support pour cette version. Cependant, à ce niveau de maturité, il se peut que vous ayez un grand nombre de versions de produits en cours d'utilisation à travers toute la base de clients / utilisateurs, demandant des efforts significatifs aux développeurs pour garantir la compatibilité ascendante des correctifs de produits.

        question: Identifiez-vous et supprimez-vous les systèmes, les applications, les dépendances des applications ou les services qui ne sont plus utilisés, ont atteint leur fin de vie ou ne sont plus activement développés ou maintenus?
        quality_criteria:
            - Vous n'utilisez pas d'applications ou de dépendances non maintenues
            - Vous gérez la migration des clients / utilisateurs à partir des anciennes versions pour chaque produit et chaque groupe de clients / utilisateurs

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Un processus normalisé de démantèlement réduisant le risque d'oubli de composant
        activity: |
            Dans le cadre du démantèlement d'un systèm, d'une application ou d'un service, suivez un processus établi pour supprimer tous les comptes pertinents, les règles du pare-feu, les données, etc. de l'environnement opérationnel. En supprimant ces éléments inutiles des fichiers de configuration, vous améliorez la maintenabilité des ressources infrastructure-en-tant-que-code.

            Suivez un processus cohérent pour le remplacement ou la mise à jour en temps opportun d'applications tierces ou de dépendances de l'application (par ex., système d'exploitation, applications utilitaires, bibliothèques), qui ont atteint leur fin de vie.

            Rapprochez-vous des clients et des groupes d'utilisateurs de vos produits en fin de vie ou approchant de leur fin de vie afin de les faire migrer en temps voulu vers des versions supportées.

        question: Suivez-vous un processus établi pour la suppression de toutes les ressources associées, dans le cadre du démantèlement des systèmes, des applications, des dépendances des applications ou des services inutilisés?
        quality_criteria:
            - Vous documentez les statuts de prise en charge de toutes les versions publiées de vos produits dans un endroit accessible
            - Le processus comprend le remplacement ou la mise à jour des applications tierces ou des dépendances d'applications qui ont atteint leur fin de vie
            - Les environnements d'exploitation ne contiennent pas de comptes, de règles de pare-feu ou autres artefacts de configuration inutiles

        answers:
            - Non
            - Oui, une partie du temps
            - Oui, au moins la moitié du temps
            - Oui, la majeure partie du temps ou tout le temps

    level3:
        level: 3
        benefit: |
            Visibilité totale dans le cycle de vie de tous les actifs logiciels
        activity: |
            Évaluez régulièrement l'étape du cycle de vie et le statut de support de tous les actifs logiciels et composants d'infrastructure sous-jacents et estimez leur fin de vie. Suivez un processus bien défini pour atténuer activement les risques de sécurité qui surviennent lorsque les actifs / composants approchent de leur fin de vie. Examinez et mettez à jour régulièrement votre processus afin de refléter les leçons tirées de l'expérience.

            Établissez un plan de support produit fournissant des échéanciers clairs pour la fin de support des versions antérieures du produit. Limitez les versions de produits en cours d'utilisation à un petit nombre (par exemple, N.x.x et N-1 seulement). Établissez et diffusez des échéanciers pour la fin de support des versions antérieures, et engagez-vous de façon proactive avec les clients et les groupes d'utilisateurs afin d'éviter les perturbations de service ou de support.

        question: Évaluez-vous régulièrement l'état du cycle de vie et le statut de maintenance de chaque logiciel et de chaque composant d'infrastructure sous-jacent et estimez-vous leur fin de vie?
        quality_criteria:
            - Votre processus de gestion de fin de vie est validé
            - Vous informez les clients et les groupes d'utilisateurs des échéanciers des produits afin d'éviter toute perturbation du service ou du support
            - Vous passez en revue le processus au moins une fois par an

        answers:
            - Non
            - Oui, pour certains des actifs
            - Oui, pour au moins la moitié des actifs
            - Oui, pour la plupart ou la totalité des actifs

---
