# Glass Pro — Davomat tizimi V3

Glass Pro uchun yangilangan, korporativ va ko‘zga qulay dashboard dizayni.

## V3 yangiliklari

- Kunduzgi va tungi rejim
- Aniq, katta va o‘qilishi oson Dashboard
- Bugungi davomatni statuslar bilan ajratish
- Kelish / ketish / kechikish / erta ketish / overtime ko‘rsatkichlari
- 60 daqiqadan oshgan vaqtlar avtomatik ravishda `1 soat 5 daqiqa` ko‘rinishida chiqariladi
- Xodimlar ro‘yxati
- Bugungi davomat
- Davomat tarixi
- Bo‘limlar
- Hisobotlar
- CSV eksport
- Supabase real database bilan ishlash

## Ish vaqti

Standart:

- Ish boshlanishi: 08:30
- Ish tugashi: 18:00

Avtomatik hisob:

- Kechikish: 08:30 dan keyingi vaqt
- Erta ketish: 18:00 dan oldingi ketish
- Overtime: 18:00 dan keyingi ish vaqti
- Ishlangan vaqt: kelish va ketish oralig‘i

## GitHub

Repository rootida:

```text
index.html
README.md
```

GitHub Pages:

`Settings → Pages → Deploy from a branch → main → / (root)`

## Supabase

`index.html` ichida:

```js
const SUPABASE_URL = 'YOUR_SUPABASE_PROJECT_URL';
const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_OR_PUBLISHABLE_KEY';
```

qiymatlarini o‘zingizning Supabase Project URL va anon/public yoki Publishable keyingiz bilan almashtiring.

`service_role` yoki secret keyni frontendga qo‘ymang.

## Eslatma

Login/RLS, QR-kod va Telegram xabarnomalari keyingi modul sifatida ulanishi mumkin.
