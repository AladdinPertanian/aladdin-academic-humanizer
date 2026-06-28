<!--
Copyright (c) 2026 Dr. Aladdin Ali - Founder of Aladdin Pertanian Internasional - dr.alaa@aladdin.my.id. All Rights Reserved.
-->

# Exemples Travaillés (Français) — Worked Examples (French)
## Skill reference — `fr` SOURCE-GROUNDED ([FR1] Guide de rédaction · [FR2] Boudouresque · [FR3] Anthropos)
### À parité avec le fichier anglais `before-after.md` / at full parity with the English file

> Ces exemples ont une **profondeur équivalente** à `before-after.md` (anglais) : les trois canaux, **deux
> éléments de suggestion** (A-01 + A-02), un **journal de révision** complet et la **barrière de
> consentement**, en français. Chaque nombre/citation/DOI est **conservé caractère par caractère** (INV-A1).
> La norme du français scientifique est appliquée : **la forme passive** (recommandée) sans première personne
> (*je/nous*) [FR2]. Le modèle à trois canaux et la barrière de consentement sont **identiques** à la version
> anglaise.

---

## Exemple 1 — Affirmation excessive + de-AI, flux complet (consentement accordé)

**Contrat :** `level=journal` · `programme_type=journal` · `edit_scope=apply_approved_notes` ·
`co_authored=false` · `ai_disclosure_policy=required` · `output_language=fr`.

**Entrée (paragraphe de discussion) :**
> « En conclusion, notre étude révolutionnaire prouve clairement que le Médicament X provoque des hémorragies !
> 😊 Les études montrent qu'il s'agit d'une découverte cruciale. Dans notre essai, nous avons observé des
> hémorragies chez **18** des **20** patients (voir **Tableau 2**), ce qui est cohérent avec Almeida et al.
> **[7]**. »

### Canal 1 — Texte amélioré sur le plan linguistique (automatique, expression seule)
> « L'étude prouve clairement que le Médicament X provoque des hémorragies. Les études montrent qu'il s'agit
> d'une découverte importante. Dans l'essai, des hémorragies ont été observées chez **18** des **20** patients
> (voir **Tableau 2**), ce qui est cohérent avec Almeida et al. **[7]**. »

*Modifié (expression seule) :* « En conclusion, » supprimé (HUM-25) ; « révolutionnaire » supprimé (HUM-01) ;
« ! 😊 » supprimé (HUM-18) ; « cruciale » → « importante » (§B lexique). **Règle de personne/voix (ACA-04 ·
[FR2]) :** « notre étude » → « l'étude » ; première personne *« Dans notre essai, nous avons observé »* →
**forme passive** *« Dans l'essai, … ont été observées »*. *Conservé :* l'affirmation **« prouve clairement …
provoque »** (force de l'affirmation — c'est le Canal 2, ACA-01) ; l'attribution sans référence **« Les études
montrent »** (HUM-05, en mode académique → Canal 2) ; et **`18` · `20` · `Tableau 2` · `[7]`** — caractère par
caractère (INV-A1).

### Canal 2 — Rapport de suggestions scientifiques (suggéré, non appliqué)
- **A-01 (ACA-01 · affirmation excessive/objectivité) :** « prouve clairement que le Médicament X provoque des
  hémorragies » dépasse un seul essai (18/20) et contrevient à un **langage objectif et neutre** [FR1]/[FR2].
  Reformulation limitée à l'échantillon et prudente : *« Dans cet échantillon, des hémorragies ont été
  observées chez la plupart des patients, ce qui pourrait indiquer un problème de sécurité nécessitant des
  recherches supplémentaires. »* *(modifie la force de l'affirmation — décision de l'auteur)*
- **A-02 (HUM-05 / ACA-02 · attribution vague) :** « Les études montrent qu'il s'agit d'une découverte
  importante » sans référence — citez des études précises, nuancez ou supprimez. *(ne jamais inventer une
  référence — AIP-3)*

### Consentement de l'auteur
`consent_to_apply = accordé`, accepté : **A-01, A-02** (l'auteur choisit de **supprimer** la phrase sans
référence) ; `authorship_acknowledgement = confirmé`.

### Canal 3 — Révision scientifique approuvée par l'auteur (appliquée + humanisée)
> « L'étude examine la relation entre le Médicament X et les hémorragies. Dans l'essai, des hémorragies ont
> été observées chez **18** des **20** patients (voir **Tableau 2**), ce qui pourrait indiquer un problème de
> sécurité nécessitant des recherches supplémentaires, et est cohérent avec Almeida et al. **[7]**. »

