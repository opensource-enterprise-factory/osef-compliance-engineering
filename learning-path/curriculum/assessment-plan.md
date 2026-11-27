# Évaluations et examens — plan pilote
Le [règlement v0.1](../certification-rules.md) prévaut. Les exercices ci-dessous sont des sujets blancs publics; le jury prépare variantes inédites en espace privé. Notes individuelles, données personnelles et preuves client hors dépôt public.
## Diagnostic S1
30 min : 10 questions de base Git/Linux/JSON/risques et mini exercice de lecture JSON/PR. Non noté pour certification. Mentor propose plan de remise à niveau et valide prérequis.
## Quiz formatifs S1–S12
5 à 10 questions par semaine, correction argumentée par mentor. Objectif indicatif 80% et reprise si inférieur; n'entre pas automatiquement dans la note certificative. Exemples avec réponses attendues :
- S1 : Norme vs obligation ? Une norme n'est pas automatiquement obligatoire; vérifier incorporation et applicabilité. Un hash prouve-t-il origine ? Non.
- S2 : Catalogue vs profil OSCAL ? Le profil sélectionne/adapte des contrôles; vérifier schéma et références.
- S3 : Pourquoi deny-by-default ? Refuser en absence d'autorisation explicite; décision allow distincte du succès d'exécution.
- S4 : Audit vs enforcement ? Observer/rapporter vs empêcher action selon politique et mode; vérifier exception.
- S5 : ERROR équivaut-il à PASS ? Non; distinguer erreur, inconnu et non-applicable; permissions lecture seule.
- S6 : SCAP état vs événement Wazuh ? Évaluation de configuration vs observation de changements; couverture à vérifier.
- S7 : Preuve expirée ? Ne pas la considérer actuelle; réévaluer et signaler. Hash seul ne prouve pas provenance.
- S8 : RBAC et restauration ? Tester refus d'accès et restauration dans environnement jetable.
- S9 : RAG garantit-il exactitude ? Non; citations, version, abstention et revue humaine.
- S10 : Comment calculer exactitude ? Réponses correctes / questions répondables; mesurer abstention hors corpus séparément.
- S11 : Pourquoi idempotence ? Rejeu sans doublon ni modification indue; UNKNOWN/ERROR jamais PASS.
- S12 : SLA d'accusé vs résolution ? Engagements différents, périmètre et exclusions contractuels.
## Examens certificatifs proposés
| Jalon | Quiz | Pratique | Oral | Seuil |
|---|---:|---:|---:|---:|
| S2 L1 | 30 min | 2 h | 20 min | 75 |
| S4 L2 | 30 min | 3 h | 20 min | 75 |
| S8 L3 | 45 min | 4 h | 30 min | 80 |
| S12+ L4 | 45 min | 6 h | 45 min | 85 |
- L1 blanc : 5 obligations inédites fictives, catalogue/profil et fixture invalide, expliquer mapping et preuves; rechercher doublon upstream. Livrer JSON, logs, mapping et restitution.
- L2 blanc : nouvelle règle d'accès et manifestes inconnus; écrire tests, CI et exception bornée; démontrer refus et correction. Livrer patch, logs, rapport et critères de recette.
- L3 blanc : jeux de résultats cloud/Linux et GRC sandbox préinstallé; diagnostiquer écart et preuve périmée, traiter incident, exporter risque et plan; démontrer restauration ou test préconvenu. Livrer incident, preuves, matrice et mission simulée. Labs préparés en amont restent obligatoires.
- L4 blanc : architecture banque fictive, panne d'un scanner, doublon et question IA hors corpus; diagnostiquer, corriger par PR et réévaluer; défendre coût, sécurité, RTO/RPO, SLA, limites; prouver accompagnement pair. Livrer ADR, tests, runbook et soutenance. Le capstone complet est préparé avant examen.
## Barème
Connaissances 15, pratique 35, preuves 20, sécurité 15, upstream 5, mission/soutenance 10. Chaque catégorie note 0–4 × poids/4; seuils par catégorie et critères éliminatoires du règlement. Matrice C01–C16 vérifiée indépendamment. Chaque examen utilise jury de deux évaluateurs sans conflit, variante inconnue et reproduction. Documentation autorisée; IA déclarée et résultats vérifiés individuellement. 
## Rattrapage
Si non acquis : plan correctif par compétence, exercices ciblés et nouvelle variante conformément au règlement; aucune progression certifiée automatique. Révision des seuils/durées uniquement après pilote et par PR, sans effet rétroactif. 
