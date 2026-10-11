# Changelog

## 1.1.0

- New: doctrines of an AI pagan reform also shift. Each changed doctrine moves one step to a neighbouring option (for example, Witchcraft from Shunned to Accepted or to Criminal), weighted by the reformer's traits, gender and sexuality. Head of faith and special doctrines are never changed.
- New game rule **Pagan Reform Doctrine Variation**: None, Light (1 doctrine), Moderate (2, default) or Strong (3 or 4). Saves started before this version use Moderate.
- The tenet game rule is now shown as **Pagan Reform Tenet Variation**. Its setting is kept in existing saves.
- Fixed: Adaptability could be added to a faith that is not Pluralist; it now needs Pluralist, as in the faith editor.
- Carnal Exaltation is no longer removed from a faith with Virtuous Deviancy.
- The console test effect `effect tpr_debug_vary_my_faith = yes` also varies doctrines.

## 1.0.0

- First public release.
- When the AI reforms a pagan faith, 1 or 2 of the reformed faith's tenets are swapped for ones that fit the reformer's personality, lifestyle and education.
- At least one tenet inherited from the old faith is always kept.
- Only tenets the faith can actually take are added, and clashing combinations are avoided.
- Game rule **Pagan Reform Variation**: Light (1 tenet), Moderate (1 or 2, default) or Strong (2).
- Console test effect: `effect tpr_debug_vary_my_faith = yes`.
- English and Spanish localization; other languages fall back to English.