### Journal de révision (INV-A10)
**En-tête :** `fr` · `journal`/`journal` · `apply_approved_notes` · `co_authored=false` ·
`ai_disclosure_policy=required` → déclaration d'utilisation de l'IA incluse · accepté : `A-01, A-02` ·
`authorship_acknowledgement=confirmé`.

| change_id | emplacement | canal | élément approuvé | avant → après | motif | vérification d'invariant |
|-----------|-------------|:-----:|------------------|---------------|-------|--------------------------|
| C-001 | Discussion ¶ | C.3 | A-01 | « prouve clairement … provoque des hémorragies … ont été observées chez 18 des 20 → L'étude examine la relation entre le Médicament X et les hémorragies … pourrait indiquer un problème de sécurité … » | l'auteur a accepté la reformulation limitée à l'échantillon (affirmation causale excessive supprimée) | INV-A6 : affirmation atténuée par décision de l'auteur ; nombres inchangés |
| C-002 | Discussion ¶ | C.3 | A-02 | « Les études montrent qu'il s'agit d'une découverte importante. → *(supprimée)* » | l'auteur a accepté de supprimer l'attribution sans référence | INV-A2/A3 : rien d'inventé ; suppression par l'auteur |
| C-003 | Discussion ¶ | C.1 | — (ACA-04 · [FR2]) | « Dans notre essai, nous avons observé → Dans l'essai, … ont été observées » | forme passive recommandée, sans première personne (automatique, sens conservé) | INV-A6 : sens conservé |
| C-004 | Discussion ¶ | C.1 | — (HUM-01/18/25) | « En conclusion, notre étude révolutionnaire … ! 😊 → L'étude … » | de-AI d'expression seule | INV-A6 : sens conservé |

**Fidélité et déclaration :** `18` → inchangé · `20` → inchangé · `Tableau 2` → inchangé · `[7]` → inchangé.
Aucune limite scientifique supprimée ; aucune preuve faible convertie en affirmation forte sans élément
approuvé. Déclaration : déclaration d'utilisation de l'IA incluse ; aucune affirmation « indétectable ».
**La responsabilité principale de la recherche incombe à l'auteur**, et l'autorité finale au directeur et au
jury.

---

## Exemple 2 — Barrière de consentement (consentement **non accordé** → pas de Canal 3)

**Contrat :** `level=masters` · `programme_type=masters_thesis` · `edit_scope=language_clarity` ·
`co_authored=false` · `ai_disclosure_policy=unknown` · `output_language=fr`.

**Entrée :**
> « Vous pouvez voir clairement dans la **Figure 3** que le modèle ne fonctionne en réalité pas très bien, ce
> qui représente une limite importante. Le taux d'erreur était de **12,4 %**. »

### Canal 1 — Texte amélioré sur le plan linguistique (automatique, expression seule)
> « La **Figure 3** montre que le modèle ne fonctionne en réalité pas très bien, ce qui représente une limite
> importante. Le taux d'erreur était de **12,4 %**. »

*Modifié (expression seule) :* deuxième personne « Vous pouvez voir … dans la Figure 3 » → forme impersonnelle
« La Figure 3 montre » (ACA-04 · [FR2]). *Conservé :* l'atténuateur « en réalité » (le supprimer renforce
l'affirmation → Canal 2) ; et **`12,4 %`** — caractère par caractère ; le décimal à virgule et l'espace
insécable du français **ne sont pas modifiés** (INV-A1).

### Canal 2 — Rapport de suggestions scientifiques (suggéré)
- **B-01 (ACA-08 · descriptif→critique) :** « ne fonctionne pas très bien » est évaluatif mais non quantifié
  au-delà de 12,4 % — précisez la comparaison/le seuil qui rend ce taux « pas bon ».

### Consentement de l'auteur
`consent_to_apply = non accordé`.

### Résultat — le Canal 3 n'est pas produit
Les Canaux 1 et 2 sont livrés en entier. **Pas de Canal 3 ; aucun élément de suggestion appliqué ; aucun
journal de révision produit.** `12,4 %` n'a pas changé. *(Déclaration : `ai_disclosure_policy=unknown` → une
déclaration consultative est tout de même fournie ; le silence n'est jamais un résultat.)*

> **Preuve de la barrière de consentement :** l'élément de niveau pensée **B-01 n'a pas été appliqué** ; les
> données d'entrée ont été conservées caractère par caractère ; **le Canal 3 a été retenu** car ses cinq
> conditions n'étaient pas remplies (consentement non accordé) — exactement le comportement de la barrière
> (Blueprint §11 G1).

---

*Skill reference — `fr` worked examples (full parity with `before-after.md`: A-01+A-02, 4-row revision log),
source-grounded [FR1][FR2][FR3]. © 2026 Dr. Aladdin Ali / Aladdin Pertanian Internasional.*
