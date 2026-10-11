مطعمي — مشروع مستقل لـ GitHub Pages وSupabase

قبل أن يصبح كاملًا: قاعدة Supabase يجب أن تكون منفصلة للمطعم أو استخدم الجداول restaurant_* فقط. الملف الرئيسي index.html، والملف restaurant-config.js يحوي إعدادات عامة غير سرية.

1) أنشئ مشروع Supabase مستقلًا للمطعم، ثم شغّل restaurant-supabase-setup.sql في SQL Editor.
2) أنشئ حساب مسؤول من Authentication > Users، انسخ UID، ثم نفّذ آخر أمر موضح في ملف SQL بعد استبدال PASTE_ADMIN_USER_UID_HERE. لا تضع كلمة المرور داخل SQL أو GitHub.
3) في restaurant-config.js ضع Project URL وPublishable key فقط، واسم المطعم ورقم واتساب بصيغة دولية دون + وأجرة التوصيل. هذه القيم العامة تظهر للمتصفح.
4) ارفع كل الملفات والمجلد restaurant-audio مباشرة إلى جذر مستودع GitHub، ولا ترفع المجلد الخارجي كطبقة إضافية. يجب أن يكون index.html في الجذر.
5) Settings > Pages > Deploy from a branch > main > /(root) > Save.

مهم: publishable key (أو anon key القديم) مخصص للواجهة ويمكن أن يكون في GitHub. لا ترفع service_role / secret key أو كلمة مرور قاعدة البيانات أو كلمة مرور المسؤول. هذا الموقع لا يحتاج أي مفتاح سري في المتصفح.

البحث عن الطلب يحتاج رقم الهاتف ورمز تتبع عشوائي طويل؛ لا يُكشف سجل الطلبات باستخدام رقم الهاتف وحده. احفظ الرمز ولا تشاركه علنًا.
