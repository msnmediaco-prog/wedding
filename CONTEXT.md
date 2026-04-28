# Mani + Navi Wedding Hub — Claude Code Handoff

## The App
A wedding coordination hub for Mani + Navi's wedding, May 2026, Melbourne & Sydney.
Single HTML file (index.html) — no framework, pure HTML/CSS/ES5 JS, localStorage for data.
All data is pre-seeded on first load (guests, tasks, vendors, decision log).

## Your Job
1. Deploy index.html to GitHub Pages → permanent free URL
2. Ensure all buttons work on Safari iPhone (no fixed heights, no overflow:hidden, no modern JS)
3. Set up workflow: Mani tells you updates → you edit index.html → redeploy automatically

## The Wedding
- **Groom:** Mani | **Bride:** Navi (Navleen)
- **Locations:** Melbourne (pre-events) + Sydney (wedding)
- **Key date:** Friday 22 May 2026 — Anand Karaj at Glenwood Gurdwara NSW

## 6 Events
| Event | Date | Location | ~Heads |
|-------|------|----------|--------|
| Sukhmani Paath | Sat 16 May | Bickhams Left Unit, St Kilda East VIC | ~81 |
| Maiyan / Vatna | Mon 18 May | Bickhams Right Unit, St Kilda East VIC | ~46 |
| Mehndi | Tue 19 May | Bickhams VIC → depart Sydney 9pm | ~28 |
| Jaggo | Wed 20 May | Londonderry NSW (Khera family hosts) | ~53 |
| ✨ Anand Karaj | Fri 22 May | Glenwood Gurdwara NSW ✅ confirmed | ~52 |
| Reception | Sun 24 May | Ultima Function Centre VIC | ~200 |

## 🚨 Urgent Tasks (as of 28 Apr 2026)
1. Book 2–3 black baraat cars with ribbons — Glenwood Gurdwara 22 May (Dad's top priority)
2. DJ call tonight 7–8pm — lock package (Elite $6k / Platinum $4.5k / Diamond $2.5k / Emerald $1.5k / Standard $800)
3. White Diamond Palace courier — confirm if arrived
4. Marquee hire — confirm status (Mum got quote $950 Dandenong, Tarun getting 3 quotes)
5. Mithai 150kg — who orders/packs/stores? Lock by 12 May
6. Mattress details from Mum — how many, which rooms at Bickhams right unit
7. Book Airbnb Sydney for Canada (6) + NZ (6-8) guests — NO beds confirmed
8. Assign command roles — Transport/Food/Accommodation/Event leads (Dad's request: 1 person per job)

## Key People
- **Mani** — groom, main coordinator
- **Navi** — bride
- **Dad** — patriarch, high priority voice in WhatsApp, focused on baraat + upper responsibilities
- **Mum** — logistics, accommodation, catering sorted
- **Jas (Sister)** — groom's side, booked makeup/hair for bridal party
- **Grover + Family** — food/catering responsibility
- **Shota** — van driver confirmed (Melb→Sydney 19 May)
- **Nagi** — researching home speaker (NOT DJ)

## Guests Summary
- 37 guest groups loaded in app
- Confirmed: Mani, Ajmer, Raj, Jas, Gurnam, Mohinder, Amritpal, Nagi, Grover, Rupika, Shota, Emanuel, Shawqi, John Ho, Baljeet (UK), Satti Bhaji (CAN), Harpreet (CAN)
- TBC: Kanika, Tejinder, Surinder, Manpreet+Jaiveer, Yad, Pabi, Amrinder, Pamma Nijjar, Roger, Suba, Kuldeep (UK), Pinky (UK), Bholi Didi/Niku/Aman (Canada), all India guests, all NZ guests
- Overseas: UK (3 groups), Canada (5 groups), India (2 groups), NZ (2 groups)

## Accommodation
### Melbourne — Bickhams
- Unit 1 (Left): Furniture hired via Click Rentals (Peter: 03 9362 1818)
- Unit 2 (Right): Room 1 → Gurpreet family, Room 2 → Satu paji + Saberwal, Room 3 → Supreet family
- Post-reception houses: Bickhams (elders), Altona North, Slinky St (10-13 mattresses), Kandy house, Suni house

### Sydney
- Oakville Airbnb ✅ (4 nights, core family — capacity >8 unconfirmed)
- Kimberley Hotel ✅ (12 rooms, $976 + 1.8%, card on check-in 24 May)
- Penrith Hotel ✅ (extra room)
- ❗ Canada + NZ guests — NO accommodation booked

## Confirmed Vendors
- Shota (van driver) ✅
- Gurdwara catering 16 May ✅ (~$875 via Ajay)
- Catering 18 + 25 May ✅ (Ajay)
- House help 16–19 May + 25 May ✅
- Kimberley Hotel ✅
- Oakville Airbnb ✅
- Dhol player ✅
- Photographer ✅
- Makeup/hair — Jas booked for Nav, Raj, Jas, Aman, Harpreet ✅
- Carpet cleaning Clematis (Wednesday 11am) ✅

## Pending Vendors
- ⚠️ Baraat cars (black + ribbons) — NOT booked
- ⚠️ DJ package — call tonight
- ⚠️ White Diamond Palace / Khalsa decorations — courier unknown
- ⚠️ Marquee hire — status unknown
- ⚠️ Click Rentals mattresses — pending Mum info
- ⚠️ Wedding cake — search ongoing, not booked

## 14 Blind Spots
1. Milni list — family pairings for Gurdwara ceremony
2. MC for reception — not confirmed, no script
3. Wedding cake — not booked
4. Seating plan — 200 people, not started
5. Entry + first dance songs — not locked with DJ
6. Family photo list — not given to photographer
7. Airport pickup plan — flight times not collected from overseas guests
8. Travel food — Melbourne→Sydney van not planned
9. Giveaways — who packs + distributes at venue exit
10. Cultural items checklist — Chunni chadai 21 May
11. Shagan envelope amount — not confirmed with Mum
12. Command roles — not assigned to real names
13. White Diamond Palace courier — arrived or not?
14. Backup plans — vendor cancels, no contingency named

## App Structure (index.html)
- **Home** — urgent panel, countdown to 22 May, 6 events (tap to expand: heads/transport/accommodation/who's attending)
- **Guests** — 37 guests, filter by group/RSVP, tap to see event attendance grid + update RSVP
- **Tasks** — 32 tasks, filter by priority, tap to mark done/in progress/edit
- **Vendors** — 15 vendors by category + Decision Log + Room/Accommodation view
- **Hub** — Brain Dump (free text input), Blind Spots, WhatsApp message template, RSVP chase list

## Tech Notes
- Pure HTML/CSS/ES5 JavaScript — NO frameworks, NO external scripts
- localStorage for persistence (per device — not shared across phones)
- Safari fix: no fixed heights on body, no overflow:hidden, no arrow functions, no async/await
- To make shared/live: add Supabase (URL: https://pecvorberttcojnkdgpm.supabase.co, tables: guests/tasks/vendors/brain_dumps/decision_log already created)
- Supabase anon key available if needed for live sync feature

## Deployment History
- Netlify: mani-navi-wedding.netlify.app (paused — exceeded free credits due to Claude Agent)
- Target: GitHub Pages (free, permanent, no limits)

## Update Workflow (for Claude Code)
When Mani says:
- "Mark X as done" → update task status in index.html seed data
- "Add guest Y" → add to INITIAL_GUESTS array
- "X vendor confirmed" → update vendor status
- "New brain dump: [info]" → process and update relevant data
- Always redeploy after changes via `git push` to GitHub Pages
