📡 EmissionTimeTweek

A lightweight UE4SS mod for MISERY that customizes emission timing and restores the iconic pre-emission siren.
Author: Ruff Trigger

🎯 Features

Custom Emission Timer
Set your own emission interval by editing a single variable:

EMISSION_TIME_SECONDS = 600.0


Works reliably across all emission cycles.

Authentic Siren Warning
Automatically plays the game’s original 2-minute siren cue before each emission.
Configurable threshold:

SIREN_THRESHOLD_SECONDS = 120.0


Cycle Detection System
Detects when a new emission cycle begins and reapplies your custom timing automatically.

Non-Intrusive Design
The mod does not cancel or freeze emissions.
It simply adjusts the emission countdown and injects a warning sound.

⚙ Configuration

All settings are at the top of main.lua.

local EMISSION_TIME_SECONDS   = 600.0   -- Custom emission interval (seconds)
local ENABLE_SIREN            = true    -- Toggle siren on/off
local SIREN_THRESHOLD_SECONDS = 120.0   -- Play siren when timer reaches this value

🔊 Siren Playback

Uses UE4SS and GameplayStatics to correctly play the 2-minute siren cue:

/Game/Sounds/S_2minSiren_Cue.S_2minSiren_Cue

🧠 Requirements

UE4SS installed

MISERY

Mods enabled via mods.txt

📁 Installation

Place the folder EmissionTimeTweek into:

MISERY/Binaries/Win64/ue4ss/Mods/


Add to mods.txt:

EmissionTimeTweek


Launch the game.

🧪 Status

✔ Stable
✔ Tested with multiple emission cycles
✔ Siren + timer override fully working

📝 License

Free to use and modify. Please credit Ruff Trigger.
