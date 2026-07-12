e0sec | overtsleeping | BroncoCTF 2026 | OSINT

<img src="docs/Digital Crumbs/Screenshot 2026-07-12 at 02-07-03 BroncoCTF.png" alt="alt text" width="406">

> Personally solved: 3
> Attempted: 4
# Challenge Information
**`Admin Abuse | yoshie878 | Easy`**


Some administrator has been going around doing some weird things lately. All they left me were these two cryptic clues. Allegedly, if you follow their trail, they'll lead you to a flag. What gives?

- 1160888390661714032
- <t:1739660340:R>

# Steps
1. <t:1739660340:R> looks like a Discord timestamp. After copy-pasting it into a random message box, we see that it maps to `February 15, 2025 at 4:59 PM (CST)`. This means we are looking for a message sent at that exact time.
2. Filter messages in the official Bronco server (since there's no other server participants could reasonably access).
<img src="docs/Admin-Abuse/image-2.png" alt="alt text" width="531">
The flag is in the message with a spoiler.

<details>
<summary> Flag </summary>
bronco{wh0_g4v3_th15_m4n_3d1t_pr1v1l3g35} 
</details>

# Notes
If I was brighter, I would've just looked for the beginning of the CTF flag format. I wasn't sure whether the timestamp would lead me to an admin message with more clues or directly to a flag, but I should've grabbed the low-hanging fruit first. Also, filtering by a day after the event helps because Discord didn't load a few messages.
1160888390661714032 also references the #announcements channel. Didn't even know you could get a channel's ID.
<img src="docs/Admin-Abuse/image-1.png" alt="alt text" width="486">