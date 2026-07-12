# Romantic Gift Website

مشروع موقع هدايا رومانسية مع تصميم حديث وديناميكي.

## المميزات

- 🎨 تصميم عصري وجميل
- ⚡ أداء سريع
- 📱 متوافق مع جميع الأجهزة (Responsive)
- 🎯 تجربة المستخدم ممتازة

## التثبيت والتشغيل

### المتطلبات
- Node.js 16.x أو أعلى
- npm أو yarn أو pnpm

### التثبيت المحلي

```bash
# تثبيت الحزم
npm install

# تشغيل النسخة التطويرية
npm run dev

# بناء الإصدار الإنتاجي
npm run build

# معاينة الإصدار الإنتاجي
npm run preview
```

## النشر على Netlify

### الخطوات:

1. **ادفع المشروع إلى GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **انتقل إلى Netlify**
   - اذهب إلى [netlify.com](https://netlify.com)
   - سجل دخول باستخدام حسابك على GitHub
   - انقر على "New site from Git"
   - اختر المستودع
   - اترك الإعدادات الافتراضية (ستقرأ `netlify.toml` تلقائياً)
   - انقر على "Deploy site"

### متغيرات البيئة (إذا لزم الأمر)

إذا احتاج المشروع إلى متغيرات بيئة:

1. اذهب إلى Site Settings → Build & deploy → Environment
2. أضف المتغيرات المطلوبة

## هيكل المشروع

```
romantic_gift_website/
├── client/          # تطبيق React/Vue
│   ├── src/
│   ├── public/
│   └── dist/       # سيتم إنشاؤه عند البناء
├── server/         # خادم Node.js (إن وجد)
├── netlify.toml    # إعدادات Netlify
└── package.json
```

## التطوير

لمعرفة المزيد عن المشروع، انظر الملفات الموجودة في المجلدات الرئيسية.
