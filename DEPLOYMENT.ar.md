# Romantic Gift Website - Deployment Guide

## إرشادات النشر على Netlify

### المتطلبات قبل البدء:
- ✅ حساب GitHub
- ✅ حساب Netlify (يمكنك إنشاء واحد مجاني)
- ✅ الملفات مرفوعة على GitHub

### خطوات النشر:

#### 1️⃣ ادفع المشروع إلى GitHub

```bash
git add .
git commit -m "Setup for Netlify deployment"
git push origin main
```

#### 2️⃣ انتقل إلى Netlify وأنشئ موقع جديد

1. اذهب إلى [app.netlify.com](https://app.netlify.com)
2. انقر على **"Add new site"** → **"Import an existing project"**
3. اختر **GitHub**
4. ستطلب منك الموافقة على الوصول

#### 3️⃣ حدد المستودع الخاص بك

- ابحث عن المستودع `Test`
- انقر عليه

#### 4️⃣ إعدادات البناء

Netlify سيقرأ تلقائياً من `netlify.toml`:

- **Build command**: `npm install && npm run build`
- **Publish directory**: `client/dist`

انقر على **"Deploy site"**

#### 5️⃣ انتظر اكتمال البناء

- Netlify سينشئ موقع بعنوان عشوائي
- بمجرد اكتمال البناء، سيكون الموقع مباشراً! 🎉

### خطوات إضافية:

#### ✨ ربط نطاق مخصص (اختياري)

1. اذهب إلى **Site settings** → **Domain management**
2. انقر على **"Add custom domain"**
3. اتبع التعليمات

#### 🔐 متغيرات البيئة (إذا لزم الأمر)

1. اذهب إلى **Site settings** → **Build & deploy** → **Environment**
2. انقر على **"Edit variables"**
3. أضف المتغيرات المطلوبة

### 📋 ملاحظات مهمة:

- كل `push` إلى GitHub سيؤدي لبناء تلقائي على Netlify
- يمكنك رؤية سجل البناء في تبويب **"Deploys"**
- الملفات الثابتة يتم تخزينها مؤقتاً تلقائياً لسرعة أفضل

### 🆘 استكشاف الأخطاء:

إذا فشل البناء:
1. اذهب إلى **Deploys** → أحدث نشر
2. انقر على **"Deploy log"**
3. ابحث عن رسالة الخطأ
4. عدّل الملفات وادفعها مرة أخرى

---

**والآن موقعك جاهز! 🚀**
