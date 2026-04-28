# Claude Code — First Prompt to Paste

Paste this into Claude Code when you first run `claude` in the wedding-handoff folder:

---

I'm handing off a wedding coordination app to you. Read CONTEXT.md first for full context.

The app is index.html — a single HTML file wedding hub for Mani + Navi's wedding on 22 May 2026.

Please do the following in order:

1. **Read CONTEXT.md** so you understand the full situation
2. **Deploy index.html to GitHub Pages** — create a repo called `wedding-hub`, push the file as index.html, enable GitHub Pages, give me the live URL
3. **Test that buttons work on Safari** — the file must use no fixed heights on body/html, no overflow:hidden, pure ES5 JS only (no arrow functions, no async/await, no const/let if possible)
4. **Confirm the live URL** so I can share it with family

After that, I'll give you ongoing updates like:
- "Mark baraat cars as confirmed"
- "Add new guest: [name]"  
- "Process this brain dump: [text]"

And you'll update index.html and redeploy each time.

---

## Quick Reference — Key Things Claude Code Needs to Know

- App uses localStorage (per device) — Supabase integration is optional upgrade later
- All data is seeded in init() function inside the <script> tag
- Guests are in sv('g', [...]) array — fields: id, n (name), r (relation), c (count), rv (RSVP), ac (accommodation), tr (transport), ev (events object), nt (notes)
- Tasks are in sv('t', [...]) — fields: id, d (description), a (assigned), du (due date), p (priority: urgent/soon/later), s (status: todo/inprogress/done), n (notes)
- Vendors are in sv('v', [...]) — fields: id, n, c (category), ct (contact), co (cost), s (status), nt (notes)
- Decision log in sv('l', [...]) — fields: id, d (decision), c (category), b (decided by), dt (date)
