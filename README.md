# Basketball 4Mat Virtual Environment

ملف المشروع: `index.html` — بيئة افتراضية تعليمية مصمّمة باستخدام نموذج 4Mat لمهارات كرة السلة (المحاورة - التمريرة الصدرية - التصويب من الثبات).

## ماذا يوجد داخل الحزمة
- `index.html` — الصفحة الرئيسية والصفحات الفرعية للمهارات، تحتوي على محاكاة بسيطة، رفع فيديو، قوائم ملاحظة، وسجل xAPI-like.
- `README.md` — أنت تقرأه الآن.

## معاينة محلية
1. فك الضغط عن الملف أو انسخ `index.html` إلى مجلد محلي.
2. افتح `index.html` في متصفح حديث (Chrome/Edge/Firefox).
> ملاحظة: رفع الفيديوهات يعرض معاينة محلية باستخدام `URL.createObjectURL`، والبيانات التحليلية تحفظ في `localStorage` للمستخدم فقط.

## رفع على GitHub Pages (الطريقة السهلة عبر واجهة الويب)
1. ادخل إلى https://github.com وسجّل الدخول.
2. اضغط **New repository** وأنشئ مستودعًا جديدًا (مثلاً `basketball-4mat`). اجعله `Public`.
3. داخل المستودع: **Add file → Upload files** ثم اسحب `index.html` و `README.md` ثم اضغط **Commit changes**.
4. ادخل إلى **Settings → Pages** (أو Settings → Code and automation → Pages حسب الواجهة). في قسم **Source** اختر الفرع `main` والمجلد `/ (root)` ثم احفظ.
5. انتظر دقيقة أو دقيقتين، ستحصل على رابط مشابه: `https://your-username.github.io/basketball-4mat/`

## رفع عبر Git (الأوامر)
1. افتح الطرفية في المجلد الذي يحتوي `index.html` و `README.md`.
2. نفّذ الأوامر التالية (غيّر `USERNAME` و`REPO`):
```bash
git init
git add index.html README.md
git commit -m "Initial commit - Basketball 4Mat"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```
3. ثم فعّل GitHub Pages من إعدادات المستودع كما في الخطوة أعلاه.

## ملاحظات تقنية
- جميع العمليات تتم من جهة العميل (Client-side). إن أردت تخزين فيديوهات المستخدمين فعليًا على الخادم (server) أو عرض سجلات المستخدمين مركزيًا فسنحتاج إلى Backend + تخزين (مثال: Firebase Storage أو خادم خاص).
- إذا أردت فصل الملفات (css/, js/, assets/) أو إضافة مكتبات خارجية يمكنني تنظيم المشروع في مجلدات وإعداد `index.html` لمرجعتها.
- السجل المولّد يكون بصيغة JSON (xAPI-like) ويمكن تحميله من لوحة التحليلات داخل التطبيق.

## هل تريدني أن أفعل ذلك لك؟
- أستطيع تجهيز المستودع كاملًا كهيكل ملفات (مع `.gitignore`، LICENSE، assets) ثم أمدك بتعليمات رفع أو أقدّم ملف ZIP جاهز للرفع.
- أو أستطيع إرشادك خطوة بخطوة أثناء رفعه على GitHub (أوجهك خلال كل خطوة).

بالتوفيق — دكتور!
