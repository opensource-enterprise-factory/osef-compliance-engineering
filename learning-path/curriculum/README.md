# Programme CCE — 12 semaines (pilote v0.1)
Issue #45. Référentiel et règlement v0.1 dans learning-path/. Les 12 semaines sont un calendrier cible; la charge est renforcée aux examens et à l'intégration. Qualification uniquement après validation du règlement, preuves, jury et cibles cumulatives. Pas de certification accréditée.
## Cas fil rouge
Banque UEMOA fictive « Banque Horizon » : 1 cluster lab, 1 sandbox cloud autorisé, VM Linux, 10 contrôles fictifs, registre des risques et preuves. Aucun lien avec une banque réelle. Toute obligation réelle nécessite source/version/droit d'usage et revue compétente. Aucun secret ni données client. Déploiements par PR et automation; aucun accès production.
## Charge et prérequis
Git, Linux, JSON, réseau, Python de base; diagnostic S1 et remédiation préalable si nécessaire. Ressources évolutives selon #14–21; sandbox cloud budgetée, inférence IA et stockage à qualifier. Les heures sont par apprenant, estimées pour environnement préparé, incluant cours/exercices/TP/revue/examen; temps mentor séparé. Les labs initiaux ont des durées indicatives distinctes, notamment #21 cinq jours : prévoir prolongation, travail en binôme avec preuve individuelle et créneaux supplémentaires si nécessaire. Aucun raccourci sur critères.
| Semaine | Thème | Niveau | Heures cibles | Labs |
|---|---|---|---:|---|
| 1 | Fondamentaux de la conformité et diagnostic initial | L1 | 10 | #14 |
| 2 | OSCAL, Trestle et évaluation Foundations | L1 | 12 | #14 |
| 3 | Policy as Code avec OPA et Rego | L2 | 12 | #15 |
| 4 | Kubernetes Compliance et évaluation Practitioner | L2 | 14 | #16 |
| 5 | Cloud Compliance avec Prowler | L3 | 12 | #17 |
| 6 | Linux Compliance et collecte technique | L3 | 12 | #18 |
| 7 | Evidence Engineering et incident simulé | L3 | 12 | #18 |
| 8 | Enterprise GRC et évaluation Engineer | L3 | 16 | #19 |
| 9 | Regulatory Intelligence AI — corpus et RAG | L4 | 12 | #20 |
| 10 | Évaluation IA et architecture d'intégration | L4 | 14 | #20, #21 |
| 11 | Intégration Continuous Compliance et résilience | L4 | 18 | #21 |
| 12 | Capstone bancaire, soutenance et évaluation Architect | L4 | 18 | #21 |
Total indicatif 162 h. Les examens occupent une part des semaines 2/4/8/12. Organiser 2 créneaux cours/exercices, 2–3 créneaux TP et 1 revue; horaires réels à convenir. Prévoir réserve après S12 pour reprises.
## Séances détaillées
### S01 — Fondamentaux de la conformité et diagnostic initial
Niveau L1 · 10 h · compétences C01 C02 C08 C10 C11 C15 C16 · Labs #14.
- **Cours :** Différencier loi, règlement, norme, politique, contrôle, risque et preuve; applicabilité, cycle de vie, audit vs conformité continue; Git/PR, licences et secrets.
- **Exercices :** Classer 12 énoncés fictifs; mapper 10 exigences à des contrôles, propriétaires, fréquence et preuve; justifier 3 risques et 2 exceptions; quiz de 10 questions.
- **Travaux pratiques :** Préparer Linux/Python/Git, vérifier versions et droits; créer données synthétiques et structure LAB-001; tester JSON et préparer catalogue.
- **Livrables :** Matrice de 10 contrôles, diagnostic d'entrée non noté, inventaire versions, PR revue.
- **Validation :** 10 liens obligation-contrôle-preuve; distinguer applicabilité et interprétation; aucun secret.
- **Upstream :** #36 : lire documentation OSCAL et CONTRIBUTING; chercher sujets similaires.
- **Mission/Meetup :** #27/#28 : entretien simulé et reformulation du besoin.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S02 — OSCAL, Trestle et évaluation Foundations
Niveau L1 · 12 h · compétences C01 C02 C03 C08 C10 C11 C15 C16 · Labs #14.
- **Cours :** Modèles catalogue/profil, identifiants, schémas, validation, Git et CI; provenance des preuves.
- **Exercices :** Construire un profil de sélection; prédire résultat de 5 fixtures; identifier 2 erreurs de mapping; restitution sponsor.
- **Travaux pratiques :** Finaliser LAB-001 : catalogue 10 contrôles, validation positive/négative, pipeline CI et clone propre; examen L1 en fin de semaine.
- **Livrables :** Catalogue et profil fictifs, fixtures, logs CI, restitution et portfolio privé.
- **Validation :** Critères #14 atteints, variante nouvelle et cible L1; seuil 75 selon règlement.
- **Upstream :** #36 : recherche de doublons et brouillon utile, sans soumission forcée.
- **Mission/Meetup :** #22 : préparer démonstration; #28 : matrice réglementaire fictive.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S03 — Policy as Code avec OPA et Rego
Niveau L2 · 12 h · compétences C02 C03 C04 C08 C10 C11 C12 C14 C15 C16 · Labs #15.
- **Cours :** Décision vs enforcement, deny-by-default, entrée JSON, Rego, tests déterministes, exceptions et expiration.
- **Exercices :** Écrire table de décision pour accès privilégié; concevoir 20 cas positifs/négatifs, champs manquants et expiration; expliquer code de sortie vs allow.
- **Travaux pratiques :** LAB-002 : version épinglée, règles et fixtures, opa test, CI bloquante, PR de correction, rollback.
- **Livrables :** Règles, 20 tests, logs, mapping OSCAL, revue pair.
- **Validation :** 20 tests passent; tous refus attendus; CI bloque non-conformité et accepte correction.
- **Upstream :** #38 ou #37 : identifier besoin réel, reproduire et discuter approche.
- **Mission/Meetup :** #31 : qualifier dix contrôles automatisables et définir recette.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S04 — Kubernetes Compliance et évaluation Practitioner
Niveau L2 · 14 h · compétences C04 C05 C08 C10 C11 C12 C14 C15 C16 · Labs #16.
- **Cours :** Admission Kubernetes, audit/enforce, RBAC, policies, exceptions bornées, PolicyReports.
- **Exercices :** Analyser 5 manifests; prédire admission; concevoir exception datée et rollback; distinguer scan existant/admission.
- **Travaux pratiques :** LAB-003 : kind isolé, 5 politiques, tests positifs/négatifs, rapports, correction PR et teardown; examen L2.
- **Livrables :** Manifests, policies, résultats admission, rapport et dossier L2.
- **Validation :** 5 politiques testées; ressources interdites rejetées; exception retirée; cibles L2 et seuil 75.
- **Upstream :** #39 ou #38/#37 : contribution soumise ou alternative motivée selon règlement.
- **Mission/Meetup :** #23 : préparer démo; #31 : livrer politique CI et recette simulée.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S05 — Cloud Compliance avec Prowler
Niveau L3 · 12 h · compétences C02 C06 C08 C10 C11 C12 C14 C15 C16 · Labs #17.
- **Cours :** Responsabilité partagée, IAM lecture seule, couverture des contrôles, posture, coûts et remédiation.
- **Exercices :** Choisir 5 contrôles supportés; définir vérité terrain, permissions minimales et budget; classer PASS/FAIL/ERROR/non applicable.
- **Travaux pratiques :** LAB-004 : sandbox autorisé, 5 écarts inoffensifs, scan JSON, normalisation, tickets, correction IaC/PR, rescan et teardown.
- **Livrables :** Rapports avant/après, mapping, tickets, coûts, preuve nettoyage.
- **Validation :** 5/5 écarts détectés puis résolus; lecture seule; aucune exposition réelle.
- **Upstream :** #41 : explorer tests mockés et contrôles existants.
- **Mission/Meetup :** #32 : cadrer un pilote cloud et ses limites.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S06 — Linux Compliance et collecte technique
Niveau L3 · 12 h · compétences C07 C08 C10 C11 C12 C14 · Labs #18.
- **Cours :** SCAP, XCCDF/OVAL, profils compatibles, état vs événement, Wazuh agent/manager, UTC et provenance.
- **Exercices :** Choisir 10 contrôles Linux fictifs; mapper source et fréquence; distinguer preuve absente, expirée, modifiée et résultat FAIL.
- **Travaux pratiques :** LAB-005 partie A : VM cible isolée, profil autorisé, scan OpenSCAP, événements Wazuh et exports; vérifier compatibilité.
- **Livrables :** Topologie, résultats bruts expurgés, mapping 10 contrôles, journal versions.
- **Validation :** 10 contrôles avec résultat attendu et source; accès restreints; horodatage et versions.
- **Upstream :** #40 : lire documentation SCAP et reproduire un cas minimal.
- **Mission/Meetup :** #33 : cartographier preuves manuelles et sources.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S07 — Evidence Engineering et incident simulé
Niveau L3 · 12 h · compétences C07 C08 C10 C11 C12 C14 C15 C16 · Labs #18.
- **Cours :** Normalisation, SHA-256, manifeste protégé, provenance, rétention, expiration, intégrité vs authenticité, incident et escalade.
- **Exercices :** Définir schéma evidence_id/control_id/source/UTC/version/hash/status; tester 4 cas de preuve et calculer fraîcheur; définir procédure incident.
- **Travaux pratiques :** LAB-005 partie B : collecteur Python, stockage protégé, altération d'une copie, absence/expiration, correction PR et nouvelle preuve; exercice incident.
- **Livrables :** Scripts, registre, tests, chronologie incident et rapport avant/après.
- **Validation :** 10 preuves traçables; altération/absence/expiration détectées; pas de PASS sur preuve invalide.
- **Upstream :** #40 ou #41 : fixture/test de régression et échange amont.
- **Mission/Meetup :** #24 : préparer démo; #33/#34 : pilote et rapport d'incident.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S08 — Enterprise GRC et évaluation Engineer
Niveau L3 · 16 h · compétences C02 C03 C04 C05 C06 C07 C08 C09 C10 C11 C12 C14 C15 C16 · Labs #19.
- **Cours :** GRC, actifs, risques, contrôles, RBAC, API, sauvegarde/restauration, recette et transfert.
- **Exercices :** Évaluer 10 risques fictifs, définir propriétaires, traitements, priorités et KPI; préparer rapport exécutif et exercice incident.
- **Travaux pratiques :** LAB-006 : Compose, référentiel autorisé, 10 risques, contrôles/preuves, API/export, test accès et restauration; variante d'intégration; examen L3.
- **Livrables :** Matrice risques, scripts API, preuve restauration, dossier mission ADVISE/BUILD/OPERATE.
- **Validation :** 10 risques reliés, cohérence API/export, accès interdit refusé, restauration; cibles L3 et seuil 80.
- **Upstream :** #42 ou autre parcours : soumission utile ou alternative motivée; suivi des retours.
- **Mission/Meetup :** #27/#30/#34 : mission simulée complète et restitution.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S09 — Regulatory Intelligence AI — corpus et RAG
Niveau L4 · 12 h · compétences C01 C11 C13 C14 C16 · Labs #20.
- **Cours :** Corpus versionné, extraction, segmentation, embeddings, retrieval, pgvector, citations, droits d'usage et revue humaine.
- **Exercices :** Sélectionner 2–5 textes publics autorisés; identifier version et page; écrire 20 questions annotées dont 5 hors corpus; décrire risques IA.
- **Travaux pratiques :** LAB-007 partie A : ingestion, métadonnées, indexation, retrieval filtré, réponses citées, tests d'injection documentaire.
- **Livrables :** Manifest corpus, pipeline et jeu d'évaluation annoté.
- **Validation :** Sources vérifiables et extraction contrôlée; aucun document confidentiel; modèle/licence épinglés.
- **Upstream :** #36/#37 : étudier exemples de métadonnées; contribution ciblée existante si pertinente.
- **Mission/Meetup :** #29 : inventaire IA, risques et protocole d'évaluation.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S10 — Évaluation IA et architecture d'intégration
Niveau L4 · 14 h · compétences C01 C02 C08 C11 C13 C14 C15 C16 · Labs #20, #21.
- **Cours :** Hallucinations, abstention, métriques, supervision humaine, contrats d'interface et modèle d'évaluation.
- **Exercices :** Exécuter les 20 questions, calculer exactitude sur répondables et couverture citations; concevoir architecture et ADR; menaces, coûts et SLO.
- **Travaux pratiques :** Finaliser LAB-007, analyser erreurs; LAB-008 partie A : mapping 10 contrôles, schéma PASS/FAIL/UNKNOWN/ERROR, topologie et plan de tests.
- **Livrables :** Rapport IA, ADR, modèle de données et architecture.
- **Validation :** ≥85% exactitude sur répondables; citations vérifiables; 5/5 abstentions hors corpus; injections ignorées sur scénarios.
- **Upstream :** Revue d'une contribution #36–42; accompagner un pair.
- **Mission/Meetup :** #25 : préparer démo IA; #29/#30 : arbitrages et limites.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S11 — Intégration Continuous Compliance et résilience
Niveau L4 · 18 h · compétences C02 C03 C04 C05 C06 C07 C08 C09 C10 C11 C12 C14 C15 C16 · Labs #21.
- **Cours :** Adaptateurs, idempotence, orchestration, preuve protégée, observabilité, indisponibilité et reprise.
- **Exercices :** Écrire tests doublon, timeout, preuve expirée et indisponibilité; définir RTO/RPO cibles et protocole de mesure; revue menace et capacité.
- **Travaux pratiques :** LAB-008 partie B : intégrer ≥3 sources, 10 contrôles, registre, GRC/API ou import explicite, ticket, PR corrective, réévaluation; mesurer délai.
- **Livrables :** Adaptateurs, tests, rapports, runbook, métriques et preuve rollback.
- **Validation :** 10 contrôles reliés; ≥3 sources; écart détecté et ticket <5 min sur scénario; erreur jamais PASS; remédiation reproductible.
- **Upstream :** Accompagner pair, revue upstream et journal des retours.
- **Mission/Meetup :** #26 : répétition démo bancaire; #33/#34 : définir recette et SLO.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

