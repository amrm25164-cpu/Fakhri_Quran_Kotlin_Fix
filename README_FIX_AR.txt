Fakhri Quran — Kotlin compatibility fix

سبب الخطأ في آخر سجل: Flutter 3.47.2 يحتاج Kotlin Gradle Plugin 2.2.20 أو أحدث، بينما android/settings.gradle يحدد 2.0.20.

الإصلاح: استبدل android/settings.gradle بالملف المرفق، ثم احفظ وارفع التعديل إلى main وأعد تشغيل GitHub Actions.

تحذيرات AGP 8.11.1 وGradle 8.14.3 ليست سبب الفشل الحالي. سجل البناء يفشل عند فحص إصدار Kotlin.

لم أتمكن من الكتابة إلى مستودع GitHub المتصل لأن التكامل أعاد HTTP 403 (لا توجد صلاحية كتابة)، ولم يتم تأكيد نجاح بناء APK.
