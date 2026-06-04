# -SQL-Case-Study
This case study is designed for students to practice SQL Server data analysis using a real-world dataset from the music streaming industry.

# SQL Server Case Study: Global Music Streaming Trends & Listener Insights

## Overview

Music streaming services collect large amounts of listener data every day. This data helps companies understand customer behavior, improve recommendations, and make better business decisions.
In this project, you will work as a Data Analyst and use Microsoft SQL Server to analyze a real-world music streaming dataset.
Your goal is to answer business questions using SQL queries and provide insights based on the data.

## نظرة عامة

تقوم خدمات بث الموسيقى بجمع كميات كبيرة من بيانات المستمعين يوميًا. تساعد هذه البيانات الشركات على فهم سلوك العملاء، وتحسين التوصيات، واتخاذ قرارات أعمال أفضل.
في هذا المشروع، ستعمل كمحلل بيانات وتستخدم Microsoft SQL Server لتحليل مجموعة بيانات واقعية لبث الموسيقى.
هدفك هو الإجابة على الاسئلة باستخدام استعلامات SQL وتقديم رؤى بناءً على البيانات.


حمل البيانات من هنا
https://github.com/alsinanihajar/-SQL-Case-Study/blob/main/MusicStreaming.csv 
---

## Dataset Information

**Dataset Name:** Global Music Streaming Trends & Listener Insights

**Table Name:** `MusicStreaming`

### Columns

- User_ID
- Age
- Country
- Streaming_Platform
- Top_Genre
- Minutes_Streamed_Per_Day
- Number_of_Songs_Liked
- Most_Played_Artist
- Subscription_Type
- Listening_Time
- Discover_Weekly_Engagement
- Repeat_Song_Rate
## وصف الأعمدة

### User_ID
معرّف فريد لكل مستخدم في البيانات.

---

### Age
عمر المستخدم.

---

### Country
الدولة التي يقيم فيها المستخدم.

---

### Streaming_Platform
منصة بث الموسيقى التي يستخدمها المستخدم مثل Spotify أو Apple Music أو YouTube.

---

### Top_Genre
أكثر نوع موسيقي يستمع إليه المستخدم.

---

### Minutes_Streamed_Per_Day
متوسط عدد دقائق الاستماع يوميًا لكل مستخدم.

---

### Number_of_Songs_Liked
إجمالي عدد الأغاني التي أعجب بها المستخدم.

---

### Most_Played_Artist
الفنان الأكثر استماعًا لدى المستخدم.

---

### Subscription_Type
نوع الاشتراك (مجاني أو مدفوع).

---

### Listening_Time
وقت الاستماع المفضل للمستخدم خلال اليوم (صباح / مساء / ليل).

---

### Discover_Weekly_Engagement
نسبة التفاعل مع قوائم Discover Weekly.

---

### Repeat_Song_Rate
نسبة تكرار الاستماع لنفس الأغاني.
---



## استيراد ملف CSV إلى Microsoft SQL Server

اتبع الخطوات التالية لاستيراد مجموعة البيانات:

1. افتح **SQL Server Management Studio (SSMS)**.
2. أنشئ قاعدة بيانات جديدة.
3. انقر بزر الماوس الأيمن على قاعدة البيانات.
4. اختر **Tasks (المهام)**.
5. اختر **Import Flat File (استيراد ملف نصي)**.
6. تصفح واختر ملف CSV.
7. انقر على **Next (التالي)**.
8. راجع تفاصيل الجدول.
9. انقر على **Finish (إنهاء)**.
10. تأكد من إنشاء الجدول بنجاح.
---

# Business Questions

## Question 1


What is the average number of minutes streamed per day for each streaming platform?

ما متوسط عدد دقائق الاستماع اليومية لكل منصة بث؟

**Hint:** Use `AVG()` with `GROUP BY`.

**تلميح:** استخدم `AVG()` مع `GROUP BY`.

---

## Question 2


Which countries have the highest average streaming time per day?

ما الدول التي تمتلك أعلى متوسط لوقت الاستماع اليومي؟

**Hint:** Calculate the average listening time for each country and sort the results.

**تلميح:** احسب متوسط وقت الاستماع لكل دولة ثم قم بترتيب النتائج.

---

## Question 3

What is the average number of liked songs for each music genre?
 
ما متوسط عدد الأغاني المفضلة لكل نوع موسيقي؟

**Hint:** Use `AVG()` with `GROUP BY`.

**تلميح:** استخدم `AVG()` مع `GROUP BY`.

---

## Question 4


Compare Premium and Free users in terms of average listening time.


قارن بين مستخدمي Premium و Free من حيث متوسط وقت الاستماع.

**Hint:** Group the data by subscription type.

**تلميح:** قم بتجميع البيانات حسب نوع الاشتراك.

---

## Question 5

Which music genre has the highest average listening time?

أي نوع موسيقي يمتلك أعلى متوسط لوقت الاستماع؟

**Hint:** Calculate the average streaming minutes for each genre and sort descending.

**تلميح:** احسب متوسط دقائق الاستماع لكل نوع موسيقي ثم قم بترتيب النتائج تنازليًا.

---

## Question 6

What is the average Discover Weekly Engagement percentage for each streaming platform?

ما متوسط نسبة التفاعل مع Discover Weekly لكل منصة بث؟

**Hint:** Use `AVG()` with `GROUP BY`.

**تلميح:** استخدم `AVG()` مع `GROUP BY`.

---

## Question 7

What is the average Repeat Song Rate for each streaming platform?

ما متوسط معدل إعادة تشغيل الأغاني لكل منصة بث؟

**Hint:** Use `AVG()` with `GROUP BY`.

**تلميح:** استخدم `AVG()` مع `GROUP BY`.

---

## Question 8

Find all users who stream more than 500 minutes per day.

اعرض جميع المستخدمين الذين يستمعون لأكثر من 500 دقيقة يوميًا.

**Hint:** Use a `WHERE` condition.

**تلميح:** استخدم شرط `WHERE`.

---

## Question 9

Find all Premium users from Germany.

اعرض جميع مستخدمي Premium من ألمانيا.

**Hint:** Use multiple conditions in the `WHERE` clause.

**تلميح:** استخدم أكثر من شرط داخل `WHERE`.

---

## Question 10

Show the average listening time for each age.

اعرض متوسط وقت الاستماع لكل عمر.

**Hint:** Use `AVG()` and `GROUP BY Age`.

**تلميح:** استخدم `AVG()` و `GROUP BY` حسب العمر.

---



## يجب على الطلاب تسليم:
- ملف SQL يحتوي على جميع حلول الاستعلامات.
- تقرير مختصر (1–2 صفحة) يلخص النتائج والرؤى حسب مفهومك . 

---



