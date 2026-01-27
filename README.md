# 🤖 بوت الذكاء الاصطناعي | تسجيل الدخول الآمن

واجهة تسجيل دخول احترافية وعصرية باستخدام حساب Google، مصممة خصيصًا للغة العربية مع دعم كامل لاتجاه النص من اليمين لليسار (RTL).

![واجهة تسجيل الدخول](https://placehold.co/800x500/1a1a2e/6366f1?text=واجهة+تسجيل+الدخول+الاحترافية)

## ✨ الميزات

- **تصميم عصري**: واجهة زجاجية (Glassmorphism) مع تدرجات ألوان فاخرة (أرجواني-وردي-أزرق)
- **دعم اللغة العربية**: خط Tajawal، اتجاه نص RTL، واجهة بالكامل بالعربية
- **أمان عالي**: يسمح فقط بحسابات Gmail (`@gmail.com`)
- **تجربة مستخدم ممتازة**: تأثيرات حركية، شاشة تحميل أنيقة، توجيه تلقائي
- **متجاوب بالكامل**: يعمل على الجوال، الحاسوب، والتابلت
- **ملف واحد فقط**: لا يعتمد على أي ملفات خارجية — كل شيء في `index.html`

## 🚀 العرض الحي

يمكنك تجربة الموقع مباشرةً عبر:

👉 [https://your-username.github.io/ai-bot-login](https://your-username.github.io/ai-bot-login)

> ⚠️ **ملاحظة**: استبدل `your-username` باسم مستخدم GitHub الخاص بك.

## 🛠️ كيفية الاستخدام

### 1. التثبيت المحلي
1. نزّل الملف [`index.html`](./index.html)
2. افتحه مباشرةً في متصفحك (لا حاجة لخادم)

### 2. النشر على GitHub Pages
1. أنشئ مستودعًا جديدًا على GitHub
2. ارفع ملف `index.html` إلى المستودع
3. شغّل GitHub Pages من:
   - Settings → Pages → Source: `main` branch, folder `/`
4. أضف نطاقك إلى Google Cloud Console (انظر أدناه)

### 3. إعداد Google OAuth (ضروري للعمل)
لتفعيل زر "تسجيل الدخول بـ Google"، يجب:

1. الذهاب إلى [Google Cloud Console](https://console.cloud.google.com/)
2. إنشاء مشروع أو اختيار موجود
3. تفعيل **Google Identity Platform** أو **OAuth Consent Screen**
4. في **Credentials**:
   - أضف **Authorized JavaScript origins**:
     ```
     https://your-username.github.io
     https://your-username.github.io/ai-bot-login
     http://localhost (للتطوير المحلي)
     ```
5. استبدل `GOOGLE_CLIENT_ID` في الكود بـ Client ID الخاص بك

> 🔐 **Client ID الحالي في الكود هو للتوضيح فقط** — يجب استبداله بـ ID خاص بك في الإنتاج.

## 📁 هيكل المشروع
