---
layout: post_ar
title: "تعلم البرمجة بلغة بايثون - الدرس الأول: مقدمة"
date: 2020-03-01
categories: [دورة-تعلم-البرمجة-بلغة-بايثون] 
tags: [بايثون, برمجة, لغات-برمجة, تعلم-البرمجة, البرمجة-للمبتدئين, تعلم-البرمجة-بالعربي]
postlang: arabic 
permalink: "/ar/:year/learn-programming-with-python-1-1-arabic"
sharing-img: "/assets/images/2020/pyc-1-6.png"

---



![دورة تعلم البرمجة بلغة بايثون. القسم الأول، الدرس الأول](/assets/images/2020/pyc-1-6.png)

في هذه الدورة **ستتعلم البرمجة بلغة بايثون (Python) من الصفر**. هذه الدورة لا تفترض أن لديك خبرة سابقة في البرمجة ، فيمكنك دخول هذه الدورة حتى لو كنت لا تعرف شيئاً عن البرمجة من قبل.

الدورة ستكون مقسمة إلى عدة أقسام ، وكل قسم يحتوي على عدد من الدروس. 

سيتم طرح دروس هذه الدورة عن طريق تدوينات مثل هذه وعن طريق فيديوهات على موقع يوتيوب (YouTube). فيمكنك اختيار الأفضل بالنسبة لك.

