# Image Plan & AI Prompts — Andrew Kelly, Nenagh Dentist

The site currently ships with **original SVG artwork and gradient "photo slots"** so it looks
complete and loads instantly, with **zero copyright risk** (no images were copied from any
website or social media). To make it feel fully bespoke, replace the marked slots with real
photography — ideally a professional shoot at the practice.

> **Best option:** a 2–3 hour local photoshoot of the real practice, team and (consenting)
> patients. Nothing builds trust like genuine local faces. Use the AI prompts below only as a
> fallback until real photos are available.

Recommended photography style throughout: **natural light, warm and airy, shallow depth of
field, authentic candid moments, soft teal/cream tones to match the brand.** Avoid stiff,
overly-clinical stock imagery.

---

## Where each image goes

| Page | Location | Slot in code | Purpose |
|------|----------|--------------|---------|
| Home | Hero (right card) | `.hero__card` | Warm, welcoming first impression |
| Home | Problem/solution | `.split__media` (1st) | Reassure nervous patients |
| Home | Why choose us | `.split__media` (2nd) | Show the caring team |
| About | Story section | `.split__media` | The practice on O'Rahilly Street |
| About | Team cards | avatar circles | Real headshots of each team member |
| Services | (optional) | add above grid | Treatment-in-progress detail shots |
| Contact | Map | already live Google embed | Location |

**Export specs:** hero ~1200×1320px; split images ~1000×840px; team headshots 400×400px
(square). Save as **.webp** (with .jpg fallback), compress to < 200 KB each, and add
descriptive `alt` text (examples already in the HTML comments).

---

## AI image prompts (fallback only)

**1. Hero — welcoming practice**
> Bright, modern dental reception in a small Irish town practice, warm morning light through a
> front window, soft teal and cream colour palette, a friendly receptionist smiling naturally,
> tasteful plants, shallow depth of field, editorial lifestyle photography, calm and premium,
> 35mm, natural skin tones, no text.

**2. Problem/solution — reassured patient**
> A relaxed middle-aged patient smiling and chatting with a dentist in a calm treatment room,
> soft natural light, teal accents, genuine unposed moment conveying trust and comfort, warm
> tones, shallow depth of field, documentary lifestyle style, no dental gore, no text.

**3. Why choose us — the team**
> A small friendly dental team of 2–3 people standing together in a bright practice, warm
> genuine smiles, clean uniforms, teal and cream interior, soft window light, approachable and
> professional, editorial portrait, 50mm, natural colour grade, no text.

**4. About — the practice exterior/interior**
> Cosy, welcoming dental practice interior on a traditional Irish town street, exposed warmth,
> plants and soft seating in a waiting area, teal and cream tones, bright and airy, real-estate
> editorial photography, inviting, no text.

**5. Team headshots**
> Professional friendly headshot of a dentist against a soft neutral teal-grey background, warm
> approachable smile, natural light, shallow depth of field, high-end corporate portrait,
> square crop, no text.

**6. (Optional) Treatment detail**
> Close, tasteful detail of gloved hands preparing clean modern dental instruments on a tray,
> soft focus, bright hygienic environment, teal accents, calm and premium, macro lifestyle
> photography, absolutely no blood or distressing content, no text.

---

## Consent & rights checklist
- [ ] Written model-release consent from any patient or staff member shown.
- [ ] Only use photos you own or have a clear licence for.
- [ ] Do **not** reuse images from competitor sites, Google, or social media.
- [ ] Compress and convert to .webp before uploading.
- [ ] Add meaningful `alt` text to every image for accessibility & SEO.
