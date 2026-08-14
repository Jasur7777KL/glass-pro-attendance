# Glass Pro — Xodimlar va Davomat tizimi

Bu repository GitHub Pages uchun tayyor `index.html` saytni o'z ichiga oladi.

## Fayllar

- `index.html` — asosiy web-sayt.
- `README.md` — loyiha haqida ma'lumot.

## GitHub Pages

Repository `main` branch va `/ (root)` papkadan deploy qilinsin:

`Settings → Pages → Deploy from a branch → main → / (root) → Save`

## Supabase ulanishi

`index.html` ichidagi quyidagi ikki qiymatni o'zingizning Supabase ma'lumotlaringiz bilan almashtiring:

```js
const SUPABASE_URL = 'YOUR_SUPABASE_PROJECT_URL';
const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_OR_PUBLISHABLE_KEY';
```

`SUPABASE_URL` — Supabase Project URL.

`SUPABASE_ANON_KEY` — anon/public yoki Publishable key.

**Secret/service_role keyni frontendga qo'ymang.**

## Kerakli database jadvallari

Ushbu sayt quyidagi jadvallardan foydalanadi:

- `departments`
- `employees`
- `attendance`

## Asosiy funksiyalar

- Xodim qo'shish
- Xodimlar ro'yxatini avtomatik shakllantirish
- Bo'limlar
- Bugungi davomat
- `+ Davomat qo'shish`
- Kelish vaqtini avtomatik qayd qilish
- Ketish vaqtini qayd qilish
- 08:30 dan kechikishni hisoblash
- Ishlangan vaqtni hisoblash
- Davomat tarixi
- Hisobotlar
- CSV eksport

## Eslatma

Haqiqiy xodimlarning ma'lumotlarini kiritishdan oldin Supabase RLS va login/rollarini production uchun qat'iy sozlash tavsiya etiladi.