ما يميز هذه الدورة أنها مبنية على مصادر من **أفضل المصادر** العالمية الموجودة لتعلم بايثون خاصة دورات [Python for Everybody](https://www.coursera.org/specializations/python) المقدمة من جامعة ميشيغان الأمريكية. وخلال هذه الدورة سنكتب برامج مفيدة وعملية يمكنك استخدامها في حياتك اليومية.

في هذا الدرس سنناقش الهدف من تعلم البرمجة ، وسنعرف ما هو البرنامج ، وسنرى مثالاً على برنامج بلغة بايثون ، ثم سنتعرف على الأسباب التي تجعلنا نختار بايثون كلغة برمجة لتعلمها ، ثم سنأخذ لمحة سريعة عن مكونات الحاسب وكيفية عمله ، وفي النهاية سأعرفكم عن نفسي ومؤهلاتي لإعداد هذه الدورة.

## لماذا نتعلم البرمجة؟

قبل أن تبدأ بتعلم البرمجة لا بد أن تسأل نفسك هذا السؤال: لماذا أريد تعلم البرمجة؟. ولتجيب عن هذا السؤال عليك أن تعلم أننا نعيش اليوم في عالم مليء بالتكنولوجيا والأجهرة الإلكترونية: حاسبات ، هواتف محمولة ، أجهزة ذكية ، إلخ. البرمجة تحولك من مجرد مستهلك للتكنولوجيا إلى صانع لها.

![من فوائد البرمجة](/assets/images/2020/pyc-1-1.png)

الحاسب (أو الكمبيوتر) هو جهاز صنع لهدف واحد وهو أن ينفذ ما تأمره به. كيف يمكن أن تعطي الأوامر (أو التعليمات) للحاسب؟ عن طريق برامج مثل برامج بايثون. كيف تصنع هذه البرامج؟ عن طريق تعلم البرمجة. عن طريق البرمجة يمكنك صنع برامج مفيدة لك تستخدمها في حياتك أو برامج يمكن للآخرين أيضاً الاستفادة منها.

## ما هو البرنامج؟

البرنامج ببساطة هو سلسلة من التعليمات للكمبيوتر مكتوبة بإحدى لغات البرمجة.

لتقريب الفكرة دعنا نعطي مثالاً من حياتنا عن برنامج للإنسان وهي وصفات الطعام. فمثلاً ستجد تعليمات مكتوبة لك في طريقة التحضير: قطع البطاطا ، ضع المكونات في وعاء ، اخلط المزيج جيداً ، ضعه في الفرن حتى يصبح لونه ذهبياً ، وهكذا. برنامج الكمبيوتر يشبه ذلك ولكنه بدل أن يكون مكتوباً بلغة بشرية كالعربية سيكون مكتوباً بلغة برمجية مثل بايثون أو جافا ، وبدلاً من أن ينفذه الإنسان سيقوم الكمبيوتر بتنفيذه.

## مثال عن برنامج بلغة بايثون

كيف يبدو البرنامج المكتوب بلغة بايثون؟ في الصورة أدناه ترى برنامجاً بسيطاً بلغة بايثون. 

![برنامج بايثون لإيجاد أكثر الكلمات تكراراً](/assets/images/2020/pyc-1-2.png)

هذا البرنامج يقوم بإيجاد أكثر كلمة تكررت في ملف نصي ويطبعها للمستخدم. تخيل مثلاً أن أعطيك كتاباً من 300 صفحة وأطلب منك أن تجد أكثر كلمة تكرراً في الكتاب وعدد مرات تكرارها. يمكنك بالطبع أداء هذه المهمة لكنها ستستهلك منك وقتاً طويلاً جداً وجهداً وتركيزاً كبيرين. لكن باستخدام هذا البرنامج الصغير يمكننا إيجاد المطلوب خلال أقل من ثانية (في الحقيقة يمكن لهذا البرنامج أن يبحث في أكثر من ألف صفحة خلال أقل من ربع ثانية!).

## لماذا بايثون؟

بايثون هي لغة برمجة تم اختراعها قبل حوالي 30 سنة (عام 1991) من قبل مبرمج هولندي اسمه جايدو ڤان روسم. يشارك اليوم المئات من أكفأ المبرمجين حول العالم في تطوير بايثون وتحسينها.

بايثون هي لغة برمجة **متعددة الأغراض** أي أنها تستخدم في الكثير من المجالات مثل برمجة تطبيقات الإنترنت وبرامج الحاسب والبرامج العلمية وعلم البيانات (data science) وتحليل البيانات (data analysis) وتصوير البيانات (data visualization) والذكاء الاصطناعي والشبكات وغيرها.

### بايثون سهلة التعلم للمبتدئين

من مميزات لغة بايثون أنها **لغة برمجة سهلة التعلم** وفي نفس الوقت **قوية جداً** وتستخدم في أكبر الشركات في العالم. ولهذا السبب تجد أن العديد من جامعات العالم صارت تدرس لغة بايثون لطلابها في سنواتهم الأولى. بالنسبة لي فقد تعلمت العديد من لغات البرمجة مثل C و C++ و Java و غيرها ووجدت فعلاً أن بايثون هي الأسهل بلا منازع. 

### بايثون أشهر لغة برمجة

[يتم استخدام بايثون اليوم من قبل أقوى الشركات](https://en.wikipedia.org/wiki/Programming_languages_used_in_most_popular_websites) على مستوى العالم مثل Google و Facebooks وغيرها. الرسم البياني في الأسفل يوضح مدى شهرة بايثون في Google مقارنة بغيرها من لغات البرمجة القوية مثل جافا وسي شارب وبي إتش بي في آخر خمس سنين. لاحظ كيف أن بايثون (ممثلة باللون الأزرق) ازدادت شهرة مع الأيام حتى أصبحت اليوم تتفوق على جميع هذه اللغات.

<script type="text/javascript" src="https://ssl.gstatic.com/trends_nrtr/2051_RC11/embed_loader.js"></script> <script type="text/javascript"> trends.embed.renderExploreWidget("TIMESERIES", {"comparisonItem":[{"keyword":"/m/05z1_","geo":"US","time":"2015-02-28 2020-02-28"},{"keyword":"/m/07sbkfb","geo":"US","time":"2015-02-28 2020-02-28"},{"keyword":"/m/07657k","geo":"US","time":"2015-02-28 2020-02-28"},{"keyword":"/m/060kv","geo":"US","time":"2015-02-28 2020-02-28"}],"category":0,"property":""}, {"exploreQuery":"date=today%205-y&geo=US&q=%2Fm%2F05z1_,%2Fm%2F07sbkfb,%2Fm%2F07657k,%2Fm%2F060kv","guestPath":"https://trends.google.com:443/trends/embed/"}); </script>

أيضاً يمكنك النظر إلى الرسم أدناه لترى مدى شهرة بايثون على الموقع البرمجي الشهير [Stack Overflow](https://stackoverflow.com/) مقارنة بالعديد من لغات البرمجة الأخرى. شاهد كيف أن بايثون (الخط الأحمر العريض في الرسم) أصبحت اليوم هي اللغة الأكثر تفاعلاً على الموقع.

![مدى شهرة لغات البرمجة على موقع Stack Overflow](/assets/images/2020/pyc-1-3.png)

وبسبب كثرة استخدام بايثون حول العالم فغالباً لن يخطر سؤال في بالك إلا وستجد له جواباً ولن تواجهك مشكلة إلا وستجد أحداً حلها من قبل.

### حزم برمجية لكل شيء

من مميزات لغة بايثون أيضاً أن هناك الكثير من الحزم البرمجية الجاهزة للاستخدام والتي تجعل القيام بالأمور العظيمة سهلاً في متناول اليد. الحزم البرمجية هي برامج تكون ضخمة أحياناً كتبها مبرمجون وجعلوها متاحة كي يستخدمها غيرهم بسهولة. هناك حزم لتحليل البيانات وحزم لإجراء حسابات رياضية معقدة وحزم أخرى لإنشاء رسوم بيانية وحزم للاتصال بقواعد البيانات المختلفة وحزم لتحميل البيانات من الإنترنت (web crawling) وحزم لتحميل الفيديوهات من يوتيوب وحزم لإنشاء برامج ذكاء اصطناعي وتعلم الآلة (machine learning) ووو... القائمة لا تنتهي. لاحقاً سترى الفائدة العظيمة لهذه الحزم!

## لمحة عن عتاد الحاسب (الهاردوير)

بما أن البرامج التي ستكتبها سيتم تنفيذها من قبل الحاسب، فمن المفيد أن نأخذ لمحة سريعة ومبسطة عن كيفية عمل الحاسب من الداخل. 

يمكن تمثيل الأجزاء الرئيسية في الحاسب كما في الصورة التالية:

![مخطط توضيحي لمكونات الحاسب](/assets/images/2020/pyc-1-4.png)

أجهزة الإدخال والإخراج: أجهزة الإدخال هي الأجهزة التي نستخدمها للإدخال إلى الحاسوب مثل الفأرة ولوحة المفاتيح، وأجهزة الإخراج هي الأجهزة التي يستخدمها الحاسوب للإخراج مثل الشاشة وسماعات الصوت. 

وحدة المعالجة المركزية أو المعالج أو CPU هي أهم جزء في الحاسب، وهي دارة كهربائية شديدة التعقيد تحتوي على الملايين والملايين من [الترانزستورات]([https://ar.wikipedia.org/wiki/%D8%AA%D8%B1%D8%A7%D9%86%D8%B2%D8%B3%D8%AA%D9%88%D8%B1](https://ar.wikipedia.org/wiki/ترانزستور))، ويمكن للمعالجات الحديثة تنفيذ حوالي 3 مليارات عملية في الثانية الواحدة، فهي سريعة جداً ودائماً تطلب التعليمة (الخطوة) التالية لتقوم بتنفيذها. ومن أين تأخذ التعليمات؟ من الذاكرة الرئيسية (RAM).

![صور معالج Intel i7 من الأعلى والأسفل](/assets/images/2020/pyc-1-5.png)

نرى أيضاً الذاكرة الثانوية وهي الذاكرة التي تحتفظ بالبيانات حتى بعد إطفاء الحاسب مثل القرص الصلب. عندما تكتب برنامجاً بلغة بايثون يتم تخزينه على الذاكرة الثانوية ثم يتم ترجمته إلى لغة الآلة (أصفار وواحدات) ونقله إلى الذاكرة الرئيسية عند تشغيله، وعندما يسأل المعالج: "ما التعليمة التالية؟" يتم إعطاء أول تعليمة من برنامجك للمعالج وعندما ينتهي من تنفيذها يتم إعطاؤه التعليمة التي بعدها وهكذا.

لماذا لا يكفي وجود ذاكرة رئيسية فقط في الحاسب؟ لماذا نحتاج إلى ذاكرة ثانوية؟ لأنه عندما نقوم بإطفاء الحاسب فإن الذاكرة الرئيسية تفقد كل محتوياتها بينما الذاكرة الثانوية تحتفظ بمحتوياتها حتى بعد إطفاء الحاسب.

## من أنا؟

بما أني سأكون الشخص الذي يعد هذه الدورة فلا بد أن أخبركم قليلاً عن نفسي ومؤهلاتي كي تزداد ثقتكم بالمحتوى المقدَّم في هذه الدورة.

اسمي عمار اليوسفي. نلت درجة الماجستير مع مرتبة الشرف في علم البيانات (Data Science) من الجامعة الأولى في ماليزيا جامعة مالايا، وقبلها حصلت على درجة البكالوريوس في هندسة الحاسوب (Computer Engineering) من جامعة الأميرة سمية للتكنولوجيا في الأردن بترتيب الأول على الدفعة. عملت في شركة عالمية في كوالالامبور في مجال علم وتحليل البيانات. ونفذت عدة مشاريع لاقت قبولاً جيداً في مجالات تحليل البيانات وتصوير البيانات وتعلم الآلة وبايثون والعديد من حزمها البرمجية و SQL وغير ذلك. للاطلاع على المزيد من التفاصيل ولزيارة صفحات المشاريع التي قمت بتنفيذها يمكنك زيارة [صفحة سيرتي الذاتية](https://ammar-alyousfi.com/s-resume/).

## فيديو الدرس

<iframe width="560" height="315" src="https://www.youtube.com/embed/w1JEjTvhfW8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

