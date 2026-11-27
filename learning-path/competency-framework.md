# OSEF Continuous Compliance Engineer — référentiel v0.1
Statut : proposition à approuver, 27 novembre 2026. Pilote : [COMP-SKILL-001](https://github.com/opensource-enterprise-factory/osef-compliance-engineering/issues/43).
## Finalité et limites
Concevoir, automatiser, tester et exploiter les contrôles de conformité, de l'obligation à la preuve et à la remédiation. Le titulaire ne remplace ni juriste, ni auditeur indépendant, ni autorité de supervision. Une preuve technique n'établit pas à elle seule la conformité juridique. Référentiels autorisés et applicabilité validée par le client et les experts compétents.
## Niveaux de qualification
| Niveau | Intitulé interne | Autonomie | Résultat attendu |
|---|---|---|---|
| L1 | Foundations | Sous supervision | Modéliser obligations, contrôles, risques, preuves |
| L2 | Practitioner | Autonome sur tâches bornées | Développer politiques testées et CI, gérer exceptions |
| L3 | Engineer | Autonome sur intégration bornée, revue par pair | Intégrer scanners, preuves, GRC; traiter incidents |
| L4 | Architect | Concevoir et encadrer, revue indépendante | Architecture bout en bout, arbitrages, sécurité, coûts, gouvernance IA |
Les niveaux sont cumulatifs; un grade ne confère ni accès production ni pouvoir d'approbation automatique. Les habilitations sont distinctes.
## Échelle de maîtrise par compétence
0 non démontré; 1 explique et réalise avec aide; 2 réalise seul sur périmètre connu; 3 adapte, diagnostique et justifie avec preuves; 4 conçoit, arbitre, accompagne et améliore. NE = non évalué, ne vaut pas réussite. Niveaux et scores évalués séparément.
## Matrice cible minimale
| Code | Domaine | L1 | L2 | L3 | L4 | Preuve principale |
|---|---|---:|---:|---:|---:|---|
| C01 | Applicabilité réglementaire, normes, droits d'usage | 1 | 2 | 2 | 3 | Matrice sourcée et limites |
| C02 | Risques, contrôles, responsabilités et exceptions | 1 | 2 | 3 | 4 | Registre et décisions |
| C03 | OSCAL, modèles et validation Trestle | 1 | 2 | 3 | 3 | #14 |
| C04 | Policy as Code OPA/Rego | 0 | 2 | 3 | 3 | #15 |
| C05 | Kubernetes / Kyverno | 0 | 2 | 3 | 3 | #16 |
| C06 | Cloud posture / Prowler / IAM | 0 | 0 | 2 | 3 | #17 |
| C07 | Linux / OpenSCAP / Wazuh | 0 | 0 | 2 | 3 | #18 |
| C08 | Evidence engineering, intégrité, fraîcheur, provenance | 1 | 2 | 3 | 4 | #18, #21 |
| C09 | GRC / CISO Assistant / API | 0 | 0 | 2 | 3 | #19 |
| C10 | Git, CI/CD, tests, PR-only, rollback | 1 | 2 | 3 | 4 | #14–21 |
| C11 | Sécurité, confidentialité, licences, éthique | 1 | 2 | 3 | 4 | Revue des preuves |
| C12 | Observabilité, incidents, SLO/SLA, exploitation | 0 | 1 | 2 | 4 | #21, #34 |
| C13 | Regulatory Intelligence IA/RAG et validation humaine | 0 | 0 | 0 | 3 | #20 |
| C14 | Architecture, interopérabilité, résilience et coûts | 0 | 1 | 2 | 4 | #21 |
| C15 | Contribution upstream, collaboration, anglais technique | 1 | 2 | 2 | 3 | #36–42 |
| C16 | Conseil, communication, recette et valeur client | 1 | 2 | 3 | 4 | Simulation / mission |
Une cible 0 signifie non requise au niveau, pas compétence acquise. Les scores 3–4 nécessitent variantes et arbitrages au-delà d'un lab guidé; le jury demande preuves supplémentaires. Pour C01 L4, revue par juriste/compétent plutôt que décision juridique autonome.
## Attendus observables par domaine
- C01 : identifier juridiction, version, source, droit d'usage, applicabilité à faire valider; distinguer norme et obligation.
- C02 : définir propriétaire, fréquence, risque résiduel, traitement et exception datée; justifier priorisation.
- C03 : catalogue/profil OSCAL versionnés, validation positive/négative, mapping stable.
- C04 : règles déterministes, refus par défaut, tests et décision exploitable; ne pas confondre évaluation et enforcement.
- C05 : admission, audit, exceptions et rapports; rollback sans exposition réelle.
- C06 : accès lecture seule, couverture, erreurs/non-applicabilité, remédiation par PR, coûts.
- C07 : compatibilité profil/distribution, état et événements, tests de régression.
- C08 : identifiants, UTC, source, version, empreinte protégée, rétention, expiration, provenance; hash seul ≠ authenticité.
- C09 : modèle risque/contrôle, RBAC, API, export et restauration.
- C10 : versions épinglées, tests positifs/négatifs, revue, CI, rollback et reproduction indépendante.
- C11 : autorisation, moindre privilège, secrets, données synthétiques, licence/DCO/CLA, divulgation responsable.
- C12 : métriques et alertes, UNKNOWN/ERROR distincts de PASS, incident horodaté, SLO mesuré et compte rendu.
- C13 : corpus versionné et autorisé, citations vérifiables, abstention, injection documentaire, évaluation et revue humaine.
- C14 : schémas et adaptateurs, idempotence, défaillances, RTO/RPO cibles testées, compromis coûts/souveraineté.
- C15 : recherche de doublons, échange respectueux, reproduction, contribution utile, suivi des retours.
- C16 : besoin, périmètre, livrables, hypothèses financières, SLA, acceptation, communication des limites et escalade.
## Spécialisations
Standards & Compliance as Code (C01–03, C10); Policy Engineering (C04–05); Continuous Controls & Evidence (C06–08, C12); GRC Integration (C09); Regulatory AI (C13); architecture transverse (C14). C11, C15 et C16 transversales. Un badge de spécialité peut être proposé après preuve L3 de ses domaines, sans dispenser du tronc commun.
## Références internes
[Parcours](README.md), [missions](mission-matrix.md), [règlement](certification-rules.md), [portfolio](portfolio-template.md), [gouvernance](../governance/README.md). Les sources techniques sont les issues de labs et les documentations officielles qu'elles référencent; versions et licences à vérifier à l'exécution.
