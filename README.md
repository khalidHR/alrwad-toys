# ALRWAD TOYS — Static Website

موقع متجر ألعاب الرواد — جاهز للرفع على GitHub Pages مجاناً.

## 🚀 كيف ترفعه على GitHub Pages

### الخطوة 1 — أنشئ Repo
1. اذهب لـ [github.com](https://github.com)
2. اضغط **New repository**
3. سمّه: `alrwad-toys` أو `YOUR_USERNAME.github.io`
4. اجعله **Public**
5. اضغط **Create repository**

### الخطوة 2 — ارفع الملفات
**طريقة سهلة (بدون كود):**
1. افتح الـ repo الجديد
2. اضغط **uploading an existing file**
3. اسحب ملف `index.html` وأي ملفات أخرى
4. اضغط **Commit changes**

**طريقة Git:**
```bash
git init
git add .
git commit -m "launch ALRWAD TOYS website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/alrwad-toys.git
git push -u origin main
```

### الخطوة 3 — فعّل GitHub Pages
1. في الـ repo → **Settings**
2. من القائمة الجانبية → **Pages**
3. Under **Source** → اختر **Deploy from a branch**
4. Branch → **main** / **root**
5. اضغط **Save**

### الخطوة 4 — انتظر دقيقتين
موقعك سيكون على:
```
https://YOUR_USERNAME.github.io/alrwad-toys/
```

## 🌐 ربط دومين مخصص (اختياري)

لو اشتريت دومين مثل `alrwadtoys.com`:

**في Namecheap — أضف DNS Records:**
```
Type: A    | Host: @   | Value: 185.199.108.153
Type: A    | Host: @   | Value: 185.199.109.153
Type: A    | Host: @   | Value: 185.199.110.153
Type: A    | Host: @   | Value: 185.199.111.153
Type: CNAME| Host: www | Value: YOUR_USERNAME.github.io
```

**في GitHub Pages Settings:**
- Custom domain → اكتب `alrwadtoys.com`
- ✅ Enforce HTTPS

انتظر 24 ساعة للـ DNS propagation.

## ✏️ كيف تعدّل المنتجات

افتح `index.html` وابحث عن `const PRODUCTS = [` — عدّل بياناتك هناك.

كل منتج يحتوي على:
```javascript
{
  id: 1,
  emoji: "🚲",           // أيقونة المنتج
  name: "اسم المنتج",
  cat: "القسم",
  short: "وصف مختصر",
  desc: "وصف تفصيلي",
  price: "299",           // السعر بالريال
  bg: "#EFF5F8",          // لون خلفية البطاقة
  featured: true          // هل هو مميز؟
}
```

## 💰 التكلفة

| البند | التكلفة |
|-------|---------|
| GitHub Pages | **مجاني** ✅ |
| دومين .com (سنوياً) | ~$9 = 34 ر.س |
| SSL | **مجاني** ✅ |
| **المجموع** | **34 ر.س/سنة فقط** |
