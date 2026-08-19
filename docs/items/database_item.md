# 🎒 Database Item RPG — Alwination

---

## Legenda Rarity

| Simbol | Rarity |
|---|---|
| ⚪ | Common |
| 🟢 | Uncommon |
| 🔵 | Rare |
| 🟣 | Ultra Rare |
| 🟡 | Mythical |

---

## Item Drop (Didapat dari Mob/Bos)

| Item | Rarity | Sumber Drop |
|---|---|---|
| Gold *(bukan vanilla)* | ⚪ Common | Mob RPG — Overworld |
| Ember Fragment | 🟢 Uncommon | Mob RPG — Overworld |
| Obsidian Relic | 🟢 Uncommon | Mob RPG — Nether |
| Undead Heart | 🔵 Rare | Mob RPG — Overworld |
| Mythril Fragment | 🔵 Rare | Mob RPG — Overworld & Dungeon |
| Valdrak Core | 🟣 Ultra Rare | Bos — Dungeon Lapisan 1 |
| Dracula Seal | 🟣 Ultra Rare | Mob RPG — Dungeon Lapisan 2 |
| Morthazar Core | 🟣 Ultra Rare | Bos — Dungeon Lapisan 2 |
| Crimson Veil | *(belum ada info)* | *(belum ada info)* |

---

## Item Sintesis (Harus Di-craft)

### 🔵 Refined Ember (Rare)

| Material | Jumlah |
|---|---|
| Mythril Fragment | x4 |
| Ember Fragment | x8 |
| Gold | x12 |

---

### 🔵 Hardened Gold Ingot (Rare)

| Material | Jumlah |
|---|---|
| Hardened Iron Ingot | x1 |
| Refined Ember | x8 |
| Gold | x64 |

> ⚠️ **Catatan:** Ada duplikasi data di sumber asli. Satu entri kosong, satu entri lengkap. Resep di atas menggunakan data yang lengkap.

---

### 🟣 Primordial Mythril (Ultra Rare)

| Material | Jumlah |
|---|---|
| Mythril Fragment | x8 |
| Refined Ember | x16 |
| Gold | x64 |

---

### 🟡 Relic of Eternity (Mythical)

> ⚠️ **Resep sintesis belum diketahui** — data kosong di sumber asli.

---

## Hierarki Item (Dari Rendah ke Tinggi)

```
⚪ Common
│  └── Gold
│
🟢 Uncommon
│  ├── Ember Fragment
│  └── Obsidian Relic
│
🔵 Rare
│  ├── Undead Heart (drop)
│  ├── Mythril Fragment (drop)
│  ├── Refined Ember (sintesis)
│  └── Hardened Gold Ingot (sintesis)
│
🟣 Ultra Rare
│  ├── Valdrak Core (drop — Dungeon L1 Bos)
│  ├── Primordial Mythril (sintesis)
│  ├── Dracula Seal (drop — Dungeon L2 Mob)
│  └── Morthazar Core (drop — Dungeon L2 Bos)
│
🟡 Mythical
   └── Relic of Eternity (sintesis — resep belum diketahui)
```

---

## Dependency Tree Sintesis

```
Refined Ember
├── Mythril Fragment x4
├── Ember Fragment x8
└── Gold x12

Hardened Gold Ingot
├── Hardened Iron Ingot x1
├── Refined Ember x8
│   ├── Mythril Fragment x32  (4×8)
│   ├── Ember Fragment x64    (8×8)
│   └── Gold x96              (12×8)
└── Gold x64

Primordial Mythril
├── Mythril Fragment x8
├── Refined Ember x16
│   ├── Mythril Fragment x64  (4×16)
│   ├── Ember Fragment x128   (8×16)
│   └── Gold x192             (12×16)
└── Gold x64

─── Total Bahan Mentah untuk 1× Primordial Mythril ───
    Mythril Fragment:  72  (8 + 64)
    Ember Fragment:    128
    Gold:              256 (192 + 64)
```
