---
layout: post_ar
title: "تعلم البرمجة بلغة بايثون - الدرس الرابع: مدخل إلى برامج بايثون (2)"
date: 2020-03-15
categories: [دورة-تعلم-البرمجة-بلغة-بايثون] 
tags: [بايثون, برمجة, لغات-برمجة, تعلم-البرمجة, البرمجة-للمبتدئين, تعلم-البرمجة-بالعربي]
postlang: arabic 
permalink: "/ar/:year/learn-programming-with-python-1-4-arabic"
sharing-img: "/assets/images/2020/pyc-4-1.png"
---



![تعلم البرمجة بلغة بايثون - الدرس الرابع: مدخل إلى برامج بايثون (2)](/assets/images/2020/pyc-4-1.png)

في هذا الدرس سنتعرف على الطرق التي يمكن أن يسير بها برنامج بايثون وسنرى أمثلة على كل طريقة.

## كيفية سير برنامج بايثون

هناك عدة أنماط لسير برنامج بايثون:

### النمط التسلسلي

في هذا النمط يكون البرنامج عبارة عن سلسلة من الخطوات التي يجب تنفيذها بالترتيب.

![مثال عن نمط سير البرنامج التسلسلي](/assets/images/2020/pyc-4-2.png)

### النمط الشرطي

في هذا النمط يقوم البرنامج بتنفيذ بعض الخطوات فقط في حال تحقق شرط ما.

![مثال عن نمط سير البرنامج الشرطي](/assets/images/2020/pyc-4-3.png)

الكلمة التي تمكننا من وضع الشروط هي `if` وهي إحدى الكلمات المحجوزة في بايثون. `if` دائماً ما تكون متبوعة بشرط. مثلاً في المثال في الصورة أعلاه الشرط الأول هو `x < 10`. فإذا تحقق الشرط وكانت قيمة `x` أقل من 10 يقوم البرنامج بتنفيذ الجملة الشرطية:

```python
print('Smaller')
```

وإذا لم يتحقق الشرط فإن البرنامج يتجاوز الجملة الشرطية ولا يقوم بتنفيذها. في المثال: قيمة `x` عند التحقق من الشرط هي 5 وهي أقل من 10 لذلك سينفذ البرنامج الجملة الشرطية.

بالنسبة للشرط الثاني: `x < 20` فإن هذا الشرط غير متحقق في مثالنا بما أن قيمة `x` هي 5 ولذلك فالبرنامج لن ينفذ الجملة الشرطية المرتبطة بهذا الشرط وهي:

```python
print('Bigger')
```

لاحظ كيف أن الجملتان الشرطيتان منزاحتان قليلاً إلى اليمين. هذا الانزياح يدل على أن الجملة الشرطية تابعة لجملة `if` التي فوقها.

بالنسبة للأمر الأخير:

```python
print('Finish')
```

فسيتم تنفيذه دائماً مهما كانت قيمة `x` لأنه غير متعلق بأي شرط.

### النمط التكراري

في هذا النمط يقوم البرنامج بتكرير تنفيذ مجموعة من الخطوات.

![مثال عن نمط سير البرنامج التكراري](/assets/images/2020/pyc-4-4.png)

في المثال أعلاه: الكلمة التي مكنتنا من إنشاء حلقة تكرارية (loop) هي `while` وهي أيضاً من الكلمات المحجوزة في بايثون. ودائماً ما تكون `while` متبوعة بشرط. وطالما بقي هذا الشرط متحققاً سيستمر البرنامج في تكرار تنفيذ الأوامر داخل الحلقة.

ففي المثال أعلاه: سيتم تخزين 5 في المتغير `n` ثم نأتي إلى جملة `while` وهنا يتم طرح سؤال: هل `n` أكبر من 0؟ إذا كان الجواب "نعم، صحيح" فسيتم تنفيذ الأوامر داخل الحلقة (وهي الأوامر المنزاحة إلى اليمين قليلاً) ثم سيتم طرح السؤال مرة أخرى وسيتكرر تنفيذ ما بداخل الحلقة حتى يصبح جواب السؤال "لا، خطأ"، عندها سيتجاوز البرنامج الأوامر داخل الحلقة وينتقل لتنفيذ الأوامر التي ما بعد الحلقة.

