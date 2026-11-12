---
name: rentabilite-import-afrique
description: "À réception d'une offre fournisseur (devis, proforma, liste de prix) pour un produit à importer en Afrique centrale : relever les prix du marché à Brazzaville, Pointe-Noire, Douala et Kinshasa, estimer fret et douane, dire si c'est rentable, puis rédiger un brouillon de réponse."
---

# Offre fournisseur → rentable ou non → brouillon de réponse

Skill offert par NELVIS (nelvis-france.com). Version gratuite.

## But unique
Transformer une offre fournisseur en décision chiffrée (RENTABLE / LIMITE / NON RENTABLE) et en brouillon de réponse, sans rien envoyer.

## Déclencheur
L'utilisateur colle ou joint une offre fournisseur (email, PDF, proforma, capture) pour un produit destiné à l'Afrique centrale (CEMAC, RDC).

## Étapes
1. **Contexte** : identifier fournisseur, produit, quantité visée. Relire tout l'échange fourni, pas seulement le dernier message. Noter ce qui est déjà négocié pour ne jamais le redemander.
2. **Extraire l'offre** : spécifications, prix unitaire, incoterm, MOQ, délais, paiement, validité.
3. **Prix marché** : chercher les prix de vente du même produit à Brazzaville, Pointe-Noire, Douala et Kinshasa (FCFA ou USD). Citer la source et la date de chaque relevé. Si introuvable : écrire « non trouvé », ne rien inventer.
4. **Coût rendu** : prix fournisseur + fret (par m³ en groupage LCL ou par kg en aérien ; demander à l'utilisateur son tarif transitaire s'il en a un) + droits et taxes du pays d'arrivée + frais locaux (port, transit, transport). Calculer le coût rendu par unité.
5. **Rentabilité** : marge par unité et par ville = prix marché − coût rendu. Verdict RENTABLE / LIMITE / NON RENTABLE.
6. **Risques** : hypothèses fragiles, taux de change, délais, MOQ, qualité. Proposer un test à coût faible (échantillon, pilote de 10 unités).
7. **Brouillon de réponse** au fournisseur, axé négociation : pilote, paliers 10/50/100, MOQ réduit, OEM/private label, paiement échelonné. Ne rien envoyer sans validation.

## Règles
- Toujours distinguer : fait vérifié / hypothèse / estimation / recommandation.
- Montrer les calculs, pas seulement le verdict.

## Exemple de sortie
**Conclusion** : LIMITE — marge ~18 % à Brazzaville, ~9 % à Kinshasa ; viable seulement avec MOQ réduit.

| Ville | Prix marché | Coût rendu | Marge |
|---|---|---|---|
| Brazzaville | … | … | … |
| Pointe-Noire | … | … | … |
| Douala | … | … | … |
| Kinshasa | … | … | … |

**Faits / Hypothèses / Risques** : …
**Test conseillé** : pilote de 10 unités.
**Brouillon de réponse** : (prêt à valider, non envoyé)
