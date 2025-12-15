# Black Dusk Mod Structure

## Directory Layout

```
black_dusk/
├── common/
│   ├── bookmarks/
│   │   └── 2028_start.txt         # Main bookmark for game start
│   ├── countries/
│   │   └── [TAG].txt              # Country color/graphics definitions
│   ├── country_tags/
│   │   └── 00_countries.txt       # All country tag definitions
│   ├── ideologies/
│   │   └── 00_ideologies.txt      # Custom ideology system
│   ├── ideas/
│   │   └── 00_country_ideas.txt   # National spirits and modifiers
│   └── national_focus/
│       ├── QLF_focus.txt          # Qing Loyalist Forces focus tree
│       ├── IND_MUG_focus.txt      # India/Mughal focus tree
│       ├── EDC_focus.txt          # Eastern Defense Command focus tree
│       ├── OMS_focus.txt          # Omsk focus tree
│       └── WSU_focus.txt          # West Siberian Union focus tree
├── events/
│   └── super_events.txt           # Major story events
├── history/
│   └── countries/
│       └── [TAG] - [Name].txt     # Country starting conditions
├── localisation/
│   └── english/
│       ├── bookmarks_l_english.yml
│       ├── countries_l_english.yml
│       ├── events_l_english.yml
│       ├── ideologies_l_english.yml
│       └── music_l_english.yml
├── music/
│   └── black_dusk_music.txt       # Music definitions
├── descriptor.mod                  # Mod descriptor
├── README.md                       # This file
└── MOD_STRUCTURE.md               # Structure documentation
```

## Country Tags

### BLA Empire
- BLA - Black Liberation Army Core
- BLE - BLA England
- BLF - BLA France
- BLG - BLA Germany
- BLI - BLA Italy
- BLB - BLA Benelux
- BLP - BLA Poland
- BLJ - BLA Japan
- BLR - BLA Russia

### Asian Front
- QLF - Qing Loyalist Forces
- IND - India (Democratic)
- MUG - Mughal Empire
- BUS - Busan Rebellion
- FJR - Free Japanese Republic
- DUR - Durzekstan

### Russian Front
- EDC - Eastern Defense Command
- NOV - Novosibirsk Command
- YEK - Yekaterinburg Warlords
- IRK - Irkutsk Monarchists
- VLA - Vladivostok Syndicalists
- KAZ - Kazan Revivalists
- OMS - Omsk
- WSU - West Siberian People's Union

### North American Front
- CLA - Continental Liberation Authority
- WCO - Western Coalition
- CAS - Cascadia
- TEX - Texas Republic
- CAH - Canadian Holdouts

### British Isles Remnants
- SCO - Scotland
- WAL - Wales
- NIR - Northern Ireland

### Other
- CHE - Chechnya

## Ideologies

1. **Liberation** - BLA ideology (radical/moderate)
2. **Monarchism** - Imperial restoration, constitutional, absolutism
3. **Democracy** - Liberal, social, emergency
4. **Syndicalism** - Revolutionary, council
5. **Communism** - Neo-Soviet, revolutionary guard
6. **Militarism** - Defense command, warlord state, national revenge
7. **Technocracy** - Industrial, corporate state
8. **Theocracy** - Religious revival, faith militant

## Super Events

1. **black_dusk_super.1** - The Second Crusade
2. **black_dusk_super.2** - The Princess's Desire
3. **black_dusk_super.3** - The Factory Reborn
4. **black_dusk_super.4** - Russia United (EDC path)
5. **black_dusk_super.5** - Russia United (Omsk path)
6. **black_dusk_super.6** - Russia United (WSU path)
7. **black_dusk_super.7** - BLA Japan Collapse

## Adding Music

Place .ogg files in the `music/` folder:
- united.ogg
- firepower.ogg
- breaking_the_law.ogg
- metal_gods.ogg
- turbo_lover.ogg
- rock_of_ages.ogg
- photograph.ogg
- hysteria.ogg
- drift_phonk_collapse.ogg
- dark_phonk_urban.ogg
- money_so_big.ogg
- talk.ogg
- after_hours.ogg
- blinding_lights.ogg
- gasoline.ogg

## Extending the Mod

### Adding New Countries
1. Add tag to `common/country_tags/00_countries.txt`
2. Create `common/countries/[TAG].txt` with graphics settings
3. Create `history/countries/[TAG] - [Name].txt` with starting conditions
4. Add localization to `localisation/english/countries_l_english.yml`
5. (Optional) Create focus tree in `common/national_focus/`

### Adding New Events
1. Add to `events/` directory
2. Add localization to `localisation/english/events_l_english.yml`

### Adding New Ideas
1. Add to `common/ideas/00_country_ideas.txt`
2. Add localization as needed