إذا تتبعنا كيفية سير عمل المثال في الصورة أعلاه: سنرى أنه عند طرح سؤال `while` فإن الإجابة ستكون "صحيح" لأن `n` والتي قيمتها 5 أكبر من 0، ولذلك سيتم تنفيذ التعليمتين داخل الحلقة وهي طباعة قيمة `n` ثم طرح 1 من `n` لتصبح 4. بعدها سيتم طرح سؤال `while` مرة أخرى: هل `n` أكبر من 0؟ وأيضاً بما أن `n` قيمتها 4 فسيكون الجواب "صحيح" وسيتم تنفيذ تعليمات الحلقة وتصبح قيمة `n` الجديدة 3. وسيتم تكرار ذلك حتى تصبح `n` مساوية لـ 0. عندها عندما يتم طرح سؤال الحلقة سيكون الجواب "خطأ" وسيخرج البرنامج من الحلقة وينفذ التعليمة التي بعدها وهي طباعة "Finished".

لاحظ أن التعليمات التابعة لحلقة `while` منزاحة إلى اليمين قليلاً ولاحظ أيضاً النقطتان الرأسيتان بعد جملة `while`. هذه كلها من قواعد كتابة بايثون التي عليك مراعاتها وإلا فإن بايثون ستخبرك بوجود خطأ في برنامجك.

لاحظ أيضاً أنه تم كتابة البرنامج في المثال أعلاه بحيث يتم تنفيذ التعليمات داخل الحلقة 5 مرات. 

### النمط الوظيفي

في هذا النمط يقوم البرنامج باستخدام الدوالّ (أو التوابع). الدالّة هي مجموعة من الأوامر تنفذ مهمة معينة ويتم استدعاؤها عند الحاجة إليها. سنعرف المزيد عن هذا النمط لاحقاً إن شاء الله.

الآن إذا نظرنا مرة أخرى إلى البرنامج الذي عرضناه سابقاً والذي يقوم بإيجاد أكثر كلمة تكراراً في ملف نصي وعدد مرات تكرارها:

![برنامج بايثون لإيجاد أكثر كلمة تكرراً في نص](/assets/images/2020/pyc-4-5.png)

سنرى أنه يحتوي على كود تسلسلي مثل أول ثلاث تعليمات ويحتوي على كود تكراري مثل التعليمات التي تبدأ في سطر رقم 5 وتنتهي في سطر رقم 8. هذه السطور تحتوي على حلقتي `for` و `for` هي كلمة محجوزة تمكننا من إنشاء حلقات تكرارية شبيهة بـ `while`. ونرى أيضاً أن هذا البرنامج يحتوي على كود شرطي مثل التعليمات التي تبدأ في سطر 13. سنعود لاحقاً لهذا البرنامج لنرى كيفية كتابته خطوة بخطوة بعد أن نتعلم الأساسيات اللازمة.

في الدروس القادمة سنتعلم بالتفصيل عن المتغيرات والجمل الشرطية والحلقات وغيرها. في هذا الدرس قمنا فقط بإلقاء نظرة إجمالية لتمكننا من ربط الأشياء ببعضها لاحقاً. فلا تقلق إن كانت بعض المفاهيم مشوشة لديك أو كانت هناك أجزاء غير واضحة بعد.

## فيديو الدرس

<iframe width="560" height="315" src="https://www.youtube.com/embed/EybWCCT9Rx0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

ملاحظة: ربما تقول في نفسك أن البرامج التي تراها حتى الآن ليس لها فائدة وهذا صحيح لأننا ما زلنا في البداية نتعلم الأساسيات والقواعد البدائية لكني أؤكد لك أنك عندما تتعلم بايثون بشكل جيد ستستطيع فعل العديد والعديد من الأمور الهامة والمفيدة التي تختصر عليك وقتاً وجهداً أو تجلب لك ربحاً مالياً أو تمكنك من تقديم فائدة للآخرين.

