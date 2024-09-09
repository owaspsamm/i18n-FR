---
title: Détection d'Incident
type: stream
url: ./model/operations/incident-management/stream-a/
business_function: Opérations
business_function_url: operations
practice: Gestion des incidents
stream: A
description: Opérations / Gestion des incidents
keywords: ["Business function", "Practice", "Opérations", "Gestion des incidents"]
aliases:
    - /fr/model/O-IM-A-1
    - /fr/model/O-IM-A-2
    - /fr/model/O-IM-A-3
    - /fr/model/O-IM-A

maturity_levels:
    level1:
        level: 1
        benefit: |
            Possibilité de détecter les incidents de sécurité les plus évidents
        activity: |
            Analysez les données journalisées disponibles (par exemple, les journaux d'accès, les journaux d'applications, les journaux d'infrastructure) afin de détecter les incidents de sécurité éventuels, tout en respectant les périodes de rétention connues des données.

            Dans de petites configurations, vous pouvez le faire manuellement à l'aide d'outils en ligne de commande courants. Avec de plus grands volumes de journaux, utilisez des techniques d'automatisation. Même une tâche `cron`, exécutant un script simple pour rechercher les événements suspects, est un pas en avant!

            Si vous envoyez des journaux à partir de sources différentes vers un système d'agrégation dédié à la journalisation, analysez-y les logs et utilisez les principes de base de corrélation de journaux .

            Même si vous n'avez pas de processus de détection d'incidents fonctionnant 24 heures sur 24, 7 jours sur 7, assurez-vous que la non-disponibilité de la personne responsable (p. ex. en raison de vacances ou de maladie) n'affecte pas significativement la vitesse ou la qualité de la détection.

            Établissez et partagez des points de contact pour la création formelle d’incidents de sécurité.

        question: Analysez-vous périodiquement les données des journaux pour ce qui est des incidents de sécurité?
        quality_criteria:
            - Vous avez un point de contact pour la création d'incidents de sécurité
            - Vous analysez les données en respectant les durées de rétention des données de journalisation
            - La fréquence de cette analyse est en phase avec le niveau de criticité de vos applications

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level2:
        level: 2
        benefit: |
            Détection rapide et cohérente des incidents de sécurité prévisibles
        activity: |
            Nommez un propriétaire dédié pour le processus de détection des incidents, rendez la documentation claire et accessible à tous les acteurs du processus et veillez à ce qu'il soit régulièrement révisé et mis à jour si besoin. Assurez-vous que les employés responsables de la détection d'incidents suivent ce processus (p. ex. en utilisant la formation).

            Le processus repose typiquement sur un degré élevé d'automatisation, de collecte et de corrélation des données de journalisation provenant de différentes sources, y compris les journaux d'évènements. Vous pouvez agréger les journaux dans un endroit centralisé si cela est souhaitable. Vérifiez périodiquement l'intégrité des données analysées. Si vous ajoutez une nouvelle application, assurez-vous que le processus la prend en compte dans un délai raisonnable.

            Détectez les éventuels incidents de sécurité en utilisant une liste de contrôle facilement disponible. La liste de contrôle devrait couvrir les vecteurs d'attaque envisageables et connus et les chaînes de compromission attendues. Évaluez-la et mettez-la à jour régulièrement.

            Lorsque vous déterminez qu'un événement est un incident de sécurité (avec suffisamment de confiance), avertissez immédiatement le personnel responsable, même en dehors des heures de bureau. Effectuez une analyse plus approfondie tel que nécessaire et commencez le processus d'escalade.

        question: Suivez-vous un processus documenté pour la détection d'incidents?
        quality_criteria:
            - Le processus a un propriétaire dédié
            - Vous stockez la documentation du processus dans un endroit accessible
            - Le processus envisage une escalade pour une analyse plus approfondie
            - Vous formez les employés responsables de la détection d'incidents à ce processus
            - Vous avez une liste de contrôle des attaques potentielles pour simplifier la détection d'incidents

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

    level3:
        level: 3
        benefit: |
            Capacité à détecter rapidement les incidents de sécurité
        activity: |
            Assurez-vous que la documentation du processus inclut des mesures pour l'amélioration continue du processus. Vérifiez la continuité de l'amélioration du processus (par exemple, via le suivi des changements).

            Assurez-vous que la liste de contrôle pour la détection d'événements suspects est corrélée au moins (i) à des sources et bases de connaissances externes à la société (par ex., les annonces nouvelles de vulnérabilités affectant les technologies utilisées), (ii) aux incidents de sécurité passés et (iii) aux résultats du modèle de menaces.

            Utilisez la corrélation des logs pour la détection d'incidents pour tous les scénarios d'incidents raisonnables. Si les données de log pour la détection d'incident ne sont pas disponibles, documentez son absence en tant que défaut, priorisez-le et gérez-le selon votre processus de gestion des défauts en place.

            La qualité de la détection d'incident ne dépend pas de l'heure ou du jour de l'événement. Si les événements de sécurité ne sont pas pris en compte et résolus dans un laps de temps déterminé (par ex. 20 minutes), assurez-vous que d'autres notifications sont générées selon un processus d'escalade établi.

        question: Réexaminez-vous et mettez-vous à jour régulièrement le processus de détection d'incident ?
        quality_criteria:
            - Vous effectuez des revues au moins une fois par an
            - Vous mettez à jour la liste de contrôle des attaques potentielles avec des données externes et internes

        answers:
            - Non
            - Oui, pour certaines applications
            - Oui, pour au moins la moitié des applications
            - Oui, pour la plupart ou toutes les applications

---
