<h1 align="center">🏴 NullOrigin CTF 2026 — Grand Finale 🚩</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;size=30&amp;duration=2800&amp;pause=1800&amp;color=55DFBD&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=90&amp;lines=NullOrigin+CTF+2026;Grand+Finale;Played+with+RUY;15th+of+50+finalists;26+challenges+%7C+9+categories;11000+points+solved" alt="NullOrigin CTF 2026 Grand Finale. 26 challenges across 9 categories, 11000 points solved." width="700">
</p>

## About the Event

- 🏫 Organized by **CyberHX**.
- 🏆 The **Grand Finale** of NullOrigin CTF 2026.
- 🏴 Played with **RUY**.
- 🥇 Placed **27th** of 800+ teams in the qualifiers, which put us in the top-50 Grand Finale — where we finished **15th**.
- 📝 26 write-ups across 9 categories, worth **11,000 points** in total.
- 📄 Everything lives in one file: [Null_Origin_Finale_Writeups.md](./Null_Origin_Finale_Writeups.md)

<p align="center">
  <img src="https://img.shields.io/badge/Qualifiers-27th_of_800%2B_teams-2C3E50?style=for-the-badge" alt="Qualifiers: 27th of 800+ teams">
  &nbsp;
  <img src="https://img.shields.io/badge/Finale-15th_of_50_teams-B7950B?style=for-the-badge" alt="Finale: 15th of 50 teams">
</p>

<p align="center">
  <a href="https://ctftime.org/event/3454"><img src="https://img.shields.io/badge/CTFtime-Event_Page-C0392B?style=for-the-badge" alt="CTFtime event page"></a>
  &nbsp;
  <a href="https://ctftime.org/team/444522"><img src="https://img.shields.io/badge/RUY-Member-2C3E50?style=for-the-badge" alt="RUY on CTFtime"></a>
</p>

> [!NOTE]
> Most of the Rev, Pwn, Crypto, Forensic and Steg challenges share one setting — the K7 phase-comparator wall — and each one hides the real flag among **16 candidates**. The other 15 are decoys. Some challenges I solved properly; others I solved by narrowing down the candidates, and the write-up says which.

<br>

## 🧩 Write-ups

