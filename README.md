# نور – قرآن وأحاديث وأذكار

## التشغيل
```
npm install
npm run seed     # يحمّل المصحف كاملاً مرة واحدة (يحتاج إنترنت)
npm start        # ثم افتح http://localhost:3000
```

## الهيكل
- `server.js` سيرفر Express والـ API
- `seed.js` تحميل المصحف إلى `data/quran.json`
- `data/` الأحاديث والأذكار (عدّل الملفات لإضافة المزيد)
- `public/index.html` الواجهة (HTML/CSS/JS)

## الـ API
- `GET /api/surah/:n` آيات سورة (1–114)
- `GET /api/search?q=كلمة` بحث في الآيات (بدون تشكيل)
- `GET /api/hadith` الأحاديث
- `GET /api/adhkar` الأذكار حسب الفئة
