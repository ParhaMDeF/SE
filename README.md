# Software Architecture


#### استاد درس

دکتر حسن بشیری

#### گرد آورنده

پرهام خوش روش




## مقدمه
معماری فرآیند و محصول برنامه ریزی برای طراحی و ساخت ساختمان ها یا سازه های دیگر است. یک طراحی خوب می تواند باعث بقای یک سازه شود و سال ها مورد تحسین قرار گیرد یا حتی نتواند پایدار بماند. این وظیفه معمار است که طریق علم مطمئن شود که تمام قطعات یک ساختمان به خوبی کنار هم قرار می گیرند و یک سازه مستحکم و ایمن را ایجاد می کنند.
مانند معماران به عنوان یک مهندس نرم افزار، ما نیز باید از علم استفاده کنیم تا راه حل ها را به روشی درست و مطمئن بخش ارائه دهیم، اما به جای آجر، از کد استفاده خواهیم کرد.

 
![image](https://user-images.githubusercontent.com/61993604/171823550-94e0f696-7049-46fe-b9d9-b39dd027bcb1.png)


## 	معماری نرم افزار چیست؟
برای فهمیدن معماری نرم افزار ، یا معماری ساده ، اجازه بدهید تا در مورد یکی از نیازهای زندگی صحبت کنیم .
اجازه بدهید فرض کنیم در اینجا درخواست یک ساختمان یک طبقه را داریم که در آینده ما میتوانیم طبقات بیشتری را به این ساختمان اضافه کنیم ، و همچنین ما این توانایی را داریم که در هر زمانی که خواستیم طراحی اتاق ها یا طبقات را با استفاده از پارتیشن براحتی تغییر دهیم ، بنابراین این ها نیاز های معمولی یک ساختمان هستند ، و همچنین زمین لرزه روی آن نباید تاثیری داشته باشد. این بدین معناست که ساختمان آمادگی رویارویی با هرگونه شرایطی رو به راحتی داشته باشد. اینها صفات و کارکرد ساختمان هستند و ما فقط با داشتن طراحی می توانیم به این دستاورد برسیم . طراحی پایه و پی ساختمان مهمترین بخش از طراحی هر ساختمان است و همچنین به عنوان کاربر یا مشتری ، ما همیشه زمان ، بودجه ، نگهداشت پذیری ، اعتبار و غیره را بصورت عقلانی در نظر میگیریم. اگرچه ما نیاز هایی در زندگی واقعی داریم از فروشنده میپرسیم : ساختن این ساختمان چگونه است ؟ هزینه نگهداری آن در اینده چگونه است ؟
معماری نرم افزار در واقع انتخاب ساختاری اساسی است که تغییر آن پس از اجرا پر هزینه است.
ایده اساسی و بنیادین این است که هر چیزی که درست و اساسی طراحی شده باشد ، یک محصول خوب تولید خواهد کرد که تمام معیارهای بالا را خواهد داشت. با استفاده از معماری می‌توانیم یک دید کلی و یا اصطلاحاً abstraction را برای مدیریت پیچیدگی‌های سیستم ایجاد کنیم و یک ارتباط بسیار مفید و یک هماهنگی منحصر به ‌فرد را بین اجزای تشکیل دهنده یک سیستم ایجاد نماییم.

<p align="center">
  <img src="https://user-images.githubusercontent.com/61993604/171863832-1ec5e684-fe5a-4d0f-8b5f-09b4b43955a1.png"/>
</p>

معماری، یک راه حل ساختارمند را برای رسیدن به تمامی نیازمندی های فنی و عملکردی یک سیستم در دست قرار می دهد. علاوه بر این؛ با استفاده از معماری می توان ویژگی های کیفی معمول از قبیل؛ عملکرد و یا performance و امنیت و یا security را تقویت و یا بهبود کرد.
علاوه بر این؛ معماری، شامل تصمیمات مهمی در رابطه با سازمان مربوط به توسعه نرم افزار است. هر کدام از این تصمیمات می‌توانند تاثیر چشمگیری بر روی کیفیت، قابلیت نگهداری، قابلیت عملکرد و موفقیت سراسری پروژه داشته باشند. برخی از این تصمیمات شامل موارد زیر هستند:

•	انتخاب عناصر ساختاری و interface هایی که با استفاده از آنها سیستم به عملکرد خود جامه عمل می پوشاند.

•	رفتار تعریف شده بین همکاری‌های شکل گرفته، مابین این عناصر.

•	ترکیب این ساختارها و رفتارهای آنها به درون یک زیر سیستم بزرگتر.

•	تصمیمات معماری منطبق بر اهداف کسب و کار.

•	سبک های معماری و تصمیمات کاربردی در برابر آنها.
<p align="center">
  <img width = 600 src="https://user-images.githubusercontent.com/61993604/171864347-86c79d4c-76f8-4587-882b-a7ce871c89cb.png"/>
</p>

## 	اهداف معماری نرم افزار:
<p align="center">
  <img width = 600 src="https://user-images.githubusercontent.com/61993604/171864636-a4cb759c-769d-4232-834b-5e99ba8fe58c.png"/>
</p>

هدف اصلی این معماری شناسایی نیازهایی است که بر ساختار برنامه تأثیر می گذارد.

یک معماری خوب خطرات تجاری مرتبط با ایجاد راه حل فنی را کاهش می دهد و پلی را بین نیازهای فنی و تجاری ایجاد می کند.

برخی از اهداف معماری نرم افزار عبارتند از:

•	ساختن طرح کلی یا اسکلت بندی برای پیاده سازی یک محصول.

•	مخفی کردن جزئیات و پیچیدگی های درونی و نشان دادن جزئیات ساختاری و اساسی.

•	کمک به توسعه دهندگان برای استفاده از مولفه ها یا کد.

•	حذف کدهای زائد با ساختن عناصر و کتابخانه های چندبار مصرف.

•	حل کردن مسائلی که در حین طراحی هر برنامه ای رخ میدهد.

•	راحتی در سازگار کردن برنامه با هر گونه تغییرات در اینده.

•	انجام تمامی موارد کاری و یا use-case ها و سناریوها.

•	پاسخ دهی به نیازمندی های مطرح شده توسط ذینفعان.

•	در نظر گرفتن نیازمندی های کیفی و عملکردی.

•	افزایش سطح کیفی و عملکردی یک سیستم.

•	افزایش اعتماد خارجی به سازمان و یا سیستم.


در اینجا اهداف متنوعی وجود دارد که با طراحی مناسب و خوب قابل دسترسی هستند.

### جدایی از نگرانی - Separation of Concern:

این بدان معناست که کلید های منطقی بهتر است در لایه های جداگانه یا درون فایلی از طراحی واسط کاربری باشند.

### مسئولیت تنها - Single Responsibility:

همانطور که از نامش پیداست ، هر معیار یا عنصر بهتر است فقط مسئول یک کار باشند.

### حداقل دانش - Least Knowledge:

بدان معنیست که یک عنصر نباید از جزئیات عناصر دیگر خبر داشته باشند.

### تکرار نکردن - Do not Repeat:

این بدان معناست که توابع مختلف در مولفه های مختلف تکرار شوند. یک تابع فقط باید در یک مولفه استفاده شود.

### به حداقل رساندن طراحی - Minimize the Design: 

تنها طراحی است که برای برنامه اجباریست و سعی در استفاده مجدد از چیزی که وجود دارد نکنید. تا جایی ای که ممکن است از مولفه های reuseable استفاده کنید . این کار در تسریع زمان رفع باگ های برنامه بسیار موثر است. 
ایده اصلی این طراحی ها پنهان کردن پیچیدگی ماژول ها بوسیله تقسیم Solution بر اساس مولفه ها و استفاده از مولفه های reuseable یا توابعی است که ممکن است در طول برنامه بارها از آنها استفاده شوند . برای مثال ، قسمت های مختلف را در مولفه های مختلف نظیر Data Access, Business Logic, Exception Handling Mechanism, Email یا  SMS handling, File Operation, Services ، توزیع کنید. 

 
### <p align = right>: OOPS</p> 
 
استفاده کامل از ظرفیت های الگوی شی گرا که به حل مشکلات شناخته شده ی توسعه نرم افزار کمک میکند و با یک روش یکپارچه به شما امکان گسترش و نگهداری از برنامه را میدهد. 

### لایه های برنامه - Application Layer:

درباره ی اینکه قصد توسعه کدام مولفه را در Solution دارید و در مورد طبقه بندی کردن آنها در لایه ها دقیق باشید ، که این امر به ما در پیاده سازی تئوری مشخصی که به دنبال آن هستیم کمک می کند. 

-  استفاده از domain model و object برای ارسال و دریافت داده از لایه ها.
- بر اساس عملکرد مولفه ها ، آنها را در لایه های مختلف نظیر Data Access, Business Logic, Helper یا Utility یا Common, Domain, Service تقسیم میکنیم.


### کیفیت سیستم- System Quality: 

کیفیت مولفه ها یکی از جنبه های کلیدی برای توسعه نرم افزار برای مواجه با کارآمد بودن نیازمندی های کاربر است. برای انجام unit test برای هر توسعه به منظور اطمینان از درست کار کردن کد ها میتوانید از یک سیستم تست کردن دقیق استفاده کنید.

### زمان ایجاد معماری - When to Create Architecture:

معماری ها در فاز طراحی یا حتی زودتر از آن در توسعه یک سیستم ایجاد می‌شوند. اگر شما از روش پردازش توسعه آبشاری (waterfall development process) استفاده می کنید، ایجاد معماری یکی از ابتدایی ترین کارهایی است که شما در این روش انجام می دهید. شما مشکل را تعریف می کنید و سپس آن را به وسیله یک معماری حل می کنید. اگر به جای آن، شما از یک پردازش توسعه برنامه مکرر (iterative software development process) نظیر Unified Process یا agile استفاده می کنید، این معماری باعث ایجاد تکرار های زود هنگام در انجام کارها می شود. زمانی که تکرار توسعه معماری کامل شد، مراحل دیگر نظیر طراحی و کدنویسی میتوانند آغاز شوند.


<p align="center">
  <img width = 350 src="https://user-images.githubusercontent.com/61993604/171866684-a83fabeb-201b-4c08-86b5-64259c80a133.png"/>
</p>

 ## محدودیت های معماری نرم افزار
 
 معماری نرم افزار هنوز یک رشته در حال ظهور در مهندسی نرم افزار است که محدودیت های زیر را دارد:
 
•	کمبود ابزار و روش های استاندارد برای نمایش معماری.

•	کمبود روش تجزیه و تحلیل پیش بینی اینکه آیا معماری منجر به پیاده سازی مطابق با الزامات خواهد شد یا خیر.

•	عدم آگاهی از اهمیت طراحی معماری در توسعه نرم افزار.

•	عدم درک نقش معمار نرم افزار توسط ذینفعان و ارتباط ضعیف بین آن ها.

•	عدم درک فرآیند طراحی، تجربه طراحی و ارزیابی طرح.


<p align="center">
  <img width = 600 src="https://user-images.githubusercontent.com/61993604/171869157-043c0f51-fb77-42d8-8ad2-9321520692d3.png"/>
</p>

## نقش معمار نرم افزار چیست؟
<p align="center">
  <img width = 600 src="https://user-images.githubusercontent.com/61993604/171869440-656af315-a481-4dd9-b56d-32722a1fcdd2.png"/>
</p>

یک معمار نرم افزار راه حلی را ارائه می دهد که تیم فنی می تواند آن را در کل برنامه ایجاد و طراحی استفاده کند.

خروجی طرحی که از معمار نرم افزار دریافت می شود شامل موارد زیر می شود:

•	مجموعه ای واضح، کامل، سازگار و قابل دستیابی از اهداف عملکردی.

•	شرح عملکرد سیستم، حداقل با دو لایه تجزیه مفهومی برای سیستم.

•	طرحی به شکل سیستم، با حداقل دو لایه تجزیه.

•	ایده ای از زمان کلی، ویژگی های اپراتور و برنامه های اجرا و بهره برداری.

•	یک سند یا فرآیند که تضمین می کند تجزیه عملکردی دنبال شده، و نوع رابط کنترل می شود.

برای رسیدن به نتایج بالا یک معمار نرم افزار باید در زمینه های زیر تخصص داشته باشد:

### تخصص طراحی

•	متخصص در طراحی نرم افزار، از جمله روش ها و رویکردهای متنوع مانند طراحی شی گرا، طراحی رویداد محور و غیره.

•	رهبری تیم توسعه و هماهنگی تلاش های توسعه برای یکپارچگی طراحی.

•	باید قادر به بررسی پیشنهادات طراحی و سبک و سنگین کردن آن ها جهت استفاده باشد.

### تخصص فناوری

•	متخصص در فن آوری های موجود که در اجرای سیستم کمک می کند.

•	هماهنگ سازی انتخاب زبان برنامه نویسی، چارچوب، سیستم عامل ها، پایگاه داده و غیره.

### تخصص روش شناسی

•	متخصص روش های توسعه نرم افزار که ممکن است در طول SDLC (چرخه عمر توسعه نرم افزار) اتخاذ شود.

•	رویکردها و روش های مناسبی را برای پیشرفت انتخاب کند که به کل تیم کمک کند.

### نقش پنهان معمار نرم افزار

•	تسهیل کار فنی در میان اعضای تیم و تقویت رابطه اعتماد در تیم.

•	متخصص اطلاعات که دانش مشترک دارد و تجربه زیادی دارد.

•	از اعضای تیم در برابر نیروهای خارجی که باعث حواس پرتی آن ها می شود و ارزش کمتری برای پروژه دارند محافظت می کند.

## ویژگی های کیفی در معماری نرم افزار

کیفیت معیاری برای تعالی یا عاری بودن از کمبود و نقص است. ویژگی های کیفی خصوصیاتی از سیستم هستند که از عملکرد سیستم جدا هستند. پیاده سازی ویژگی های کیفیت، تمایز یک سیستم خوب از یک سیستم بد را آسان می کند. این ویژگی ها به طور کلی عواملی هستند که بر رفتار زمان اجرا، طراحی سیستم و تجربه کاربر تاثیر می گذارند.

ویژگی های کیفی را می توان در موارد زیر طبقه بندی کرد:

### ویژگی های کیفیت استاتیک:

انعکاس ساختار یک سیستم و سازمان که مستقیماً با معماری، طراحی و کد منبع مرتبط است.
این موارد برای کاربر نهایی نامرئی هستند اما بر هزینه توسعه و نگهداری تاثیر می گذارند.

به عنوان مثال: ماژولار بودن، قابلیت تست، قابلیت نگهداری و غیره

### ویژگی های کیفیت پویا:

این ویژگی ها بازتاب رفتار سیستم در هنگام اجرای آن است که مستقیما با معماری، طراحی، کد منبع، پیکربندی، پارامترهای استقرار، محیط و بستر سیستم ارتباط دارند. این موارد برای کاربر نهایی قابل مشاهده هستند و در زمان اجرا وجود دارند. به عنوان مثال توان عملیاتی، قدرت، مقیاس پذیری و غیره.

## ابزار های معماری نرم افزار
### زبان های مدلسازی

#### <p align="right">:UMl</p>
          
          
استاندارد جهانی برای ایجاد مصنوعات معماری و طراحی از زمان شروع آن در سالهای 1994-1995 است.

این استاندارد توسط سازمان بین المللی استاندارد (ISO) به عنوان استاندارد ISO مورد تایید پذیرفته شد و از آن زمان توسط معماران و طراحان برای مستندسازی معماری نرم افزار استفاده می شود.
به طور کلی می توانید نمودارهای ساختاری، رفتاری یا تعاملی را با استفاده از UML ایجاد کنید.

### ابزار مدل سازی معماری

پس از انتخاب زبان مدلسازی نوبت به انتخاب معماری و ابزار مدل سازی مناسب در زمینه سازمان و مرتبط به سیستم و برنامه است.
#### نمونه هایی ابزار های مدلسازی معماری:
![image](https://user-images.githubusercontent.com/61993604/171989522-f4dd53c3-7888-4ae8-9932-c4f6845568fd.png)



## نتیجه

معماری نرم افزار یکی از مهم ترین گام ها پیش از شروع به پیاده سازی هر گونه سیستم و نرم افزار است که باید روی آن توجه اکید داشت تا کیفیت کلی و قابلیت اطمینان سیستم به بالاترین حد خود برسد و میزان هزینه ها تا حد ممکن کاهش یابد. همچنین باعث دیباگ کردن آسان سیستم و اضافه کردن قابلیت های جدید بدون دخالت در ساختار قسمت های دیگر می شود، امنیت را به حد قابل قبول میرساند و تمامی نیاز های کاربران و کارفرمایان را برطرف می کند.
با توجه به این مطالب مهندسی معماری یکی از شاخه هایی است که دارای اهمیت بسیار بالایی است و افراد علاقه مند میتوانند با افزایش یادگیری خود در این زمینه به موقعیت های شغلی مناسبی دست پیدا کنند.

## منابع

https://barnamenevisan.org/Articles/Article5140.html

https://namatek.com/%D9%85%D8%B9%D9%85%D8%A7%D8%B1%DB%8C-%D9%86%D8%B1%D9%85-%D8%A7%D9%81%D8%B2%D8%A7%D8%B1/

https://vrgl.ir/2hAYR

https://www.altexsoft.com/blog/software-architect-role/

https://www.tutorialspoint.com/software_architecture_design/introduction.htm#

https://vedcraft.com/architecture/top-10-tools-you-should-know-for-software-architecture-and-design-diagrams/

