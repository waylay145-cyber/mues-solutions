# Mues Solutions Website

Trusted Home Maid & Caregiving Services — Nairobi, Kenya

---

## ✅ How to Edit Staff (No Coding Needed!)

1. Go to your GitHub repo → **github.com/waylay145-cyber/mues-solutions**
2. Click on **`staff.json`**
3. Click the **pencil icon ✏️** (top right of the file)
4. Make your changes (see guide below)
5. Scroll down → click **"Commit changes"**
6. Your live website updates automatically in ~30 seconds ✅

---

## 📋 staff.json Field Guide

Each staff member looks exactly like this:

```json
{
  "id": 1,
  "name": "Lewis Murong'a Kariuki",
  "role": "Caregiver",
  "type": "Caregiver",
  "av": "yes",
  "rate": "KSh 1,100/day",
  "exp": "2 yrs",
  "loc": "Nairobi CBD",
  "phone": "0794 324 724",
  "skills": ["Disability Care", "Companionship", "Meal Prep", "Safe Handling"],
  "rating": "4.9",
  "initials": "LK",
  "avc": "av-teal",
  "bio": "Short description of the person..."
}
```

| Field      | What to put                                                                 |
|------------|-----------------------------------------------------------------------------|
| `id`       | Unique number — count up from the last one (1, 2, 3...)                     |
| `name`     | Full name                                                                   |
| `role`     | Job title e.g. `"Caregiver"`, `"Senior Caregiver"`, `"House Maid"`         |
| `type`     | Must be exactly: `"Caregiver"`, `"Maid"`, or `"Nanny"` (controls filter)   |
| `av`       | `"yes"` if available now, `"no"` if currently engaged                       |
| `rate`     | e.g. `"KSh 1,100/day"`                                                     |
| `exp`      | e.g. `"2 yrs"` or `"6 yrs"`                                                |
| `loc`      | Area in Nairobi e.g. `"Westlands"`, `"Karen"`                              |
| `phone`    | Their personal phone number e.g. `"0712 345 678"`                          |
| `skills`   | List in square brackets, each skill in quotes, separated by commas          |
| `rating`   | A number in quotes between `"1.0"` and `"5.0"` e.g. `"4.9"`               |
| `initials` | 2 letters from their name e.g. `"LK"` for Lewis Kariuki                    |
| `avc`      | Avatar colour — pick ONE: `av-teal` `av-amber` `av-blue` `av-coral` `av-purple` `av-green` |
| `bio`      | A short paragraph about them (1–3 sentences)                                |

---

## ➕ Adding a New Staff Member

1. Open `staff.json` on GitHub → click ✏️
2. Go to the **end of the last staff block** — find the last `}` before the final `]`
3. Add a **comma** after it, then paste a new block:

```json
  ,
  {
    "id": 7,
    "name": "New Person Name",
    "role": "Caregiver",
    "type": "Caregiver",
    "av": "yes",
    "rate": "KSh 1,100/day",
    "exp": "1 yr",
    "loc": "Nairobi CBD",
    "phone": "07XX XXX XXX",
    "skills": ["Skill One", "Skill Two", "Skill Three"],
    "rating": "4.8",
    "initials": "NN",
    "avc": "av-teal",
    "bio": "Description of the new person here."
  }
```

4. Click **"Commit changes"** — done! ✅

---

## ➖ Removing a Staff Member

Delete their entire block: from `{` all the way to the closing `}` including the comma before it. Make sure you don't leave a trailing comma on the last item.

---

## 🔄 Changing Availability

Find the person's block and change:
- `"av": "yes"` → shows green **Available** badge
- `"av": "no"`  → shows orange **Engaged** badge

---

## 📁 Files in This Repo

| File         | Purpose                              | How often you edit it        |
|--------------|--------------------------------------|------------------------------|
| `staff.json` | All staff data                       | Every time staff info changes |
| `index.html` | The website design & logic           | Rarely — design changes only  |
| `README.md`  | This guide                           | Never                         |

---

## 📞 Contact Details (in index.html)

Your WhatsApp bookings go to: **+254 794 324 724**  
To change this, search for `254794324724` in `index.html` and replace it.
