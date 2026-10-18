# CINDERPRINT

**Fire erased the truth. The shadows kept it.**

A 3D first-person forensic fire reconstruction mystery where the player investigates a burned apartment, recovers temporal traces, identifies contradictions, reconstructs the causal timeline, and determines the true cause of the fire.

## Themes

- **Fire** — physical fire evidence and burn reconstruction
- **Shadow** — Temporal Shadows and missing traces
- **Time** — timestamps, causal order, and reconstruction

## Play on Windows

The competition build is a **Windows x86_64 standalone** application. Unity Editor is not required to play.

1. Download [CINDERPRINT_Windows_v1.0.zip](CINDERPRINT_Windows_v1.0.zip).
2. Extract the entire archive to a local folder.
3. Open the extracted `CINDERPRINT` folder and launch `CINDERPRINT.exe`.

Keep `CINDERPRINT_Data`, `UnityPlayer.dll`, `MonoBleedingEdge`, and all other extracted runtime files alongside the executable. Do not launch from inside the ZIP or move only the executable.

The game starts at Boot and opens the Main Menu. Choose **How To Play** for the investigation guide or **Play Case** to begin Case 001 through its opening cinematic. Settings, Credits, and Quit are available from the menu; Esc opens the in-case pause menu.

## Controls

| Input | Action |
| --- | --- |
| WASD | Move |
| Mouse | Look |
| Shift | Sprint |
| Space | Jump |
| E | Interact |
| F | Scanner |
| Esc | Pause |

## Open and build the Unity project

**Unity version: `6000.6.6f1`**

1. Install this Editor version through Unity Hub with **Windows Build Support**.
2. Clone or download the project, then add its root folder to Unity Hub. The root contains `Assets`, `Packages`, and `ProjectSettings`.
3. Open it with Unity `6000.6.6f1`. Allow Unity to restore the locked packages and regenerate its local Library.
4. For an Editor launch, open `Assets/_Game/Scenes/00_Boot.unity` and press Play.
5. To create a standalone player, open **File → Build Profiles**, select **Windows**, and use **Intel 64-bit / x86_64** architecture.
6. Verify the enabled scenes appear in this order:

   1. `Assets/_Game/Scenes/00_Boot.unity`
   2. `Assets/_Game/Scenes/01_MainMenu.unity`
   3. `Assets/_Game/Scenes/01_Case001_Intro.unity`
   4. `Assets/_Game/Scenes/02_Case001.unity`
   5. `Assets/_Game/Scenes/03_Case001_Ending.unity`

7. Use Product Name **CINDERPRINT**, Company Name **Shehryar Aslam**, version **1.0**, and the existing assigned icon. Leave graphics and audio settings as authored.
8. Disable **Development Build**, **Script Debugging**, and **Autoconnect Profiler**. Build to `Builds/Windows/CINDERPRINT/CINDERPRINT.exe`.
9. Distribute the complete generated `CINDERPRINT` folder. The submitted ZIP contains that folder and its runtime dependencies.

`Packages/manifest.json` and `Packages/packages-lock.json` define the project's dependencies. The `Library`, `Temp`, `Logs`, IDE caches, local tools, and uncompressed builds are excluded from version control; Unity recreates its generated data locally.

## Credits

- **Development by Shehryar Aslam**
- **Game Design by Ayyaz Ahmed**
- **Engine made with Unity**

## Third-party attribution and licenses

See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for the submission notice index and [the existing asset register](Assets/_Game/ThirdParty/ASSET_LICENSES.md) for detailed provenance.

| Component | Creator / provider | License / record |
| --- | --- | --- |
| Appartement environment | SrMonteiro | CC BY 4.0; [attribution and modification notice](Assets/_Game/ThirdParty/Appartement/ATTRIBUTION.txt) |
| Surface textures | Poly Haven; Amal Kumar, Guillaume Monsergent, Rob Tuytel | CC0 1.0; [download manifest](Assets/_Game/ThirdParty/PolyHaven/download-manifest.json) |
| Barlow Condensed | The Barlow Project Authors | [SIL Open Font License 1.1](Assets/_Game/UI/MainMenu/Fonts/Barlow-OFL.txt) |
| Share Tech Mono | Carrois Type Design / Ralph du Carrois | [SIL Open Font License 1.1](Assets/_Game/UI/MainMenu/Fonts/ShareTechMono-OFL.txt) |
| Nathan Animated 003 Walking | Renderpeople GmbH | Proprietary Renderpeople terms; redistribution review required for source assets |
| Menu background | AI-assisted adaptation of a user-supplied visual | [Existing provenance note](Assets/_Game/UI/MainMenu/MENU_ASSETS.md); source-reference rights confirmation pending |
| Background music | Provenance not recorded locally | Rights/source confirmation pending |

Third-party assets retain their respective terms. No blanket open-source license is granted by this submission. **Public source publication is pending the rights checks listed in [SUBMISSION_CHECK.md](SUBMISSION_CHECK.md)**, particularly permission to distribute the Renderpeople source and derived assets. The local project and playable build have been preserved unchanged.
