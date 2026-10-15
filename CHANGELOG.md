# Changelog

## 1.3.0

- New tenet setting **No Kinship**: all three tenets of the reformed faith are replaced, and none of the old faith's tenets can be kept or come back. Syncretism and Carnal Exaltation can be replaced too; a Virtuous deviancy then moves back to Accepted.
- New doctrine setting **Radical**: 4, 5 or 6 doctrines (even odds) move one step.

## 1.2.1

- Checked against CK3 1.20.1.
- Fixed: a reformed faith could end up with both Ecclesiarchy (Pentarchy) and Fundamentalist pluralism, a combination the faith editor does not allow. The mod now checks this rule too.

## 1.2.0

- New: a reformer's bonds with people of another religion can bring that religion's syncretism tenet (Christian, Islamic, Jewish, Dharmic or Sinitic Syncretism, or Syncretic Folk Traditions for another pagan faith) into the reformed faith. Soulmates weigh the most, then best friends, lovers and spouses; a spouse who is also the soulmate weighs even more. Suggested by TurtleShroom.
- Every tenet the game lets the faith choose is now an option when reforming, instead of a fixed list of pagan tenets; any tenet except syncretism can be swapped out. This fixes Religious Law always being kept. Zealous, just or paranoid reformers favour Religious Law, and new trait affinities cover Pacifism, Vows of Poverty, Polyamory, Gnosticism and others.
- Every doctrine group the faith editor allows can now shift (adds Theism, Funeral, Coronation, Monasticism and Sacraments); religion-specific and special doctrines are never changed.
- The faith editor's compatibility rules are read from the game files and checked after every change; a change that breaks one is undone and another option is tried.
- Arrogant reformers now lean as much as ambitious ones toward a temporal head of faith.
- Syncretism tenets are never removed by the mod, never added without such a bond, and a faith never gets more than one.
- Game rules are now named **TPR: Pagan Reform Tenets** and **TPR: Pagan Reform Doctrines**, with a coloured prefix so they are easy to find. Their settings are kept in existing saves.
- New: the head of faith can shift too, one step between None, Spiritual and Temporal, weighted by the reformer's traits. The title is handled by the game's own events, as when a rite is edited.
- New thumbnail: a wheel of pagan symbols (triquetra, sun, moon, triple spiral, tree, stag, waves, raven, dolmen) with the gold frame used by the other Sourenics mods.

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
