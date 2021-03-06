---
title: Converting Integer to String in Python
localeTitle: تحويل عدد صحيح الى سلسلة في بايثون
---
## تحويل عدد صحيح الى سلسلة في بايثون

بخلاف العديد من اللغات الأخرى هناك ، فإن Python لا تقوم بتضمين الأعداد الصحيحة typecast (أو العائمة) ضمنيًا إلى سلاسل عندما تكون متسلسلة مع السلاسل. لحسن الحظ ، تمتلك Python `str()` وظيفية `str()` والتي ستحول الوسيطة التي تم تمريرها إلى تنسيق السلسلة.

#### الطريق الخطأ

قد يحاول المبرمجون القادمون من لغات أخرى تنفيذ سلسلة السلاسل التالية التي تنتج خطأ:

 `age = 18 
 
 string = "Hello, I am " + age + " years old" 
` 

[تشغيل الكود على repl.it](https://repl.it/JyYH/0)

الخطأ الذي يظهر هو

 `Traceback (most recent call last): 
  File "python", line 3, in <module> 
 TypeError: must be str, not int 
` 

`TypeError: must be str, not int` يشير إلى أنه يجب أولاً تحويل العدد الصحيح إلى سلسلة ليتم توصيله.

#### الطريق الصحيح

مثال سلسلتي بسيط:

 `age = 18 
 
 print("Hello, I am " + str(age) + " years old") 
 
 # Output 
 # Hello, I am 18 years old 
` 

[تشغيل الكود على repl.it](https://repl.it/Jz8Q/0)

اطبع `1 2 3 4 5 6 7 8 9 10` باستخدام جملة واحدة

 `result = "" 
 
 for i in range(1, 11): 
    result += str(i) + " " 
 
 print(result) 
 
 # Output 
 # 1 2 3 4 5 6 7 8 9 10 
` 

[تشغيل الكود على repl.it](https://repl.it/KBLB/0)

#### شرح عن طريق الخط من التعليمات البرمجية أعلاه

1.  أولا وقبل كل شيء يتم تعيين "نتيجة" متغير لسلسلة فارغة.
2.  للحلقة المستخدمة للتكرار عبر قائمة من الأرقام.
3.  يتم إنشاء قائمة الأرقام هذه باستخدام دالة النطاق.
4.  لذا فإن النطاق (1،11) سيؤدي إلى إنشاء قائمة بالأرقام من 1 إلى 10.
5.  في كل تكرار للتكرار ، سيأخذ هذا المتغير 'i' القيم من 1 إلى 10.
6.  عند التكرار الأول عند المتغير i = 1 ، ثم المتغير \[result = result + str (i) + "(space space)"\] ، يقوم str (i) بتحويل "i" وهي قيمة عددية لقيمة سلسلة.
7.  نظرًا لأن i = 1 ، فإن النتيجة الأولى ستؤدي أخيراً إلى النتيجة = 1.
8.  وتستمر العملية نفسها حتى i = 10 وأخيراً بعد نتيجة التكرار الأخيرة = 1 2 3 4 5 6 7 8 9 10.
9.  لذلك عندما نطبع النتيجة أخيراً بعد الحلقة ، يكون المخرج في الكونسول "1 2 3 4 5 6 7 8 9 10".

#### معلومات اكثر:

[وثائق بيثون الرسمية لل `str()`](https://docs.python.org/3/library/stdtypes.html#str)