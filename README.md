<p align="center"><img src="mod/true_pagan_reforms/thumbnail.png" width="256" alt="True Pagan Reforms"></p>

# True Pagan Reforms

A Crusader Kings III mod that makes AI pagan reformations less predictable. When an AI ruler reforms a pagan faith, some of the new faith's tenets are swapped for ones that fit the reformer, and some of its doctrines shift in the same direction: a lustful reformer may preach Carnal Exaltation and accept adultery, an eccentric mystic Esotericism and witchcraft, a sadistic warlord Human Sacrifice. Every playthrough gets its own reformed faiths.

- **Game version:** 1.20.x
- **Mod version:** 1.3.0
- **Author:** [Sourenics](https://github.com/Sourenics)
- **Steam Workshop:** [True Pagan Reforms](https://steamcommunity.com/sharedfiles/filedetails/?id=3817742251)

## Features

- **Only AI reformations.** When you reform a faith yourself, nothing changes: you keep the tenets and doctrines you picked.
- **1 or 2 tenets swapped**, depending on the game rule. A reformed faith has three tenets, so at least one always stays.
- **Kinship with the old faith.** If the reformed faith kept tenets from the unreformed one, at least one of them is always kept.
- **Or a clean break.** With the **No Kinship** setting, all three tenets are replaced, and none of the old faith's tenets can be kept or come back. Syncretism and Carnal Exaltation can go too; if the faith had Virtuous deviancy, it moves back to Accepted, since it needs Carnal Exaltation.
- **Shaped by the reformer.** The new tenets are drawn at random, weighted by the reformer's personality traits, lifestyle traits and education. A tenet that fits gets a much higher chance; one that does not fit can still appear, so results stay varied.
- **A tenet that already fits the reformer is more likely to stay**, and so is one inherited from the old faith.
- **Every tenet is an option.** Any tenet the game lets the faith choose can be added, and any tenet can be swapped out, except syncretism (which only comes from the reformer's bonds) and the last one inherited from the old faith.
- **No impossible faiths.** Every new tenet and doctrine passes the game's own checks for the faith (`is_shown` and `can_pick`, including religion and DLC requirements). The faith editor's compatibility rules, which the game only checks while editing a faith, are read from the game files and checked after every change; a change that breaks one is undone and another option is tried. On top of that, the mod keeps violent tenets out of pacifist faiths and Asceticism away from Hedonism and Carnal Exaltation.
- **Love and friendship across faiths.** If the reformer has a soulmate, best friend, lover or spouse of another religion, that religion's syncretism tenet (Christian, Islamic, Jewish, Dharmic or Sinitic Syncretism, or Syncretic Folk Traditions for another pagan faith) can be one of the new tenets. A soulmate pulls hardest, and a spouse who is also the soulmate even more; a best friend, a lover and a spouse pull less, in that order. Without such a bond, syncretism tenets are never added, and a faith never gets more than one.
- **Doctrines shift too.** Depending on its own game rule, 0 to 6 doctrines move one step to a neighbouring option (for example, Witchcraft from Shunned to Accepted or to Criminal, never straight from Criminal to Virtuous). Each doctrine changes at most once per reform, and the choice is weighted by the reformer's traits, gender and sexuality.
- **Doctrines that can change:** every doctrine group a faith can pick in the editor except the religion-specific ones: Head of Faith, View on Gender, Religious Attitude, Clerical Tradition, Pilgrimage Attitude, Theism, Clerical Function, Clerical Gender, Clerical Marriage, Clerical Appointment, Funeral, Coronation (with its DLC), Monasticism, Sacraments, Marriage Type, Divorce, Bastardry, Consanguinity and all crime doctrines (Same-Sex Relations, Deviancy, Male and Female Adultery, Kinslaying, Witchcraft). Groups with an order move one step; the others can move to any option the game allows. Special doctrines are never changed.
- **Head of faith.** It moves one step too (None, Spiritual, Temporal). The title is then handled by the game's own events, the same ones it uses when a rite is edited: a title is created when the requirements (holy sites, piety) are met, otherwise the faith can create it later with the game's decision.
- **Doctrines and tenets stay compatible**, following the faith editor's rules: for example Adaptability only with Pluralist, Virtuous Deviancy only with Carnal Exaltation, Polyamory only with accepted adultery, and no Theocratic tradition or spiritual appointment with a temporal head of faith.

### What fits whom

| Reformer | Favoured tenets |
|---|---|
| Lustful, Reveler | Carnal Exaltation, Hedonism, Ritual Celebrations |
| Chaste, Temperate, Humble | Asceticism |
| Gluttonous, Gregarious | Ritual Celebrations, Hedonism, Ritual Hospitality |
| Shy, Paranoid, Deceitful, Craven, Intrigue education | Sacred Lies, Esotericism, Chthonic Redoubts |
| Wrathful, Brave, Vengeful, Blademaster, Martial education | Warmongering, Gruesome Festivals, Unrelenting Faith |
| Sadistic, Callous | Human Sacrifice, Ritual Cannibalism, Exaltation of Pain, Gruesome Festivals |
| Zealous, Stubborn | Unrelenting Faith, Literalism, Sacrificial Ceremonies, Religious Law |
| Cynical, Arbitrary, Fickle | Adaptability, Pursuit of Power |
| Eccentric, Mystic, Learning education | Esotericism, Astrology, Auspicious Birthright |
| Ambitious, Greedy, Arrogant | Pursuit of Power, Auspicious Birthright |
| Content | Ancestor Worship, Communal Identity |
| Generous, Compassionate, Calm, Forgiving, Diplomacy education | Ritual Hospitality, Communal Possessions, Sacred Childbirth |
| Just | Legalism, Religious Law |
| Diligent, Patient, Stewardship education | Megalithic Constructions, Communal Possessions |
| Hunter, Herbalist | Sanctity of Nature |
| Physician | Sacred Childbirth |
| Compassionate, Calm | Pacifism |
| Generous, Humble, Temperate | Vows of Poverty, Mendicant Preaching |
| Deceitful, Cynical | Sanctioned False Conversions |
| Lustful | Polyamory |
| Arrogant | Divine Marriage |
| Learning education, Eccentric | Gnosticism |

Every other tenet the faith can choose can still be drawn with the base chance.

| Reformer's bond with someone of another religion | Weight for that religion's syncretism tenet |
|---|---|
| Soulmate | 150 |
| Best friend | 80 |
| Lover | 60 |
| Spouse | 30 (100 if the spouse is also the soulmate) |

Weights add up, so a Christian spouse who is also the reformer's soulmate gives Christian Syncretism 250. For comparison, every other tenet starts at 10, plus up to about 40 to 80 for fitting traits.


| Reformer | Favoured doctrines |
|---|---|
| Lustful, Reveler | Adultery Accepted, Deviancy Accepted or Virtuous, Concubines or Polygamous, Divorce Always Allowed, Clerical Marriage Allowed |
| Chaste, Temperate | Monogamous, Adultery and Deviancy Criminal, Clerical Marriage Disallowed, No Bastards |
| Zealous | Head of Faith: Spiritual, Fundamentalist or Righteous, Theocratic, Mandatory or Encouraged Pilgrimage, Witchcraft Criminal |
| Ambitious, Arrogant, Greedy | Head of Faith: Temporal |
| Content, Humble | Head of Faith: None |
| Cynical, Ambitious, Arrogant | Pluralist, Lay Clergy, Temporal Appointment, laxer Kinslaying |
| Eccentric, Mystic, Herbalist | Witchcraft Accepted or Virtuous |
| Paranoid | Witchcraft Criminal, Pilgrimage Forbidden, Temporal for Life appointment |
| Compassionate, Just, Forgiving | Kinslaying Criminal, Legitimization, Divorce Must be Approved |
| Sadistic, Callous, Arbitrary | Kinslaying Shunned or Accepted |
| Greedy, Stewardship education | Clerical Function: Control |
| Generous, Compassionate, Diplomacy education | Clerical Function: Alms and Pacification, Pluralist |
| Wrathful, Brave, Martial education | Clerical Function: Recruitment |
| Female reformer | Equal or Female Dominated, Clerical Gender Either or Female Only |
| Male reformer | Male Dominated, Clerical Gender Male Only |
| Homosexual or bisexual reformer | Same-Sex Relations Accepted |

### Game rules

Two rules in the game rules screen when starting a new game:

| Setting | **TPR: Pagan Reform Tenets**: tenets swapped | **TPR: Pagan Reform Doctrines**: doctrines changed |
|---|---|---|
| None | — | 0 |
| Light | 1 | 1 |
| Moderate (default) | 1 or 2, even odds | 2 |
| Strong | 2 | 3 or 4, even odds |
| No Kinship | all 3, none of the old faith's tenets kept | — |
| Radical | — | 4, 5 or 6, even odds |

In a save started before the doctrine rule existed, doctrines use the Moderate setting.

### Languages

English and Spanish. Players using any other game language see the English text. Translations are welcome: open an [issue](../../issues/new/choose) or post them on the Steam Workshop page.

## Installation

### Steam Workshop

Subscribe on the Steam Workshop page and enable the mod in the Paradox launcher.

### Manual

1. Download this repository (green **Code** button → **Download ZIP**).
2. Copy the contents of the `mod/` folder (`true_pagan_reforms/` and `true_pagan_reforms.mod`) into:
   - **Windows:** `Documents/Paradox Interactive/Crusader Kings III/mod/`
   - **Linux:** `~/.local/share/Paradox Interactive/Crusader Kings III/mod/`
   - **macOS:** `~/Documents/Paradox Interactive/Crusader Kings III/mod/`
3. Enable **True Pagan Reforms** in the Paradox launcher.

## Compatibility

- No DLC required. Tenets that need a DLC are only used if you own it.
- Overrides no vanilla file. It hooks into `on_faith_created` by appending to it, so it works alongside other mods that use the same on_action.
- Can be added to an existing save; reformations that already happened are not changed. Can be removed at any time.
- Faiths changed by the mod stay as they are if you remove it.

### Testing it yourself

With the console open (`-debug_mode` launch option), type `effect tpr_debug_vary_my_faith = yes` to apply the variation (tenets and doctrines) to your own faith's main rite as if your character were an AI reformer. Use it on a test save: it changes your faith.

## Reporting bugs

Please open an [issue](../../issues/new/choose) using the **Bug report** template. To be able to fix the problem we need:

1. **The `error.log` file** from the session where the problem happened:
   - **Windows:** `Documents/Paradox Interactive/Crusader Kings III/logs/error.log`
   - **Linux:** `~/.local/share/Paradox Interactive/Crusader Kings III/logs/error.log`
   - **macOS:** `~/Documents/Paradox Interactive/Crusader Kings III/logs/error.log`

   The log is overwritten every time the game starts, so copy it right after the problem happens, before launching the game again. Ideally, reproduce the problem in a session with **only True Pagan Reforms enabled**.
2. **The game version** (shown in the main menu, for example 1.20.1) and **the mod version**.
3. **Your active DLCs** and **your full mod list in load order**.
4. **Which faith** was reformed, by whom, and which tenets and doctrines it ended up with.
5. **Screenshots** of the faith window, if possible.

## Credits

Idea and testing by Sourenics.

## License

**True Pagan Reforms** © 2026 Sourenics, licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).

Forks, translations and alternative versions are welcome, provided that you:

- **Credit the original author** (Sourenics) and link to this repository.
- **Indicate the changes** you made.
- **Release your version under the same license** (CC BY-SA 4.0).

### Paradox Interactive content

Crusader Kings III and its content are © Paradox Interactive AB and are **not** covered by this license. This includes the tenets, traits and game concepts the mod refers to. This project is an unofficial fan-made mod, not affiliated with or endorsed by Paradox Interactive. Like every CK3 mod, it must be distributed free of charge.
