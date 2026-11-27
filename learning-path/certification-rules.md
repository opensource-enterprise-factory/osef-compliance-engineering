# Règlement de certification interne OSEF CCE — proposition v0.1
À faire approuver par la gouvernance avant délivrance. Qualification interne non accréditée, sans équivalence ISO, CNCF, diplôme, habilitation réglementaire ou certification d'entreprise.
## Conditions par niveau
| Niveau | Prérequis | Épreuves et preuves obligatoires | Seuil global |
|---|---|---|---:|
| L1 Foundations | Diagnostic d'entrée; Git/Linux de base | LAB-001, quiz, restitution de mapping, exercice contribution (recherche de doublons et brouillon) | 75/100 |
| L2 Practitioner | L1 ou équivalence sur preuves | LAB-002/003, épreuve pratique à variante inconnue, revue PR, contribution utile soumise ou alternative motivée | 75/100 |
| L3 Engineer | L2 ou équivalence sur preuves | LAB-004/005/006, incident et mission simulée ADVISE/BUILD/OPERATE, contribution upstream soumise ou alternative motivée, soutenance | 80/100 |
| L4 Architect | L3 ou équivalence sur preuves | LAB-007/008, architecture et cas bancaire, arbitrage sécurité/coûts/SLA, accompagnement d'un pair, soutenance et revue indépendante | 85/100 |
Équivalence : jury vérifie toutes les preuves et cibles des niveaux antérieurs, jamais sur ancienneté seule. Une fusion upstream n'est pas obligatoire; elle dépend des mainteneurs. Alternative autorisée uniquement si refus justifié, absence de besoin utile ou contrainte documentée : reproduction/test/doc interne revue, discussion amont si appropriée; jury valide sans prétendre contribution soumise.
## Barème commun (100 points)
| Domaine | Points | Indicateurs |
|---|---:|---|
| Connaissances et raisonnement | 15 | concepts, applicabilité, limites |
| Pratique technique | 35 | critères labs, variante autonome, diagnostics |
| Qualité des preuves et reproductibilité | 20 | versions, tests, traçabilité, reproduction indépendante |
| Sécurité, éthique et gouvernance | 15 | accès, confidentialité, licence, PR, rollback |
| Collaboration/upstream | 5 | utilité, doublons, communication et revue |
| Mission et soutenance | 10 | besoin, livrable, recette, argumentation |
Pour chaque catégorie, noter sur 0–4 (0 absent, 1 insuffisant, 2 partiel, 3 conforme aux attentes du niveau, 4 dépasse avec preuve); points = poids × note / 4. Total non arrondi pour décision; afficher 2 décimales. Le seuil L4 exige plusieurs catégories au-delà du minimum, justifiées par variantes complexes et arbitrages. Chaque catégorie doit atteindre au moins 50% de son poids; pratique, preuves et sécurité au moins 75%. Toutes les cibles minimales de la matrice doivent être démontrées (score de maîtrise distinct de la note d'épreuve).
## Critères éliminatoires indépendants du total
- Falsification de résultats, plagiat, violation de licence, divulgation de secret/donnée client, accès ou scan non autorisé.
- Contournement volontaire de la revue ou du contrôle de sécurité; prétention infondée de conformité/homologation.
- Critère bloquant de lab non atteint, preuve obligatoire absente, erreur critique de sécurité non corrigée.
Décision motivée : non validé ou suspendu selon procédure; incident sécurité traité séparément. Aucun score ne compense ces écarts.
## Processus d'évaluation
1. Inscription et niveau cible; déclaration d'intégrité, règles IA et aménagements raisonnables.
2. Portfolio des preuves et auto-évaluation; référent contrôle complétude.
3. Quiz 30 min L1/L2, 45 min L3/L4; épreuve pratique supervisée 2h L1, 3h L2, 4h L3, 6h L4 (durées proposées; labs préparés en amont). Variante nouvelle; documentation autorisée; usage IA déclaré et vérification autonome, sans données sensibles.
4. Reproduction indépendante par évaluateur; soutenance 20 min L1/L2, 30 min L3, 45 min L4.
5. Deux évaluateurs qualifiés et sans conflit d'intérêts, dont au moins un indépendant du formateur direct; troisième arbitre si désaccord de décision ou écart >10 points. L4 inclut expertise architecture et sécurité; revue juridique externe si nécessaire.
6. PV avec scores par catégorie, matrice, preuves, écarts et décision. Résultats communiqués sous 10 jours ouvrés (objectif).
7. Rattrapage ciblé après plan correctif, à partir de 14 jours, dans les 90 jours; nouvelle variante. Au-delà, réévaluation du dossier. Recours motivé dans les 10 jours ouvrés; examinateur indépendant répond cible 15 jours ouvrés.
## Validité et maintien
Proposition : 24 mois à compter de validation. Maintien annuel : 20 heures de formation/pratique documentées, une revue de changement de versions/standards, une activité de contribution ou revue, un exercice de contrôle/incident adapté au niveau. Renouvellement : portfolio actualisé, revue et épreuve pratique ciblée; suspension en cas de manquement grave avec contradictoire et recours. Pas de délivrance automatique.
## Registre et protection des données
Identifiant de certificat, niveau, version du référentiel, date délivrance/expiration, statut, décision et évaluateurs dans registre privé à accès restreint. Publication du nom ou badge uniquement avec consentement et validation. Proposition de rétention des preuves : 24 mois après expiration, sous réserve des obligations applicables et politique approuvée; suppression contrôlée. Le dépôt public ne reçoit que modèles et artefacts synthétiques.
## Calibration et contrôle qualité
Piloter sur 2–4 volontaires, comparer notation inter-évaluateurs, vérifier faisabilité des durées et seuils, ajuster par PR; ne pas changer rétroactivement les critères d'une session. Revue annuelle du référentiel, audit par échantillon des dossiers et suivi des recours.
