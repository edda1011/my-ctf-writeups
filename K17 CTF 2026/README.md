<h1 align="center">🏴 K17 CTF 2026 🚩</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;size=30&amp;duration=2800&amp;pause=1800&amp;color=55DFBD&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=90&amp;lines=K17+CTF+2026;Hosted+by+UNSW+SecSoc;Played+with+EDNK;5+challenges+solved" alt="K17 CTF 2026, hosted by UNSW SecSoc, played with EDNK." width="700">
</p>

## About the Event

- 🏫 Hosted by **UNSW SecSoc**.
- 🏴 Played with **EDNK**.
- 📝 Five write-ups — one Pwn, two Rev, one Forensic, one Misc.

<p align="center">
  <a href="https://ctftime.org/event/3145"><img src="https://img.shields.io/badge/CTFtime-Event_Page-C0392B?style=for-the-badge" alt="CTFtime event page"></a>
  &nbsp;
  <a href="https://ctftime.org/team/448296"><img src="https://img.shields.io/badge/EDNK-My_Team-2C3E50?style=for-the-badge" alt="EDNK on CTFtime"></a>
</p>

<br>

## 🧩 Write-ups

### Big-win

![Pwn](https://img.shields.io/badge/Pwn-C0392B?style=flat-square)

> No reversing, no libc leak, no ROP — one `scanf` whose index you can quietly steer.

- Walk the array index into the negatives and you write straight back over `win`.
- The handout even ships a ptrace man page, because the setter built us a stack printer.

[![Read the write-up](https://img.shields.io/badge/Read_the_write--up-24292F?style=for-the-badge&logo=github&logoColor=white)](./Pwn_big-win.md)

---

### Evilgram

![Rev](https://img.shields.io/badge/Rev-8E44AD?style=flat-square)

> A villain's chat app where the message isn't text — it's a 3D animation of little cubes.

- `evilgram.html` is a fake chat client; only two conversations actually matter.
- The 4x4x4 grid over 128 frames is the ciphertext, and the other chat hides the key.

[![Read the write-up](https://img.shields.io/badge/Read_the_write--up-24292F?style=for-the-badge&logo=github&logoColor=white)](./Rev_evilgram.md)

---

### Srev

![Rev](https://img.shields.io/badge/Rev-8E44AD?style=flat-square)

> A stripped VM that advances by asking the kernel to return from a signal it never received.

- Run it forward and it spins forever — the platform just reports `Time Limit Exceeded`.
- Every "instruction" is a frozen CPU snapshot, so the whole thing unravels once you read it backwards.

[![Read the write-up](https://img.shields.io/badge/Read_the_write--up-24292F?style=for-the-badge&logo=github&logoColor=white)](./Rev_srev.md)

---

### Get fixed boi

![Forensic](https://img.shields.io/badge/Forensic-16A085?style=flat-square)

> A Terraria world save from a friend who's "definitely not cheating" — except it won't open.

- `grep` for the flag finds nothing: it isn't text, it's painted into the world in blocks.
- Repair the broken save, render the map, and read the flag off the tiles.

[![Read the write-up](https://img.shields.io/badge/Read_the_write--up-24292F?style=for-the-badge&logo=github&logoColor=white)](./Foren_get-fixed-boi.md)

---

### Verify you are human

![Misc](https://img.shields.io/badge/Misc-2980B9?style=flat-square)

> Two confiscated phones, 16 leaked photos, and all the metadata stripped.

- Five known photos per camera, and every query photo has to be matched to Camera A or B.
- The "very scary photos" turned out to be hand-drawn doodles of a capybara. Or a hamster.

[![Read the write-up](https://img.shields.io/badge/Read_the_write--up-24292F?style=for-the-badge&logo=github&logoColor=white)](./Misc_verify-you-are-human.md)

---

[![Back to all write-ups](https://img.shields.io/badge/←_All_Write--ups-24292F?style=for-the-badge&logo=github&logoColor=white)](../)

## ⚠️ Disclaimer

These write-ups are for educational purposes only. All challenges were solved in authorized CTF competitions.