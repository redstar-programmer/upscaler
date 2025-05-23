# Redstar Upscaler
Tooling FlowFrans ، FlowFrames-NOW Tooling Ffmpeg ، relectrgan ، تدعم Flowframes-NOW ** UI **!

## 🌐 إعدادات اللغة / اللغة
[한국어](https://github.com/redstar-programmer/upscaler/blob/main/README.md) | [English](https://github.com/redstar-programmer/upscaler/blob/main/README/README.en.md) | [日本語](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ja.md) | [中文](https://github.com/redstar-programmer/upscaler/blob/main/README/README.zh.md) |
[Français](https://github.com/redstar-programmer/upscaler/blob/main/README/README.fr.md) | [Deutsch](https://github.com/redstar-programmer/upscaler/blob/main/README/README.de.md) | [Español](https://github.com/redstar-programmer/upscaler/blob/main/README/README.es.md) | [Português](https://github.com/redstar-programmer/upscaler/blob/main/README/README.pt.md) |
[Русский](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ru.md) | [Italiano](https://github.com/redstar-programmer/upscaler/blob/main/README/README.it.md) | [Tiếng Việt](https://github.com/redstar-programmer/upscaler/blob/main/README/README.vi.md) | [Bahasa Indonesia](https://github.com/redstar-programmer/upscaler/blob/main/README/README.id.md) |
[ภาษาไทย](https://github.com/redstar-programmer/upscaler/blob/main/README/README.th.md) | [العربية](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align = "center">
  <strong> ffmpeg ، realesrgan ، flowFrames -spide tooling </strong> <br>
  <em> أحدث قاعدة واجهة المستخدم الرسومية ، إعداد الإعداد المسبق ، دعم معالجة الملفات المتعددة </em>
</p>

---

تنزيل: [الإصدار]

## ✨ رعاية Redstar 'Upscaler

هل تريد أن يعجبك هذا المشروع أو تطوير دعم؟  
ساعد ميزة أفضل وتحديث مستقر مع رعاية صغيرة!  

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub Sponsors** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)

> 💡 تكلفة الخادم ، ووقت التطوير ، وكوب من القهوة قوة كبيرة. شكرًا لك!

## جدول المحتويات

- [👋 مقدمة] (#Introduction)  
-[💾 التثبيت والإعداد] (#التثبيت والتقديم)  
- [🔧 الوظيفة الرئيسية] (#الوظيفة الرئيسية)  
-[🚀 كيفية استخدام (بداية سريعة)] (#استخدم us-Quick-Start)  
-[⚙ التفاصيل الوصف] (#التفاصيل الوظيفية الوظيفية)  
- [🙏 شكرا] (#شكرا كتاب)  
- [📜 التاريخ] (#History)

## 👋 مقدمة
** RedStar Upscaler ** هي أداة واجهة المستخدم الرسومية القائمة على Python تقوم تلقائيًا بتثبيت الفيديو إلى الدقة العالية باستخدام "FFMPEG` و" real-esrgan "و" FlowFrames ".

-استخراج إطار الفيديو → الارتفاع → مزيج من الفيديو مرة واحدة
-دعم لنماذج Realesrgan المختلفة
-3- من خلال FlowFrames
-استخراج وتجهيز ترميز الترميز
-العمل على الموقع الأصلي أو المسار المحدد

> ⚠ تم تطويره واختباره في بيئة Windows.

أدناه متصل بـ YouTube من خلال النقر على شاشة استخدام بسيطة. <br>
[![Watch the demo](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co "Watch on YouTube")

## 💾 التثبيت والإعداد

1.
   - [FFMPEG] (https://www.ffmpe.org/download.html)
   -[real-eSrgan] (https://github.com/xinntao/real-esrgan
   - [FlowFrames] (https://github.com/n00mkrad/flowframes) *(حدد) *
2. قم بتشغيل upscaler.exe بعد readstar
3. في حالة FlowFrames ، قد تكون النماذج المحملة وفقًا لبيئة المستخدم مختلفة ، لذا تأكد من تشغيل FlowFrames ثم <br> interpolation AI و RedStar Upscaler Resources/FlowFrames_Models.ini يجب أن تتطابق معها. <br> يُشار إلى أن النماذج التي تم تحميلها يتم التعليق عليها من خلال العرض # ، وتأكد من التحقق مما إذا كان ترتيب نموذج نافذة الإعداد لـ RedStar Upscaler مطابقة مع ترتيب طراز <br> FlowFrames.

## 🔧 الوظيفة الرئيسية

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
-فيديو اختيار متعددة وعمل متسلسل
-DD ​​الفيديو السحب/إسقاط
-ما إذا كنت تريد تشغيل البرامج الرئيسية وتحديد التحديد المباشر
-وضع حفظ الخراء
-الدعم الملتوي (15 لغة)
<br> <br>
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
-مسبقًا مسبقًا والتطبيق التلقائي
-اكتشاف أوتوماتيكي لإعدادات ترميز الصوت وإعدادات setRate
-الكشف الآلي واختيار نماذج Realesrgan
-ffmpeg ، real-esrgan ، تفاصيل FlowFrames
-تغيير إعدادات الخيار وفقًا لإصدار FlowFrames <br>
<br> <br>
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
-upscale تأكيد أمر التنفيذ (يمكن نسخه وتنفيذه بشكل منفصل عن CMD)
<br> <br>
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
-استقل التقدم الكلي للعمل الراقي
-upscale تأكيد تسجيل (يتم إنشاء ملف السجل كتاريخ في مجلد السجل في المجلد الحقيقي)
-ترتيب آلي للنتيجة بعد الانتهاء من العمل (بادئة [Redstar])
-عملية عملية بعد الانتهاء <br>
<br> <br>
## 🚀 كيفية الاستخدام (بداية سريعة)

1. أضف ملف فيديو (MP4 ، MKV ، AVI ، MOV ، FLV ، WMV ، MPG ، WebM ، 3GP ، OGV)
2. تحقق من موقع العمل أو "استخدم مسار الملف الأصلي"
3. انقر فوق الزر "الإعدادات" في الفيديو المضافة
4. FFMPEG ، Realesrgan ، تفاصيل FlowFrames
5. انقر فوق تطبيق فقط على الملف / تحديد الملف بأكمله
4. انقر على زر تأكيد المهمة
7. انقر فوق الزر "ابدأ" بعد التحقق من الأمر لتشغيله

> ✨ يتم إنشاء نتائج العمل في المجلد المحدد من خلال صورتين متضخمين وملفين فيديو محرفان.
> ✨ يتم حفظ الملف المكتمل كاسم ملف مع بادئة [RedStar].
---

## ⚙ التفاصيل الوصف

| البند | الوصف |
| ------ | ------ |
| ** إعداد مسار المهمة ** | توفير المسار الافتراضي أو "استخدم خيار مسار الملف الأصلي" |
| ** دعم تنسيق الفيديو ** | MP4 ، MKV ، AVI ، MOV ، FLV ، WMV ، MPG ، WebM ، 3GP ، OGV ، إلخ.
| ** نموذج راقي ** | Realesr-Animevideov3 ، Realesr-General ، 4xplus ، إلخ.
| ** معالجة الصوت ** | دعم تشفير مختلف التنسيق مثل "AAC" و "MP3" و "Flac" |
| ** FlowFrames مرتبطة ** | تعيين الاستيفاء (FPS × 2 ، × 4 ، × 8) |
| ** وضع توفير القرص ** | صورة وسيطة الحذف التلقائي المقدمة |

## 🙏 عيد الشكر

- realesrgan by [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes by [n00mkrad](https://github.com/n00mkrad/flowframes)
-إذا كنت ترغب في المشاركة في هذا المشروع أو اقتراح وظيفة ، فيرجى ترك رأي حول [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).

# 📜 التاريخ

v 1.1.0
 >. تكوين القائمة (فتح الملف ، إغلاق ، إعداد السجل ، إعداد اللغة)
 > 2. إضافة إعدادات لغة متعددة (اللغة المتاحة: الكورية ، الإنجليزية ، 日本語 ، 中文 ، français ، deutsch ، español ، português ،
 3. الرسالة وبعض الكود يتغير وفقًا لإضافة إعدادات اللغة
 > 4. تغيير بعض تكوين واجهة المستخدم
 >. FFMPEG ، real-esrgan ، FlowFrames كل معلومات الإصدار (الشاشة الرئيسية)
 > 6. استجابة FlowFrames 1.41.0 (الإصدار الحالي 1.41.0 له مشكلة أمر CMD ، لذلك يمكن استخدام 1.40.0 و 1.36.0 فقط)
 > حل المشكلة في أن عنصر نماذج الذكاء الاصطناعى يتم عرضه كحرف صغيرة
 8. خيارات FFMPEG (بكسل ، برنامج ترميز الفيديو)
 > 9. تعزيز شيكات CUDA لأجهزة الكمبيوتر المستخدم -يمكن استخدامها وتحقق من نوع وحدة معالجة الرسومات (الشاشة الرئيسية)

v 1.0.0
 >.
 >. تغيير واجهة المستخدم
 > 3. زيادة نطاق الفيديو/الصوت القابل للمعالجة
 > 4. إضافة وضع حفظ القرص
 > التوزيع بما في ذلك البرامج الرئيسية

v 0.1.92
 >. FlowFrames مشكلة فشل الاستيفاء عن طريق التكرار في مربع التحرير والسرد من طراز AI عند تغيير المسار
 > 2. أضف حالة اختيار مربع التحرير والسرد لأعمال الاستيفاء

V 0.1.91
 >.
 > 2. ضبط ملف التوزيع

v 0.1.9
 >. تطبيق تغيير نموذج FlowFrames
 >. FlowFrames 1.36.0 نموذج جديد ، تنفيذ النموذج 1.40.0
 3. لا مزيد من عطل الأوامر يحدث بعد الآن
 > 4. يمكنك إضافة ملفات مع السحب/إسقاط
 > حل المشكلة التي لا يتم تطبيقها

v 0.1.8
 >.
 2. إذا تم تثبيت FlowFrames في المسار الافتراضي (على سبيل المثال C: \ Users \ Administrator
 3. عند إضافة ملفات متعددة 
 > 4. بعد إضافة ملفات متعددة ،

v 0.1.7
 >. تغيير حجم البرنامج
 2. حل مشكلة الأخطاء عند العمل مع ملف بدون صوت
 > 3. قم بتغيير تكوين واجهة المستخدم بالكامل (إعادة تكوينه لتناسب تغيير الحجم)

V 0.1.6
 >.
 >. حل المشكلة التي لا يُنظر إلى معلومات الإصدار كإصدار جديد في عنوان البرنامج.
 > حل المشكلة التي يتم فيها تخزين ملفات config.ini في مسارات أخرى
 > 4. عند تغيير الصرف الصحي الراقي ، يتم تغيير مربع التحرير والسرد النموذجية الراقية معًا
 > 5. إضافة وظيفة التحقق من التحديث
 > 6. بعض التعديلات المنطقية
 > 7. القرار و FPS
 > 8. تعديل المستخدم (السابق) (يجب إدخاله في شكل 1024 × 768)

V 0.1.5
 >.
 2.
 3. أضف بعض الفيديو من مربع التحرير والسرد "حساب FPS" لمنع حساب الحالة على أنها FPS خاطئ عند حساب FPS لبعض مقاطع الفيديو.
        -> يمكن تحديد R_FRAME_RATE / AVG_FRAME_RATE ، ويتم حساب الافتراضي بواسطة R_FRAME_RATE
 > 4. عند تحديد ملف فيديو ، تقدم معلومات الفيديو 
 > 5. بعد ركل الملف ، قم بتغيير لفتح آخر مجلد محدد افتراضيًا عند تحديد الملف مرة أخرى.

V 0.1.4
 >. تغيير طريقة قراءة ملف config.ini
 > 2. قم بتغيير معلومات الفيديو من Python AV إلى FFMPEG
 > 3. أضف وظيفة نهاية Windows عند العمل على العمل
 > 4. في قائمة العمل ، يتم عرض اسم الملف بأكمله كملالية أدوات
 >. في قائمة العمل ، كل دقة ملف (قبل) / دقة (بعد) / FPS (قبل) / FPS (POST) تدوين
 > 6. إزالة مربع الإدخال FPS (إزالة بسبب كل تدوين ملف)
 > 7. إخراج FPS إزالة حجم التنبؤ (إزالة بسبب كل ملف لكل ملف)
 > 8. يتم كتابة حالة التقدم كـ اثنين

V 0.1.3
 > 1. إصلاح خطأ حساب FP FPS مع بعض معلومات FPS عند استيراد الملفات

v 0.1.2
 >. تغيير تكوين واجهة المستخدم   
 > 2. تغيير المنطق الداخلي  
 > حل المشكلة التي لا يتم تنفيذها عند اختيار نموذجين أدناه بين طرز Realesrgan  
 > 4. تغيير كيفية استخدام نموذج Realesrgan   
 > -> انسخ ملف نموذج جديد (*.param) إلى مجلد النماذج في مجلد تثبيت Realesrgan.  
 >.  
 > 6. رمز ترحيل ملف config.ini  
 > 7. صورة التحلل FFMPEG AAC-> FLAC  
 > 8. تعديلات الأخطاء الأخرى

V 0.1.1
 >. الكتابة الأولية ، FFMEPG ، Realesrgan ، و FlowFrames.