# Catalogue de Labs
Propositions non exécutées. Versions à épingler après vérification des licences et prérequis officiels. Données synthétiques, environnement isolé, secrets hors Git, changements via PR.
| ID | Niveau | Ressources indicatives | Architecture et justification | Étapes | Validation |
|---|---|---|---|---|---|
| COMP-LAB-001 | Débutant | 2 vCPU/4 Go, Python/Git | OSCAL → Trestle → CI; format ouvert et validation | Créer 10 contrôles fictifs; valider; introduire erreur; automatiser | Catalogue valide accepté, invalide rejeté |
| COMP-LAB-002 | Intermédiaire | 2 vCPU/4 Go | JSON → OPA/Rego → décision; séparer politiques et application | Écrire règles accès, 20 tests positifs/négatifs, CI | Tous tests passent; PR non conforme bloquée |
| COMP-LAB-003 | Intermédiaire | 4 vCPU/8 Go, kind | Kubernetes → Kyverno → rapports; admission native | Tester privilèges, ressources, images, exceptions expirées | 5 politiques; violation rejetée |
| COMP-LAB-004 | Intermédiaire | 4 vCPU/8 Go, cloud sandbox autorisé | Prowler lecture seule → JSON → tickets; contrôles cloud | Créer 5 écarts sans exposition réelle, scanner, corriger par PR | 5 écarts détectés puis résolus |
| COMP-LAB-005 | Intermédiaire | 4–8 vCPU/16 Go, VM Linux | OpenSCAP + Wazuh → preuves horodatées; état et événements | 10 contrôles, collecte, SHA-256, altération volontaire | Preuves traçables, altération détectée |
| COMP-LAB-006 | Intermédiaire | 4 vCPU/8 Go, Compose | CISO Assistant → GRC/API; gestion risques et contrôles | Déployer, vérifier licence, importer référentiel autorisé, 10 risques, export | Matrice et responsabilités vérifiables |
| COMP-LAB-007 | Avancé | 8 vCPU/16 Go + inférence | Corpus public → RAG PostgreSQL/pgvector → revue humaine; citations | Versionner corpus BCEAO, comparer textes, 20 questions, cas sans preuve | Citations vérifiables, abstention en absence de source |
| COMP-LAB-008 | Avancé | 16 vCPU/32 Go répartis | OSCAL/Trestle → OPA/Prowler/Wazuh → GRC; intégration à qualifier | Connecteurs, preuves expirées, tickets, remédiation PR, réévaluation | 10 contrôles reliés, écart détecté en moins de 5 min sur scénario, rapport reproductible |

Chaque exécution doit consigner versions, commandes, résultats attendus/réels, rollback, captures expurgées et limites. Aucun résultat n'est une certification.
