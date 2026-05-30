# ✦ Astra Vale SMP

> A Minecraft Paper plugin adding legendary weapons, amethyst crystal powers, and high-stakes PvP mechanics inspired by Lifesteal and Bliss SMP — built for **Astra Vale SMP**.

---

## ✦ Features

### ⚔️ Legendary Weapons
Five craftable weapons with game-changing abilities. Each requires rare, hard-to-obtain materials and fundamentally changes how combat works.

| Weapon | Ability | Rarity |
|---|---|---|
| **Blade of Exile** | Bans the player you kill for **2 hours** | Legendary |
| **Soulthief Bow** | **Steals a heart** from killed players permanently | Legendary |
| **Thundermace** | **Lunge skyward** and deal massive fall-damage on descent | Legendary |
| **Phantom Dagger** | Grants **5 seconds of full invisibility** after a kill | Epic |
| **Voidscythe** | **Teleports you behind** a target within 20 blocks | Rare |

---

### 💎 Amethyst Crystal System
Every player receives a **random Amethyst Crystal** on first join. Crystals grant passive and active powers that define your playstyle — and can be upgraded up to **Tier 3** using rare materials.

**9 Crystal Types:**

| Crystal | Base Power (T1) | Tier 3 Pinnacle |
|---|---|---|
| 🔥 **Ember** | Fire resistance | Explosion on kill |
| ❄️ **Frost** | Slowness aura to nearby enemies | Freeze target for 1.5s |
| ⚡ **Storm** | Speed I outdoors | Double jump + lightning strike on kill |
| 🌑 **Void** | Hidden on tab-list | Phase through 1-block-thick walls |
| 🌿 **Terra** | +2 max hearts | +6 max hearts + reduced fall damage |
| 🛡️ **Veil** | 10% hit negate chance | 20% negate + crits deal normal damage |
| ✨ **Echo** | +20% XP from all sources | +50% XP + enhanced Mending |
| ⚔️ **Surge** | +10% attack speed | +30% speed + absorption heart on kill |
| 💚 **Bloom** | Regen I below 6 hearts | Regen II always + heal 3 hearts on kill |

**Upgrading:**
- T1 → T2: `Primal Amethyst ×4`
- T2 → T3: `Primal Amethyst ×8` + `Void Shard ×1`

---

### 🪨 Rare Crafting Materials

| Material | Source |
|---|---|
| **Void Shard** | Drops from the Ender Dragon on death |
| **Soul Essence** | Rare drop from killing players bare-handed |
| **Wither Star Fragment** | 1-in-3 chance from a Nether Star |
| **Primal Amethyst** | Found exclusively in deep dark geodes |

---

## 🚀 Installation

1. Download the latest `.jar` from [Releases](../../releases)
2. Drop it into your server's `/plugins` folder
3. Restart your server
4. All done — crystals are assigned automatically on first join

**Requirements:**
- [Paper](https://papermc.io/) 1.21+
- Java 21+

---

## ⚙️ Commands

| Command | Description | Permission |
|---|---|---|
| `/giveweapon <player> <weapon>` | Give a legendary weapon | `astravale.admin` |
| `/crystal <player>` | View a player's crystal and tier | `astravale.admin` |
| `/crystal give <player> <type>` | Force-assign a crystal | `astravale.admin` |

---

## 🗂️ Project Structure

```
AstraVale/
├── pom.xml
└── src/main/
    ├── resources/
    │   ├── plugin.yml
    │   └── config.yml
    └── java/me/astravale/
        ├── AstraVale.java
        ├── crystal/
        │   ├── CrystalType.java
        │   ├── CrystalManager.java
        │   ├── CrystalListener.java
        │   └── CrystalUpgradeHandler.java
        ├── weapon/
        │   ├── WeaponManager.java
        │   ├── LegendaryWeapon.java
        │   └── impl/
        │       ├── BladeOfExile.java
        │       ├── SoulthiefBow.java
        │       ├── Thundermace.java
        │       ├── PhantomDagger.java
        │       └── Voidscythe.java
        ├── listener/
        │   ├── PlayerJoinListener.java
        │   └── WeaponListener.java
        ├── command/
        │   ├── GiveWeaponCommand.java
        │   └── CrystalCommand.java
        ├── data/
        │   ├── PlayerDataManager.java
        │   └── BanManager.java
        └── util/
            ├── ItemBuilder.java
            ├── MessageUtil.java
            └── WeaponIdentifier.java
```

---

## 🔨 Building from Source

```bash
git clone https://github.com/yourusername/AstraVale.git
cd AstraVale
mvn clean package
```

The compiled `.jar` will be in `/target`.

---

## 📄 License

This project is licensed under the MIT License. See [`(https://github.com/Jdoggames4/Astra-Vale-SMP/blob/main/LICENSE)`](LICENSE) for details.

---

## 🤝 Contributors
- Jdoggames4 (Developer)
- MooniiCodes (Tester)

<div align="center">
  <sub>Made with ☕ for Astra Vale SMP</sub>
</div>