### ![Web](https://img.shields.io/badge/Web-D35400?style=for-the-badge&logo=googlechrome&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Kuber](./Null_Origin_Finale_Writeups.md#kuber) | 300 | The root key and unlock pipeline ship in client JS — forge the signature, decrypt the vault offline. |
| [The Oracle](./Null_Origin_Finale_Writeups.md#the-oracle) | 500 | A SHA-512 secret-prefix MAC, so length extension appends `role=oracle_master`. |

### ![Mobile](https://img.shields.io/badge/Mobile-27AE60?style=for-the-badge&logo=android&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Ouroboros](./Null_Origin_Finale_Writeups.md#ouroboros) | 300 | Rebuild the component state and ELF fingerprint to decrypt a two-stage native VM. |
| [Basilisk](./Null_Origin_Finale_Writeups.md#basilisk) | 500 | A tiny ELF loader on Windows runs the real native `derive` over the 4 MB pack. |

### ![Rev](https://img.shields.io/badge/Rev-8E44AD?style=for-the-badge&logo=ghidra&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Beatnote](./Null_Origin_Finale_Writeups.md#beatnote) | 300 | Every decoy file points at a revision — REV P is the only one none of them use. |
| [Octave](./Null_Origin_Finale_Writeups.md#octave) | 300 | The tags aren't truncated hashes, and the engine is missing, so it came down to submissions. |
| [Combtooth](./Null_Origin_Finale_Writeups.md#combtooth) | 500 | 16 candidates in the binary; the 6 with convenient explanations next to them were bait. |
| [Linewidth](./Null_Origin_Finale_Writeups.md#linewidth) | 500 | Drop the self-labelled "unverified" candidates, map the rest back to teeth — tooth 218. |
| [Phaselock](./Null_Origin_Finale_Writeups.md#phaselock) | 800 | The bundle can't be opened; the "image" is really a WAV with nothing hidden in it. |

### ![Pwn](https://img.shields.io/badge/Pwn-C0392B?style=for-the-badge&logo=gnubash&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Escapement](./Null_Origin_Finale_Writeups.md#escapement) | 200 | Readings are checked with 8-byte SHA-256 tags before the sealed ticket picks a flag. |
| [Remontoire](./Null_Origin_Finale_Writeups.md#remontoire) | 300 | Flag-shaped strings everywhere; the real one was sitting in `witness-window.bin`. |
| [Gridiron](./Null_Origin_Finale_Writeups.md#gridiron) | 300 | Several candidates in the ELF, plus a `<=` → `<` bounds fix hinting at the bug. |
| [Fusee](./Null_Origin_Finale_Writeups.md#fusee) | 500 | Five decoys down, then the deployment record's `record:` value. |

### ![Crypto](https://img.shields.io/badge/Crypto-B7950B?style=for-the-badge&logo=letsencrypt&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Randomwalk](./Null_Origin_Finale_Writeups.md#randomwalk) | 500 | A class-group unseal with its inputs never published. |
| [Coda](./Null_Origin_Finale_Writeups.md#coda) | 800 | A VDF with `T = 2^33` and seeds that were "never recorded" — infeasible by design. |

### ![Forensic](https://img.shields.io/badge/Forensic-16A085?style=for-the-badge&logo=wireshark&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Round Robin](./Null_Origin_Finale_Writeups.md#round-robin) | 300 | Recompute D and U for 11 labs — F8's numbers don't hold up. |
| [Cold Start](./Null_Origin_Finale_Writeups.md#cold-start) | 500 | A memory core where the custody status marks the one current epoch. |
| [Guard Frame](./Null_Origin_Finale_Writeups.md#guard-frame) | 500 | Six witnesses in a worklog; only one follows fabric order and the published duty cycle. |
| [Hold Log](./Null_Origin_Finale_Writeups.md#hold-log) | 600 | Rebuild 52 WAL frames with a different salt to recover the hidden revisions. |

### ![Steg](https://img.shields.io/badge/Steg-C2185B?style=for-the-badge&logo=gimp&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Deadband](./Null_Origin_Finale_Writeups.md#deadband) | 300 | Drop the three loudly presented revisions; the dwell times carry no data. |
| [Sidelobe](./Null_Origin_Finale_Writeups.md#sidelobe) | 300 | The roster and the duty log disagree — the session duty log wins. |
| [Interstice](./Null_Origin_Finale_Writeups.md#interstice) | 500 | 16,384 files; skip the grep, ZIP and LSB bait — the answer was plain metadata. |

### ![OSINT](https://img.shields.io/badge/OSINT-2E4053?style=for-the-badge&logo=googlemaps&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [The Wall](./Null_Origin_Finale_Writeups.md#the-wall) | 500 | Match the gate and the street, not the mural, to find the right Messi mural in Rosario. |
| [The map knows the way](./Null_Origin_Finale_Writeups.md#the-map-knows-the-way) | 250 | CyberHX's Maps pin rounded to two decimals; the base64 review is a decoy. |

### ![Misc](https://img.shields.io/badge/Misc-2980B9?style=for-the-badge&logo=hackthebox&logoColor=white)

| Challenge | Points | In one line |
|---|---:|---|
| [Welcome](./Null_Origin_Finale_Writeups.md#welcome) | 50 | Base32 into CyberChef. |
| [FANTASMA](./Null_Origin_Finale_Writeups.md#fantasma--el-punto-final-invisible) | 600 | Probe the basis, then fix one coordinate per round using the collapse error's drift. |

<br>

<p align="center">
  <a href="./Null_Origin_Finale_Writeups.md"><img src="https://img.shields.io/badge/Read_the_full_write--up-24292F?style=for-the-badge&logo=github&logoColor=white" alt="Read the full write-up"></a>
  &nbsp;
  <a href="https://github.com/edda1011/my-ctf-writeups"><img src="https://img.shields.io/badge/←_All_Write--ups-24292F?style=for-the-badge&logo=github&logoColor=white" alt="Back to all write-ups"></a>
</p>

## ⚠️ Disclaimer

These write-ups are for educational purposes only. All challenges were solved in authorized CTF competitions.