### S12 — Capstone bancaire, soutenance et évaluation Architect
Niveau L4 · 18 h · compétences C01–C16 · Labs #21.
- **Cours :** Gouvernance, arbitrages coût/risque, souveraineté, sécurité, SLA, responsabilité et pérennité.
- **Exercices :** Cas banque fictive : chiffrer architecture avec hypothèses, justifier risques résiduels, présenter 90 jours et SLA; préparer revue indépendante.
- **Travaux pratiques :** Finaliser LAB-008 : répéter scénario complet, rollback, test résilience, rapport reproductible; examen L4, soutenance, accompagnement pair.
- **Livrables :** Dossier architecture, ADR, budget, preuves, rapport audit, plan exploitation, portfolio et PV privé.
- **Validation :** Critères #21, toutes cibles L4, seuil 85, aucune erreur critique ou preuve manquante; prolonger si besoin.
- **Upstream :** État réel contribution, retour d'expérience et plan de maintien.
- **Mission/Meetup :** #26 : démo validée; #27–35 : proposition ADVISE/BUILD/OPERATE simulée.
- **Suivi :** PR de livrables synthétiques, revue pair, test attendu/réel, portfolio privé, quiz formatif et décision continuer/reprendre. 

## Évaluations
Voir [plan d'examens](assessment-plan.md) et [règlement](../certification-rules.md). Les quiz hebdomadaires sont formatifs, non substituts aux examens. Les scores de maîtrise de la matrice et points d'examen restent distincts.
## Sources
Issues #14–21 et #36–42, #22–35, [référentiel](../competency-framework.md), [missions](../mission-matrix.md), documentation officielle référencée dans les Labs. Versions/licences à vérifier au démarrage. 
