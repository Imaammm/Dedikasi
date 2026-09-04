# DEDIKASI 2026

Official information portal for DEDIKASI 2026 by Himpunan Mahasiswa Sipil Universitas Hasanuddin.

## Local development

```bash
npm install
npm run dev
```

Open `http://localhost:3000`.

## Validation and production build

```bash
npm run lint
npm run typecheck
npm run build
npm run start
```

## Updating official information

- Google Form URLs: `data/registration.ts`
- Competitions, guidebook status, fees, team size, and prizes: `data/competitions.ts`
- Seminar and public lecture details: `data/events.ts`
- Master timeline: `data/timeline.ts`
- Downloadable resources: `data/resources.ts`
- Contact and organizer information: `data/site.ts`
- Social URLs: `data/socials.ts`
- Partners: `data/sponsors.ts`
- FAQ: `data/faq.ts`

When an official Google Form becomes available, replace the corresponding `null` in `data/registration.ts`. `RegistrationButton` will automatically change from a disabled “Registration Coming Soon” state to an external registration link.

## Official assets

Assets live under `public/assets`. The repository currently includes local SVG placeholders for the official DEDIKASI, COASTEC, VISION, Seminar Nasional, and Kuliah Umum logos. Add the official files under `public/assets/logos` and update their paths in `data/competitions.ts`, `data/events.ts`, `components/layout/Navbar.tsx`, and `components/layout/Footer.tsx` as appropriate. Preserve the logo aspect ratio.

Guidebook and template files may be placed under `public/assets/documents`; then set their public URLs in the relevant data file, for example `/assets/documents/coastec-guidebook.pdf`.
# Dedikasi
