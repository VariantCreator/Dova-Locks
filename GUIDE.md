# Dova Locks 1.1.2 guide

[Quick start](README.md)

## Get started

Close ICARUS and stop the server. Put `Dova-Locks_P.pak` in `Icarus/Content/Paks/mods`, creating the mods folder if needed. Replace the old PAK and keep one copy. **The server and every player need the same file.** Back up your prospect and both A/B lock saves before updating.

For a regular lock, look at a supported door, window, container or bench. Hold **Shift**, then hold your **Interact key**. That's F by default, or your custom key. Set four digits and use **Link connected base** to protect the connected structure.

## Dova's Ward

Craft it where you craft the Flow Meter, using the same materials. Place it and **tap Interact** to use its screen. A new PIN turns protection on. Owners and co-owners can set its radius from **1 to 60 m**, name it, and show or hide the boundary.

A new Ward on your own linked base reuses its PIN and access. Changes to shared access carry across both. An existing linked base remains protected beyond the Ward radius, and removing the Ward lock does not remove that separate base lock. The menu tells you when it is still active.

Check nearby protection for a 12-second view: **green has an active lock; red has none**. It covers loaded build pieces within 70 m, up to 128 objects. Show nearby Wards displays boundaries within 150 m. Hiding a boundary does not turn protection off.

The Ward covers your base, placed equipment and loot bags. Mining, chopping trees and dealing with wildlife work normally. Storms still get a vote. Players with the right access can damage their own protected stuff.

## Joined Wards and personal display

Up to three touching Wards with the same owner join their boundaries and share a name and player access. Another owner's claim cannot be absorbed. The menu tells you when a group has reached its three-Ward limit.

Each Ward keeps its own PIN. Installing or changing one does not replace the other devices' PINs. A new Ward can still inherit its owner's linked-base PIN when first placed. Removing a Ward lock turns that Ward off and keeps its lock removed until you explicitly install it again. Other Wards, linked base locks and separate private locks keep their protection.

Open **Your Ward Display** for color, opacity and brightness. These are personal visual settings; they do not change anyone's protection. Joined Wards have one named lock marker on the map.

**Transfer Ownership** is a dropdown in both menus. Confirm the new owner's 17-digit Steam ID to transfer the claim, its linked base and joined Wards. PINs stay unchanged, the previous owner keeps Member access, and other players' private locks stay separate.

## Who can do what?

- **Guest:** Repair, but no protected access or building changes.
- **Associate:** Repair and use doors, windows and benches. This is the starting role after entering a PIN.
- **Member:** Shared storage, building, upgrades, pickup and crop removal.
- **Co-owner:** Member access, plus managing locks, Ward settings and access.
- **Owner:** Full control, including assigning roles.

Access is remembered. Owners and co-owners can give storage a private lock inside a shared base or Ward. Members can also private-lock chests they personally placed, including after being granted Member access later. They cannot claim someone else's chest. Placement tracking starts in 1.1.2; older chests with no recorded placer need an authorized pickup and placement again first.

## Server admins

Use the game's `/AdminLogin` with the server admin password, reopen lock controls and choose **Server Admin**. Stand within 5 m of the selected object.

The opening override lasts five minutes. It allows opening protected objects in the selected claim, not damage, pickup or building. Its status is shown in the panel; **End My Override** stops it early.

PIN recovery, disabling a Ward and removing a selected lock require confirmation. Removing or disabling the selected protection also ends your opening override. Other locks may still protect that area. Recent activity is a short, collapsible list; PINs and passwords are not logged.

## Saves and support

The host holds the world's lock saves, usually under `%LOCALAPPDATA%/Icarus/Saved/SaveGames`. Look for `DovaLocks_..._A.sav` and `_B.sav`. Some server hosts use a different Saved folder.

Stop the server before editing. For a remote server, download both saves, edit them with the Organizer, then upload both replacements. Editing a client's local files does not edit a remote server.

Missing or mismatched client versions are rejected. ICARUS may still show error **028**; detailed DL001/DL002 reasons are in the server log.

Other mods can conflict if they change the same assets. The Organizer handles PAKs; it does not merge them. Game updates may need a mod update.

[Report a problem](https://github.com/VariantCreator/Dova-Locks/issues) with your version, what happened and any other mods involved. Logs and screenshots help. A screenshot of your PIN helps the wrong people, so leave that out.

Unofficial community mod. ICARUS belongs to RocketWerkz.
