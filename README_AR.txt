مشروع الموقع المسترجع — Luvera / NOIR BEAUTY
============================================

محتويات الحزمة:
- public/index.html: آخر نسخة محفوظة من واجهة NOIR BEAUTY (أسود وذهبي، عربي RTL).
- original_versions/noir_beauty_store_original.html: نسخة أصلية مطابقة للواجهة الحالية.
- original_versions/beauty_store_with_10_products_and_images.html: النسخة الأقدم التي تحتوي صور المنتجات العشرة المضمّنة داخل الملف.
- firebase.json: إعداد Firebase Hosting لنشر مجلد public.

مهم جداً قبل النشر:
1) اسم مشروع Firebase الظاهر في المحادثة هو Luvera، لكن Project ID الفعلي غير متوفر في الملفات المسترجعة؛ لذلك لم أضع Project ID تخميناً.
2) آخر نسخة محفوظة من NOIR BEAUTY تستخدم localStorage لحفظ المنتجات على نفس الجهاز والمتصفح. إضافة/تعديل/حذف المنتجات تعمل محلياً، لكنها لا تتزامن بين أجهزة الزبائن.
3) النسخة الأقدم محفوظة كما هي وبداخلها صور المنتجات العشرة الأصلية. لم أدمجها في التصميم الأحدث حتى لا أغيّر المنتجات أو الواجهة دون تأكيد.
4) لم يتم العثور على firebaseConfig أو إعدادات Firestore/Storage/Auth في الملفات السابقة. لذلك هذه الحزمة جاهزة لنشر ملفات الموقع الثابتة على Firebase Hosting، لكنها لا تدّعي أن مزامنة المنتجات السحابية مفعّلة.
5) رقم واتساب المحفوظ في النسخة الحالية: 07770167886.

للنشر باستخدام Firebase CLI (من مجلد المشروع بعد اختيار مشروع Firebase الصحيح):
  firebase login
  firebase use --add
  firebase deploy --only hosting

إذا كنت تستخدم مشروع Firebase باسم Luvera، اختره في خطوة firebase use --add وتأكد من Project ID قبل النشر.
