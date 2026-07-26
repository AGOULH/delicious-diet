# CLAUDE.md — Delicious Diet

## المشروع
موقع تعريفي من صفحة واحدة لمشروع وجبات صحية. عربي RTL، ثابت (Static) بدون باك-إند.
منشور على: GitHub Pages + Firebase Hosting.

## الملفات
- `index.html` — الصفحة كاملة (HTML + CSS داخلي + المحتوى). كل التعديلات تتم هنا.
- `support.js` / `image-slot.js` — رنتايم Claude Design (وسم `<x-dc>` وخانات الصور). لا تعدّلها ولا تحذفها.
- `_ds/industry-.../styles.css` — نظام التصميم الأساسي (tokens). التعديل هنا يؤثر على كل الصفحة.
- `firebase.json` — إعداد الاستضافة.

## الهوية البصرية (معرّفة في `:root` داخل index.html)
- أخضر `--green: #14412F` · ذهبي `--gold: #B99B54` · كريمي `--cream: #F5F2EA`
- خطوط: العناوين `Cairo` · النص `Tajawal` (Google Fonts)
- `direction: rtl` على `body`
- استخدم متغيرات CSS الموجودة (`var(--color-*)`)، ولا تكتب ألوان hex جديدة.

## أقسام الصفحة
`dd-hero-*` الهيرو · `#menu` الوجبات · `#calc` حاسبة السعرات · `#pricing` الباقات · `#contact` التواصل
واتساب: `https://wa.me/966560250302`

## قواعد العمل
- عدّل `index.html` فقط ما لم يُطلب غير ذلك.
- لا تغيّر اسم `index.html` ولا تحذف مجلد `_ds`.
- حافظ على بنية `<x-dc>` والوسوم الخاصة كما هي.
- النصوص الجديدة بالعربية الفصحى المبسطة.
- بعد أي تعديل: معاينة محلية قبل النشر.

## أوامر
- معاينة: `python3 -m http.server 8000`
- نشر GitHub: `git add -A && git commit -m "..." && git push`
- نشر Firebase: `firebase deploy --only hosting --project delicious-diet-2026`
