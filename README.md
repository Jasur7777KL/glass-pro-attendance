# Glass Pro — Davomat tizimi V2

Yangilangan versiya: tezkor kelish/ketish, tungi/kunduzgi rejim, kechikish, erta ketish va overtime avtomatik hisob-kitobi.

## Fayllar
- index.html
- README.md

## GitHub Pages
`Settings → Pages → Deploy from a branch → main → / (root)`

## Supabase
Jadvallar: `departments`, `employees`, `attendance`.
`index.html` ichidagi `SUPABASE_URL` va `SUPABASE_ANON_KEY`ni o‘zingiznikiga almashtiring. Secret/service_role keyni frontendga qo‘ymang.

## Xodim qo‘shish
Foydalanuvchidan ID yoki ishga qabul qilingan sana so‘ralmaydi. Xodim ID tizim tomonidan avtomatik yaratiladi.

## Davomat
- Kelishni tasdiqlash
- Ketishni tasdiqlash
- `+ Davomat qo‘shish` orqali vaqtni qo‘lda kiritish/tahrirlash
- 08:30 dan keyingi kelish — kechikish
- 18:00 dan oldingi ketish — erta ketish
- 18:00 dan keyingi ketish — overtime
- Ishlangan vaqt avtomatik hisoblanadi

## Keyingi bosqichlar
Login va rollar, QR-kod, Telegram xabarnoma va audit log interfeysda rejalashtirilgan.
