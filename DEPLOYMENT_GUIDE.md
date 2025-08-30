# تعليمات نشر موقع الفارس للأعمال
# AlFaris Business Website Deployment Instructions

## 📋 الوضع الحالي | Current Status

تم دمج طلب السحب رقم 2 بنجاح والذي يحتوي على التصميم الحديث الجديد للموقع، لكن هناك حاجة لتفعيل GitHub Pages لنشر الموقع.

Pull Request #2 has been successfully merged with the new modern design, but GitHub Pages needs to be enabled to deploy the website.

## 🔧 خطوات التفعيل المطلوبة | Required Setup Steps

### 1. تفعيل GitHub Pages | Enable GitHub Pages

1. اذهب إلى إعدادات المستودع | Go to repository **Settings**
2. انتقل إلى قسم **Pages** في الشريط الجانبي | Navigate to **Pages** in the sidebar
3. تحت "Source"، اختر **GitHub Actions** | Under "Source", select **GitHub Actions**
4. احفظ الإعدادات | Save settings

### 2. التحقق من التكوين | Verify Configuration

بعد تفعيل GitHub Pages، يمكنك التحقق من التكوين عبر:
After enabling GitHub Pages, you can verify the configuration by:

1. الذهاب إلى تبويب **Actions** في المستودع
2. تشغيل workflow "Test GitHub Pages Configuration" يدوياً
3. مراجعة النتائج للتأكد من نجاح التكوين

## 🚀 النشر التلقائي | Automatic Deployment

بمجرد تفعيل GitHub Pages، سيتم نشر الموقع تلقائياً عند:
Once GitHub Pages is enabled, the website will automatically deploy when:

- ✅ دفع تغييرات إلى فرع `main`
- ✅ دمج طلبات السحب إلى `main`
- ✅ تشغيل workflow النشر يدوياً

## 🌐 رابط الموقع المتوقع | Expected Website URL

```
https://alfaris-business.github.io/alfarissa-website1/
```

## 📄 محتويات الموقع الحالية | Current Website Content

✅ **التصميم الجديد من PR #2**:
- تصميم مظلم حديث واحترافي
- تخطيط RTL للمحتوى العربي
- خدمات تفاعلية مع فلاتر
- أسئلة شائعة قابلة للطي
- تصميم متجاوب للجوال

✅ **الصفحات المتاحة**:
- الصفحة الرئيسية (index.html)
- خدماتنا (our-services-page.html)
- الخدمات القانونية (legal-services-page.html)
- المعاملات الحكومية (government-transactions-page.html)
- الباقات (packages-page.html)
- الأسئلة الشائعة (faq-page.html)
- رؤيتنا (vision-page.html)
- التراخيص (licenses-page.html)
- الزكاة والضرائب (zakat-tax-page.html)
- سياسة الخصوصية (privacy-policy-page.html)
- شروط الخدمة (terms-of-service-page.html)

## 🔍 اختبار محلي | Local Testing

للاختبار المحلي قبل النشر:
For local testing before deployment:

```bash
cd /path/to/repository
python3 -m http.server 8080
# أو | or
npx serve -p 8080
```

ثم زيارة: http://localhost:8080

## ❗ مشاكل شائعة | Common Issues

### 1. فشل النشر | Deployment Failure
```
Error: Get Pages site failed. Please verify that the repository has Pages enabled
```
**الحل | Solution**: تأكد من تفعيل GitHub Pages كما هو موضح أعلاه

### 2. عدم ظهور التحديثات | Updates Not Showing
- انتظر 5-10 دقائق لتحديث الكاش
- تحقق من حالة workflow في تبويب Actions
- امسح كاش المتصفح

## 📞 الدعم | Support

إذا واجهت أي مشاكل:
If you encounter any issues:

1. تحقق من تبويب **Actions** لمراجعة سجلات النشر
2. شغل workflow "Test GitHub Pages Configuration"
3. راجع هذا الدليل مرة أخرى

## 📝 ملاحظات إضافية | Additional Notes

- الموقع يستخدم ملفات HTML ثابتة فقط
- لا يحتاج إلى عمليات بناء معقدة
- يدعم اللغة العربية و RTL بشكل كامل
- محسن للأجهزة المحمولة

---

تم إنشاء هذا الدليل لمساعدتك في نشر التحديثات من طلب السحب رقم 2 بنجاح.
This guide was created to help you successfully deploy the updates from Pull Request #2.