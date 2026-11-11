# خطوات التشغيل

1. firebase.google.com > Add project. من Build فعّل: Authentication (Email/Password)، Firestore Database، Storage (قد يطلب Blaze).
2. Project settings > Your apps > Web (</>) وانسخ الـ config والصقه في public/firebase-config.js
3. Authentication > Users > Add user (إيميلك وكلمة سر قوية). انسخ الـ User UID.
4. استبدل ADMIN_UID في firestore.rules و storage.rules بالـ UID ده.
5. على جهازك: npm i -g firebase-tools ثم firebase login ثم firebase init (اختر Use existing project، واترك الملفات زي ما هي) ثم firebase deploy
6. افتح الرابط /admin.html، ادخل، حط عنوان إنستاباي وارفع أول عمل.
7. Firestore يطلب فهرس بسيط لو ظهر خطأ في الكونسول: اضغط الرابط اللي فيه.
