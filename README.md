```text
  _  _   _ ___ ___ ___  _   _ ___   _  _ ___ _  _ ___  __  ___

 |_)|_|_|\| |  |_) |__)/_\ |\| |   |_|/_\ |  |\| |  \|  \(_ 
 |  |__ | | |  | \ |__ \_/ | | |   | | _/ |  | | |__/|__/__)
 -------------------------------------------------------------
```
 [========= GLOBAL NETWORK & PHYSICS ADDON v1.0.0 =========]


# 🧗‍♂️ PEAK VR Hands Mod — Global Network & Physics Addon (v1.0.0)

Welcome to the global network and physics expansion for the original **PEAK VR** mod! This addon transforms a basic visual VR plugin into a fully-featured cooperative climbing simulator with real physics interaction.

---

## 🤝 Credits & Disclaimer

**Huge thanks and maximum respect to the original VR mod author on GitHub!(https://github.com/AstienVR)** Thank you for building the amazing base that made it possible to run the game in virtual reality and brought the controllers to life on a local PC.

> 💡 **Why this addon was created:**
> The original creator deliberately chose not to add multiplayer or free finger tracking over the network to prevent toxic behavior from younger players. I completely respect his position and rules, but as a developer, I couldn't ignore the massive potential of cooperative climbing. This addon was created solely for **honest teamwork, scaling peaks with friends, and hardcore physics climbing**. Please use this mod respectfully!

---

## 🛠️ Base Mod Features (Preserved from the original author):
* Full first-person VR mode support.
* Head and hand tracking in space via VR controllers.
* Automatic basic initialization of the BepInEx mod loader inside the game engine.

---

## 🚀 Addon Features (New in v1.0.0):

### 1. 🎛️ Free 5-Finger Network Sync
Your hands are now fully alive! The network integration (`VRHandSender` -> `VRHandReceiver`) broadcasts every finger position in real-time using the UDP protocol on port `7777`.
* You can show any gestures, clench fists, make **"finger guns"** 👈, point directions, or wave at your friend.
* All gestures smoothly bend the bones of the 3D character model on other players' screens!

### 2. 🧗‍♂️ True Physics Hand Climbing
Forget about pressing keys on your keyboard — now you scale the cliff using your own strength!
* Bring your hands close to the wall and squeeze the controllers tightly (**`Grip > 0.85f`**) to lock your hand onto the surface.
* Move your hands down one by one ("step-by-step"), physically pulling your body up to the summit!

### 3. 🛑 Advanced Surface & Angle Protection
The mod features strict physical surface logic to eliminate cheating and glitches:
* **You cannot climb smooth walls or ceilings!** The code reads surface tilts.
* You can only grab **fair climbing zones and ledges** designed for mountaineering. Your hands will slip on slippery concrete or glass.

### 4. 🤝 Physical "Helping Hand" Mechanic
Teamwork has reached a whole new level!
* If your friend slips or can't reach a ledge, you can **physically extend your hand to them**.
* The bone detection system reads the grip, triggers the game event, and you can literally pull your buddy out of the abyss with your own hands!

### 5. ⚡ In-Game Stamina Integration
No free rides — the mod is fully synchronized with the character's native energy system:
* While you are hanging on a cliff or holding a friend, the game gradually **drains your stamina bar**.
* If your stamina drops to zero, your hands will automatically open, physical anchors will release the wall, and your character will fall!

---

## 🎮 How to Play in a Big Group (Up to 20 Players — VR and PC):

The mod is fully optimized and tested for stable play in large lobbies **up to 20 players simultaneously**! The lobby can have any mix of players (some in VR headsets, some on regular computers).

Thanks to this setup, **every single player in the room will see everything perfectly**: you will see your own hands, your VR friends will see their hands, and all PC players on their monitors will see the exact hand movements and climbing physics of every VR player in the lobby.

In the **Releases** section, two ready-to-use packages are prepared for your convenience:
* **`friend(VR)+friend(VR).zip`** — If you have a VR headset.
* **`friend(VR)+friend(PC).zip`** — If your friend plays from a regular computer with a monitor (the PC version has heavy VR components removed so your friend's game runs smoothly without lag).

---

## 🔧 Network Setup (Choose your option):

### 📌 OPTION №1: If you play AS A DUO (1v1)
*This option is for exactly two players: VR + VR or VR + PC.*

1. Download the required ZIP archive from the **Releases** section and drop the `BepInEx` folder into the game root.
2. Launch **Radmin VPN** on both computers and join the same virtual room.
3. Setup the **`vrhand_config.txt`** files in the `BepInEx \ plugins` folder "cross-wise":
   * **You** open the Notepad file and type **your friend's IP address** from Radmin VPN.
   * **Your friend** opens the Notepad file and types **your IP address** from Radmin VPN.
   * *Note: If your friend plays from a regular PC, they don't need to touch any Notepad files at all (they don't have it)! Only the VR player edits the file by entering the PC player's IP.*
4. Press **Ctrl + S** to save, close the Notepad, and start climbing. You will perfectly see each other's hands!

### 📌 OPTION №2: If you play IN A BIG PARTY (Up to 20 Players)
*This option is for massive climbing sessions with a crowd on the mountain.*

1. All 20 players download their respective archives (VR or PC) and drop the `BepInEx` folder into the game root.
2. All players join the same network room in **Radmin VPN**.
3. Choose one main person to be the **Host (the one who creates the game room)**.
4. Editing the **`vrhand_config.txt`** file (Done ONLY by players in VR headsets):
   * Every VR player opens their Notepad file in the `plugins` folder.
   * **All VR players must enter the exact same IP address — the main Host's IP address from Radmin VPN!**
   * The Host enters the IP address of their main VR friend.
5. Press **Ctrl + S** to save and close the Notepad.

*🛑 **PC FRIENDS DO NOT NEED TO CONFIG ANYTHING:** All your 10–15 friends playing on regular monitors do not touch any Notepad files. Their mods will automatically catch all hand movements from the Radmin VPN network!*

---

### 🔍 How to quickly find your own IP address for a friend (Hacker Method):
To instantly find and copy your exact IP address inside Windows, do the following:
1. Press the **`Win + R`** key combination on your keyboard.
2. Type the following command into the "Run" window: **`cmd /k ipconfig`** and hit **Enter**.
3. A black console window will open and stay active. Look for the line that says **IPv4 Address** (e.g., `192.168.1.50`).

---

## 📺 Video Guide for those who are confused:

If you are stuck, cannot find the right line in the Notepad, or don't understand where exactly to paste the IP numbers — I recorded a detailed step-by-step video guide for you!

* 👉 **[WATCH THE IP SETUP VIDEO GUIDE (https://youtu.be/unyc9IMXfzU?si=uND6XpnmOO74BDnO)** 🎬

*(The video is uploaded via a private link and is accessible only to GitHub users!).*

---
### 📧 BE A BETA TESTER!
My PC is too weak for full scale testing, so I need your help! 
Please test this mod with your friends and send your feedback or bug reports to my email:
👉 [ВСТАВЬ_СЮДА_СВОЮ_ПОЧТУ] 👈
Thank you for helping me make this mod better! 🙏
---
Created with love for VR technologies and hardcore climbing. See you at the summit! 🚀
