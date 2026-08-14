# Glass Pro — Xodimlar va Davomat tizimi

Glass Pro korxonasining xodimlar va davomat boshqaruv web-sayti.

## Papka tarkibi

```text
glass-pro-final/
├── index.html
└── README.md
```

## 1. GitHub Pages

Repository rootida aynan quyidagilar tursin:

```text
index.html
README.md
```

GitHub:

`Settings → Pages → Source: Deploy from a branch`

Sozlamalar:

- Branch: `main`
- Folder: `/ (root)`

## 2. Supabase

Sayt quyidagi jadvallardan foydalanadi:

- `departments`
- `employees`
- `attendance`

Ular oldindan yaratilgan bo‘lishi kerak.

## 3. index.html ichida Supabase sozlamasi

Faylning yuqori qismidagi:

```js
const SUPABASE_URL = 'YOUR_SUPABASE_PROJECT_URL';
const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_OR_PUBLISHABLE_KEY';
```

qiymatlarini o‘zingiznikiga almashtiring.

Misol:

```js
const SUPABASE_URL = 'https://YOUR_PROJECT_ID.supabase.co';
const SUPABASE_ANON_KEY = 'YOUR_ANON_OR_PUBLISHABLE_KEY';
```

`service_role` yoki `secret` keyni frontendga qo‘ymang.

## 4. Ish vaqti

Standart:

- Ish boshlanishi: 08:30
- Ish tugashi: 18:00

Sozlamalar bo‘limidan o‘zgartirish mumkin.

## 5. Davomat logikasi

- 08:30 gacha yoki 08:30 da → Vaqtida
- 08:30 dan keyin → Kechikdi
- Kelish vaqti yo‘q → Kelmagan
- Ketish vaqti kiritilganda → Ishni tugatdi

Kechikish daqiqalari va ishlangan vaqt avtomatik hisoblanadi.

## 6. Saytdagi asosiy funksiyalar

### Bosh sahifa
Bugungi:
- jami xodimlar
- kelganlar
- kelmaganlar
- kechikkanlar
- kelish va ketish vaqtlari

### Xodimlar
- xodim qo‘shish
- xodimlar ro‘yxati
- bo‘lim bo‘yicha filter
- qidiruv
- xodimning bugungi holati
- davomatni ochish

### Bugungi davomat
- `+ Davomat qo‘shish`
- ism-familiya avtomatik chiqadi
- kelgan vaqt
- ketgan vaqt
- tahrirlash
- kelishni qayd etish
- ketishni qayd etish
- kechikish
- ishlangan vaqt
- status

### Davomat tarixi
Sana tanlanadi va aynan shu kunning davomatlari ko‘rsatiladi.

### Bo‘limlar
Bo‘limlar va ulardagi faol xodimlar soni.

### Hisobotlar
Bugungi umumiy ko‘rsatkichlar va CSV eksport.

## 7. Tavsiya

Haqiqiy xodim maʼlumotlarini kiritishdan oldin Supabase RLS va login/rollarini production uchun qatʼiy sozlash kerak.

