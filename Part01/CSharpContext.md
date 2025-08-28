
<div dir="rtl" style="text-align: right;">

# بقاء تیزترین‌ها

زمانی که در دانشگاه مشغول تحصیل در رشته **علوم کامپیوتر** (*Computer Science*) بودم، یکی از همکلاسی‌هایم، استاد را در مورد جزئیاتی که روی تخته سیاه (*Blackboard*) نوشته بود، تصحیح کرد. استاد با حالتی کمی کلافه به نظر می‌رسید و پاسخ داد: "بله، می‌دانم. داشتم ساده‌سازی (*Simplifying*) می‌کردم. اینجا دارم حقیقت را پنهان می‌کنم تا حقیقت بزرگ‌تری را نشان دهم." اگرچه امیدوارم در بخش 1 (*Part 1*) چیز زیادی را پنهان نکنم، اما قطعاً در مورد حقیقت بزرگ‌تر است.

بیشتر این کتاب به بررسی دقیق سی‌شارپ (*C#*) می‌پردازد و گاهی اوقات آن را زیر میکروسکوپ (*Microscope*) قرار می‌دهد تا ریزترین جزئیات را ببیند. قبل از اینکه این کار را شروع کنیم، فصل 1 (*Chapter 1*) لنز (*Lens*) را عقب می‌کشد تا نگاهی کلی به تاریخچه سی‌شارپ (*C#*) و اینکه چگونه سی‌شارپ (*C#*) در زمینه وسیع‌تر محاسبات (*Computing*) قرار می‌گیرد، بیندازیم.

شما مقداری کد (*Code*) را به عنوان پیش‌غذا (*Appetizer*) خواهید دید، قبل از اینکه غذای اصلی (*Main Course*) بقیه کتاب را سرو کنم، اما جزئیات در این مرحله مهم نیستند. این بخش بیشتر در مورد ایده‌ها (*Ideas*) و مضامین (*Themes*) توسعه سی‌شارپ (*C#*) است تا شما را در بهترین حالت ذهنی (*Frame of Mind*) برای درک نحوه پیاده‌سازی (*Implemented*) این ایده‌ها قرار دهد.

بزن بریم!

## بقاء تیزترین‌ها

این فصل شامل موارد زیر است:
- چگونه تکامل (*Evolution*) سریع سی‌شارپ (*C#*) توسعه‌دهندگان (*Developers*) را بهره‌ورتر (*Productive*) کرده است.
- انتخاب نسخه‌های فرعی (*Minor Versions*) سی‌شارپ (*C#*) برای استفاده از آخرین ویژگی‌ها (*Features*).
- قابلیت اجرای سی‌شارپ (*C#*) در محیط‌های (*Environments*) بیشتر.
- بهره‌مندی از یک جامعه (*Community*) باز و فعال.
- تمرکز کتاب بر نسخه‌های (*Versions*) قدیمی و جدید سی‌شارپ (*C#*).

انتخاب جالب‌ترین جنبه‌های سی‌شارپ (*C#*) برای معرفی در اینجا دشوار بود. برخی جذاب هستند اما به ندرت استفاده می‌شوند. برخی دیگر فوق‌العاده مهم هستند اما اکنون برای توسعه‌دهندگان (*Developers*) سی‌شارپ (*C#*) عادی شده‌اند. ویژگی‌هایی مانند async/await از بسیاری جهات عالی هستند اما توضیح مختصر آن‌ها دشوار است. بدون اتلاف وقت بیشتر، بیایید ببینیم سی‌شارپ (*C#*) در طول زمان چقدر پیشرفت کرده است.

## 1.1 یک زبان در حال تکامل (*Evolving Language*)

در ویرایش‌های (*Editions*) قبلی این کتاب، من یک مثال (*Example*) واحد ارائه کردم که تکامل (*Evolution*) زبان را در نسخه‌های (*Versions*) تحت پوشش آن ویرایش نشان می‌داد. این کار دیگر به گونه‌ای که خواندن آن جالب باشد، امکان‌پذیر نیست. اگرچه یک برنامه (*Application*) بزرگ ممکن است تقریباً از تمام ویژگی‌های (*Features*) جدید استفاده کند، اما هر قطعه کد (*Code*) واحدی که برای صفحه چاپی مناسب باشد، تنها از زیرمجموعه‌ای (*Subset*) از آن‌ها استفاده می‌کند.

در عوض، در این بخش، آنچه را که مهم‌ترین مضامین (*Themes*) تکامل (*Evolution*) سی‌شارپ (*C#*) می‌دانم، انتخاب می‌کنم و مثال‌های (*Examples*) مختصری از بهبودها (*Improvements*) ارائه می‌دهم. این به هیچ وجه لیست جامعی (*Exhaustive List*) از ویژگی‌ها (*Features*) نیست. همچنین قصد آموزش این ویژگی‌ها را ندارد؛ بلکه یادآوری می‌کند که ویژگی‌هایی که از قبل می‌دانید چقدر زبان را بهبود بخشیده‌اند و همچنین اشاره‌ای به ویژگی‌هایی می‌کند که ممکن است هنوز ندیده‌اید.

اگر فکر می‌کنید برخی از این ویژگی‌ها (*Features*) از زبان‌های (*Languages*) دیگری که با آن‌ها آشنا هستید تقلید می‌کنند، تقریباً مطمئناً درست می‌گویید. تیم سی‌شارپ (*C#*) در استفاده از ایده‌های عالی از زبان‌های دیگر و تغییر شکل آن‌ها برای اینکه در سی‌شارپ (*C#*) احساس راحتی کنند، تردیدی ندارد. این چیز بسیار خوبی است! اف‌شارپ (*F#*) به ویژه به عنوان منبع الهام (*Source of Inspiration*) برای بسیاری از ویژگی‌های (*Features*) سی‌شارپ (*C#*) قابل ذکر است.

### نکته:

این احتمال وجود دارد که بزرگترین تأثیر اف‌شارپ (*F#*) آن چیزی نباشد که برای توسعه‌دهندگان (*Developers*) اف‌شارپ (*F#*) فراهم می‌کند، بلکه تأثیر آن بر سی‌شارپ (*C#*) باشد. این به معنای کم ارزش جلوه دادن ارزش اف‌شارپ (*F#*) به عنوان یک زبان (*Language*) مستقل یا پیشنهاد عدم استفاده مستقیم از آن نیست. اما در حال حاضر، جامعه (*Community*) سی‌شارپ (*C#*) به طور قابل توجهی بزرگتر از جامعه (*Community*) اف‌شارپ (*F#*) است، و جامعه (*Community*) سی‌شارپ (*C#*) به دلیل الهام بخشیدن به تیم سی‌شارپ (*C#*)، مدیون اف‌شارپ (*F#*) است.


</div>


<div dir="rtl" style="text-align: right;">

## 1.1.1 یک سیستم نوع (*Type System*) مفید در مقیاس‌های بزرگ و کوچک

سی‌شارپ (*C#*) از ابتدا یک زبان با تایپ استاتیک (*Statically Typed Language*) بوده است: کد شما انواع (*Types*) متغیرها (*Variables*)، پارامترها (*Parameters*)، مقادیر بازگردانده شده از متدها (*Methods*) و غیره را مشخص می‌کند. هرچه دقیق‌تر بتوانید شکل داده‌هایی (*Data*) را که کد شما می‌پذیرد و بازمی‌گرداند، مشخص کنید، کامپایلر (*Compiler*) بیشتر می‌تواند به شما در جلوگیری از اشتباهات (*Mistakes*) کمک کند.

این امر به ویژه با رشد برنامه‌ای (*Application*) که می‌سازید، صادق است. اگر بتوانید تمام کد (*Code*) برنامه خود را در یک صفحه نمایش (*Screen*) ببینید (یا حداقل همه آن را به طور همزمان در ذهن خود نگه دارید)، یک زبان با تایپ استاتیک (*Statically Typed Language*) مزیت زیادی ندارد. با افزایش مقیاس، ارتباط مختصر و مؤثر کد شما از آنچه انجام می‌دهد، اهمیت فزاینده‌ای پیدا می‌کند. می‌توانید این کار را از طریق مستندات (*Documentation*) انجام دهید، اما تایپ استاتیک (*Static Typing*) به شما امکان می‌دهد به روشی قابل خواندن برای ماشین (*Machine-Readable Way*) ارتباط برقرار کنید.

همانطور که سی‌شارپ (*C#*) تکامل یافته است، سیستم نوع (*Type System*) آن امکان توصیف‌های دقیق‌تری را فراهم کرده است. واضح‌ترین مثال (*Example*) این موضوع، جنریک‌ها (*Generics*) هستند. در سی‌شارپ 1 (*C# 1*)، ممکن بود کدی مانند این داشته باشید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
public class Bookshelf
{
    public IEnumerable Books { get { ... } }
}
```

</div>

<div dir="rtl" style="text-align: right;">

نوع هر آیتم (*Item*) در دنباله (*Sequence*) Books چیست؟ سیستم نوع (*Type System*) به شما نمی‌گوید. با جنریک‌ها (*Generics*) در سی‌شارپ 2 (*C# 2*)، می‌توانید مؤثرتر ارتباط برقرار کنید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
public class Bookshelf
{
    public IEnumerable<Book> Books { get { ... } }
}
```

</div>

<div dir="rtl" style="text-align: right;">

سی‌شارپ 2 (*C# 2*) همچنین انواع مقادیر null پذیر (*Nullable Value Types*) را به ارمغان آورد و به این ترتیب امکان بیان مؤثر عدم وجود اطلاعات را بدون توسل به مقادیر جادویی (*Magic Values*) مانند -1 برای یک شاخص مجموعه (*Collection Index*) یا DateTime.MinValue برای یک تاریخ (*Date*) فراهم کرد.

سی‌شارپ 7 (*C# 7*) به ما این امکان را داد که به کامپایلر (*Compiler*) بگوییم که یک ساختار (*Struct*) تعریف شده توسط کاربر (*User-Defined*) باید با استفاده از اعلان‌های readonly struct تغییرناپذیر (*Immutable*) باشد. هدف اصلی این ویژگی (*Feature*) ممکن است بهبود کارایی (*Efficiency*) کد تولید شده توسط کامپایلر (*Compiler*) باشد، اما مزایای اضافی برای انتقال قصد (*Intent*) دارد.

برنامه‌های سی‌شارپ 8 (*C# 8*) شامل انواع مرجع null پذیر (*Nullable Reference Types*) است که ارتباط بیشتری را امکان‌پذیر می‌سازد. تا این مرحله، هیچ چیز در زبان به شما اجازه نمی‌دهد که بیان کنید آیا یک مرجع (*Reference*) (چه به عنوان یک مقدار بازگشتی (*Return Value*)، یک پارامتر (*Parameter*) یا فقط یک متغیر محلی (*Local Variable*)) ممکن است null باشد یا خیر. این منجر به کد مستعد خطا (*Error-Prone Code*) می‌شود اگر دقت نکنید و کد اعتبارسنجی (*Validation Code*) تکراری (*Boilerplate*) اگر دقت کنید، که هیچ یک ایده‌آل نیستند. سی‌شارپ 8 (*C# 8*) انتظار دارد هر چیزی که صراحتاً null پذیر نیست، قصد دارد null پذیر نباشد. به عنوان مثال، یک اعلان متد (*Method Declaration*) مانند این را در نظر بگیرید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
string Method(string x, string? y)
```

</div>

<div dir="rtl" style="text-align: right;">

انواع پارامتر (*Parameter Types*) نشان می‌دهند که آرگومان (*Argument*) مربوط به x نباید null باشد اما آرگومان (*Argument*) مربوط به y ممکن است null باشد. نوع بازگشتی (*Return Type*) نشان می‌دهد که متد (*Method*) null را بازنخواهد گرداند.

</div>


<div dir="rtl" style="text-align: right;">

تغییرات دیگر در سیستم نوع (*Type System*) در سی‌شارپ (*C#*) در مقیاس کوچک‌تری هدف‌گذاری شده‌اند و بر نحوه پیاده‌سازی (*Implemented*) یک متد (*Method*) تمرکز دارند تا نحوه ارتباط اجزای مختلف (*Different Components*) در یک سیستم بزرگ. سی‌شارپ 3 (*C# 3*) انواع ناشناس (*Anonymous Types*) و متغیرهای محلی با تایپ ضمنی (*Implicitly Typed Local Variables*) (var) را معرفی کرد. اینها به رفع جنبه منفی برخی زبان‌های با تایپ استاتیک (*Statically Typed Languages*) کمک می‌کنند: پرگویی (*Verbosity*). اگر به یک شکل داده (*Data Shape*) خاص در یک متد (*Method*) واحد نیاز دارید اما در هیچ جای دیگری، ایجاد یک نوع (*Type*) اضافی کامل فقط به خاطر آن متد (*Method*) زیاده‌روی است. انواع ناشناس (*Anonymous Types*) اجازه می‌دهند که آن شکل داده (*Data Shape*) به طور مختصر بیان شود بدون از دست دادن مزایای تایپ استاتیک (*Static Typing*):

</div>

<div dir="ltr" style="text-align: left;">

```csharp
var book = new { Title = "Lost in the Snow", Author = "Holly Webb" };
string title = book.Title;
string author = book.Author;
```

</div>

<div dir="rtl" style="text-align: right;">

انواع ناشناس (*Anonymous Types*) در درجه اول در کوئری‌های (*Queries*) LINQ استفاده می‌شوند، اما اصل ایجاد یک نوع (*Type*) فقط برای یک متد (*Method*) واحد به LINQ بستگی ندارد.

به طور مشابه، به نظر می‌رسد که مشخص کردن صریح نوع یک متغیر (*Variable*) که در همان عبارت (*Statement*) با فراخوانی سازنده (*Constructor*) آن نوع مقداردهی اولیه (*Initialized*) می‌شود، اضافی است. من می‌دانم که کدام یک از اعلان‌های (*Declarations*) زیر را تمیزتر می‌یابم:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
Dictionary<string, string> map1 = new Dictionary<string, string>();
var map2 = new Dictionary<string, string>();
```

</div>

<div dir="rtl" style="text-align: right;">

اگرچه تایپ ضمنی (*Implicit Typing*) هنگام کار با انواع ناشناس (*Anonymous Types*) ضروری است، اما متوجه شده‌ام که هنگام کار با انواع معمولی (*Regular Types*) نیز به طور فزاینده‌ای مفید است. تمایز بین تایپ ضمنی (*Implicit Typing*) و تایپ پویا (*Dynamic Typing*) مهم است. متغیر map2 قبلی هنوز به صورت استاتیک (*Statically Typed*) تایپ شده است، اما نیازی نبود که نوع (*Type*) را به صراحت بنویسید.

انواع ناشناس (*Anonymous Types*) فقط در یک بلوک کد (*Block of Code*) کمک می‌کنند؛ به عنوان مثال، نمی‌توانید از آنها به عنوان پارامترهای (*Parameters*) متد (*Method*) یا انواع بازگشتی (*Return Types*) استفاده کنید. سی‌شارپ 7 (*C# 7*) تاپل‌ها (*Tuples*) را معرفی کرد: انواع مقداری (*Value Types*) که به طور مؤثر برای جمع‌آوری متغیرها (*Variables*) با هم عمل می‌کنند. پشتیبانی فریم‌ورک (*Framework Support*) برای این تاپل‌ها (*Tuples*) نسبتاً ساده است، اما پشتیبانی زبان (*Language Support*) اضافی به عناصر (*Elements*) تاپل‌ها (*Tuples*) اجازه می‌دهد نام‌گذاری شوند. به عنوان مثال، به جای نوع ناشناس (*Anonymous Type*) قبلی، می‌توانید از موارد زیر استفاده کنید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
var book = (title: "Lost in the Snow", author: "Holly Webb");
Console.WriteLine(book.title);
```

</div>

<div dir="rtl" style="text-align: right;">

تاپل‌ها (*Tuples*) می‌توانند در برخی موارد جایگزین انواع ناشناس (*Anonymous Types*) شوند، اما قطعاً نه در همه موارد. یکی از مزایای آنها این است که می‌توانند به عنوان پارامترهای (*Parameters*) متد (*Method*) و انواع بازگشتی (*Return Types*) استفاده شوند. در حال حاضر، من توصیه می‌کنم که اینها در API داخلی (*Internal API*) یک برنامه (*Program*) نگه داشته شوند تا اینکه به صورت عمومی (*Publicly*) در معرض دید قرار گیرند، زیرا تاپل‌ها (*Tuples*) یک ترکیب (*Composition*) ساده از مقادیر را نشان می‌دهند تا اینکه آنها را کپسوله (*Encapsulating*) کنند. به همین دلیل است که من هنوز آنها را به عنوان کمک کننده به کد ساده‌تر (*Simpler Code*) در سطح پیاده‌سازی (*Implementation Level*) می‌دانم تا بهبود طراحی کلی برنامه (*Overall Program Design*).

</div>


<div dir="rtl" style="text-align: right;">

### ویژگی رکورد (*Record Types*)

من باید به یک ویژگی (*Feature*) که ممکن است در سی‌شارپ 8 (*C# 8*) عرضه شود، اشاره کنم: انواع رکورد (*Record Types*). من اینها را تا حدودی، حداقل در ساده‌ترین شکل خود، به عنوان انواع ناشناس (*Anonymous Types*) نام‌گذاری شده می‌دانم. آنها مزایای انواع ناشناس (*Anonymous Types*) را از نظر حذف کد تکراری (*Boilerplate Code*) فراهم می‌کنند، اما سپس به آن انواع (*Types*) اجازه می‌دهند که رفتار (*Behavior*) اضافی مانند کلاس‌های (*Classes*) معمولی به دست آورند. منتظر باشید!

## 1.1.2 کد (*Code*) مختصرتر از همیشه

یکی از مضامین (*Themes*) تکرارشونده در ویژگی‌های (*Features*) جدید سی‌شارپ (*C#*)، توانایی آن در بیان ایده‌های شما به روش‌های هرچه گویاتر و مختصرتر است. سیستم نوع (*Type System*) بخشی از این موضوع است، همانطور که با انواع ناشناس (*Anonymous Types*) دیدید، اما بسیاری از ویژگی‌های (*Features*) دیگر نیز به این امر کمک می‌کنند. کلمات زیادی ممکن است برای این موضوع بشنوید، به خصوص در مورد آنچه که با ویژگی‌های (*Features*) جدید می‌توان حذف کرد. ویژگی‌های (*Features*) سی‌شارپ (*C#*) به شما امکان می‌دهند "مراسم (*Ceremony*)" را کاهش دهید، "کد تکراری (*Boilerplate Code*)" را حذف کنید و از "پیچیدگی بیهوده (*Cruft*)" اجتناب کنید. اینها فقط راه‌های مختلفی برای صحبت در مورد یک اثر یکسان هستند. اینطور نیست که هیچ یک از کدهای (*Code*) اضافی اکنون اشتباه بوده باشند؛ بلکه فقط گیج‌کننده و غیرضروری بودند. بیایید به چند روشی نگاه کنیم که سی‌شارپ (*C#*) در این زمینه تکامل یافته است.

### ساخت و مقداردهی اولیه (*Construction and Initialization*)

ابتدا، نحوه ایجاد (*Create*) و مقداردهی اولیه (*Initialize*) اشیاء (*Objects*) را بررسی می‌کنیم. دلیگیت‌ها (*Delegates*) احتمالاً بیشترین و در چندین مرحله تکامل یافته‌اند. در سی‌شارپ 1 (*C# 1*)، شما باید یک متد (*Method*) جداگانه برای ارجاع دلیگیت (*Delegate*) می‌نوشتید و سپس خود دلیگیت (*Delegate*) را به روشی طولانی ایجاد می‌کردید. به عنوان مثال، در اینجا چیزی است که برای اشتراک یک کنترل کننده رویداد (*Event Handler*) جدید در رویداد (*Event*) Click یک دکمه (*Button*) در سی‌شارپ 1 (*C# 1*) می‌نوشتید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
button.Click += new EventHandler(HandleButtonClick);
```

</div>

<div dir="rtl" style="text-align: right;">

سی‌شارپ 2 (*C# 2*) تبدیل گروه متد (*Method Group Conversions*) و متدهای ناشناس (*Anonymous Methods*) را معرفی کرد. اگر می‌خواستید متد (*Method*) HandleButtonClick را حفظ کنید، تبدیل گروه متد (*Method Group Conversions*) به شما امکان می‌داد کد (*Code*) قبلی را به شکل زیر تغییر دهید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
button.Click += HandleButtonClick;
```

</div>

<div dir="rtl" style="text-align: right;">

اگر کنترل کننده کلیک (*Click Handler*) شما ساده باشد، ممکن است اصلاً نخواهید با یک متد (*Method*) جداگانه زحمت بکشید و در عوض از یک متد (*Method*) ناشناس (*Anonymous Method*) استفاده کنید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
button.Click += delegate { MessageBox.Show("Clicked!"); };
```

</div>

<div dir="rtl" style="text-align: right;">

متدهای ناشناس (*Anonymous Methods*) مزیت اضافی عمل به عنوان Closure را دارند: آنها می‌توانند از متغیرهای محلی (*Local Variables*) در زمینه‌ای که در آن ایجاد شده‌اند استفاده کنند. با این حال، آنها اغلب در کد (*Code*) مدرن سی‌شارپ (*C#*) استفاده نمی‌شوند، زیرا سی‌شارپ 3 (*C# 3*) به ما عبارات لامبدا (*Lambda Expressions*) را ارائه داد که تقریباً تمام مزایای متدهای ناشناس (*Anonymous Methods*) را دارند اما سینتکس (*Syntax*) کوتاه‌تری دارند:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
button.Click += (sender, args) => MessageBox.Show("Clicked!");
```

</div>

<div dir="rtl" style="text-align: right;">

> **نکته**: در این مورد، عبارت لامبدا (*Lambda Expression*) طولانی‌تر از متد (*Method*) ناشناس (*Anonymous Method*) است زیرا متد (*Method*) ناشناس (*Anonymous Method*) از یک ویژگی (*Feature*) استفاده می‌کند که عبارات لامبدا (*Lambda Expressions*) ندارند: توانایی نادیده گرفتن پارامترها (*Parameters*) با عدم ارائه لیست پارامتر (*Parameter List*).

من از کنترل کننده‌های رویداد (*Event Handlers*) به عنوان مثالی (*Example*) برای دلیگیت‌ها (*Delegates*) استفاده کردم زیرا این استفاده اصلی آنها در سی‌شارپ 1 (*C# 1*) بود. در نسخه‌های بعدی سی‌شارپ (*C#*)، دلیگیت‌ها (*Delegates*) در موقعیت‌های متنوع‌تری، به ویژه در LINQ، استفاده می‌شوند.

</div>


<div dir="rtl" style="text-align: right;">

LINQ همچنین مزایای دیگری را برای مقداردهی اولیه (*Initialization*) در قالب مقداردهی اولیه شی (*Object Initializers*) و مقداردهی اولیه مجموعه (*Collection Initializers*) به ارمغان آورد. اینها به شما امکان می‌دهند مجموعه‌ای از ویژگی‌ها (*Properties*) را برای تنظیم روی یک شی (*Object*) جدید یا آیتم‌ها (*Items*) را برای افزودن به یک مجموعه (*Collection*) جدید در یک عبارت (*Expression*) واحد مشخص کنید. نشان دادن آن ساده‌تر از توصیف آن است، و من از فصل 3 (*Chapter 3*) یک مثال (*Example*) قرض خواهم گرفت. کدی (*Code*) را در نظر بگیرید که قبلاً ممکن بود به این صورت می‌نوشتید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
var customer = new Customer();
customer.Name = "Jon";
customer.Address = "UK";
var item1 = new OrderItem();
item1.ItemId = "abcd123";
item1.Quantity = 1;
var item2 = new OrderItem();
item2.ItemId = "fghi456";
item2.Quantity = 2;
var order = new Order();
order.OrderId = "xyz";
order.Customer = customer;
order.Items.Add(item1);
order.Items.Add(item2);
```

</div>

<div dir="rtl" style="text-align: right;">

مقداردهی اولیه شی (*Object Initializers*) و مقداردهی اولیه مجموعه (*Collection Initializers*) معرفی شده در سی‌شارپ 3 (*C# 3*) این را بسیار واضح‌تر می‌کند:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
var order = new Order
{
    OrderId = "xyz",
    Customer = new Customer { Name = "Jon", Address = "UK" },
    Items =
    {
        new OrderItem { ItemId = "abcd123", Quantity = 1 },
        new OrderItem { ItemId = "fghi456", Quantity = 2 }
    }
};
```

</div>

<div dir="rtl" style="text-align: right;">

من پیشنهاد نمی‌کنم که هیچ یک از این مثال‌ها (*Examples*) را با جزئیات بخوانید؛ آنچه مهم است سادگی فرم (*Form*) دوم نسبت به فرم (*Form*) اول است.

### اعلان‌های متد (*Method and Property Declarations*) و ویژگی (*Property*)

یکی از واضح‌ترین مثال‌ها (*Examples*) ساده‌سازی از طریق ویژگی‌های (*Properties*) پیاده‌سازی شده خودکار (*Automatically Implemented*) است. اینها اولین بار در سی‌شارپ 3 (*C# 3*) معرفی شدند اما در نسخه‌های بعدی بهبود یافته‌اند. ویژگی (*Property*) را در نظر بگیرید که در سی‌شارپ 1 (*C# 1*) به این صورت پیاده‌سازی می‌شد:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
private string name;
public string Name
{
    get { return name; }
    set { name = value; }
}
```

</div>

<div dir="rtl" style="text-align: right;">

ویژگی‌های (*Properties*) پیاده‌سازی شده خودکار (*Automatically Implemented*) اجازه می‌دهند این به صورت یک خط (*Single Line*) نوشته شود:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
public string Name { get; set; }
```

</div>

<div dir="rtl" style="text-align: right;">

علاوه بر این، سی‌شارپ 6 (*C# 6*) اعضای با بدنه عبارت (*Expression-Bodied Members*) را معرفی کرد که "مراسم (*Ceremony*)" بیشتری را حذف می‌کنند. فرض کنید کلاسی (*Class*) می‌نویسید که یک مجموعه (*Collection*) موجود از رشته‌ها (*Strings*) را می‌پوشاند، و می‌خواهید اعضای Count و GetEnumerator() کلاس (*Class*) خود را به طور مؤثر به آن مجموعه (*Collection*) محول کنید. قبل از سی‌شارپ 6 (*C# 6*)، مجبور بودید چیزی شبیه به این بنویسید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
public int Count { get { return list.Count; } }
public IEnumerator<string> GetEnumerator()
{
    return list.GetEnumerator();
}
```

</div>

<div dir="rtl" style="text-align: right;">

این یک مثال (*Example*) قوی از "مراسم (*Ceremony*)" است: سینتکس (*Syntax*) زیادی که زبان (*Language*) قبلاً با سود کمی نیاز داشت. در سی‌شارپ 6 (*C# 6*)، این به طور قابل توجهی تمیزتر است. سینتکس (*Syntax*) => (که قبلاً توسط عبارات لامبدا (*Lambda Expressions*) استفاده می‌شد) برای نشان دادن یک عضو با بدنه عبارت (*Expression-Bodied Member*) استفاده می‌شود:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
public int Count => list.Count;
public IEnumerator<string> GetEnumerator() => list.GetEnumerator();
```

</div>

<div dir="rtl" style="text-align: right;">

اگرچه ارزش استفاده از اعضای با بدنه عبارت (*Expression-Bodied Members*) یک موضوع شخصی و ذهنی است، اما من از اینکه چقدر تفاوت در خوانایی (*Readability*) کد (*Code*) من ایجاد کرده‌اند شگفت‌زده شده‌ام. من عاشق آنها هستم! یکی دیگر از ویژگی‌هایی (*Features*) که انتظار نداشتم به این اندازه از آن استفاده کنم، الحاق رشته (*String Interpolation*) است، که یکی از بهبودهای مرتبط با رشته (*String*) در سی‌شارپ (*C#*) است.

### مدیریت رشته (*String Handling*)

مدیریت رشته (*String Handling*) در سی‌شارپ (*C#*) سه بهبود قابل توجه داشته است:
- سی‌شارپ 5 (*C# 5*) ویژگی‌های (*Attributes*) اطلاعات فراخواننده (*Caller Information*) را معرفی کرد، از جمله توانایی کامپایلر (*Compiler*) برای پر کردن خودکار نام‌های متد (*Method*) و فایل (*Filenames*) به عنوان مقادیر پارامتر (*Parameter Values*). این برای اهداف تشخیصی (*Diagnostic Purposes*)، چه در ثبت دائمی (*Permanent Logging*) و چه در آزمایش موقت (*Temporary Testing*)، عالی است.
- سی‌شارپ 6 (*C# 6*) عملگر nameof را معرفی کرد که به نام‌های متغیرها (*Variables*)، انواع (*Types*)، متدها (*Methods*) و سایر اعضا (*Members*) اجازه می‌دهد به شکلی قابل تغییر (*Refactoring-Friendly Form*) نمایش داده شوند.
- سی‌شارپ 6 (*C# 6*) همچنین لیترال‌های (*Literals*) رشته‌ای الحاقی (*Interpolated String*) را معرفی کرد. این یک مفهوم جدید نیست، اما ساخت یک رشته (*String*) با مقادیر پویا (*Dynamic Values*) را بسیار ساده‌تر می‌کند.

به خاطر اختصار، من فقط نکته آخر را نشان خواهم داد. ساخت یک رشته (*String*) با متغیرها (*Variables*)، ویژگی‌ها (*Properties*)، نتیجه فراخوانی متدها (*Method Calls*) و غیره به طور منطقی رایج است. این ممکن است برای اهداف ثبت (*Logging Purposes*)، پیام‌های خطای (*Error Messages*) کاربر محور (*User-Oriented*) (اگر بومی‌سازی (*Localization*) لازم نباشد)، پیام‌های استثنا (*Exception Messages*) و غیره باشد.

</div>

<div dir="rtl" style="text-align: right;">

در اینجا یک مثال (*Example*) از پروژه Noda Time من آورده شده است. کاربران می‌توانند سعی کنند یک سیستم تقویم (*Calendar System*) را با ID آن پیدا کنند، و اگر آن ID وجود نداشته باشد، کد (*Code*) یک KeyNotFoundException را پرتاب می‌کند. قبل از سی‌شارپ 6 (*C# 6*)، کد (*Code*) ممکن بود به این صورت به نظر برسد:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
throw new KeyNotFoundException(
    "No calendar system for ID " + id + " exists");
```

</div>

<div dir="rtl" style="text-align: right;">

با استفاده از فرمت‌بندی صریح رشته (*Explicit String Formatting*)، به این صورت به نظر می‌رسد:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
throw new KeyNotFoundException(
    string.Format("No calendar system for ID {0} exists", id);
```

</div>

<div dir="rtl" style="text-align: right;">

> **نکته**: برای اطلاعات در مورد Noda Time به بخش 1.4.2 مراجعه کنید. برای درک این مثال (*Example*) نیازی به دانستن آن ندارید.

در سی‌شارپ 6 (*C# 6*)، کد (*Code*) با یک لیترال (*Literal*) رشته‌ای الحاقی (*Interpolated String*) برای گنجاندن مستقیم مقدار id در رشته (*String*) کمی ساده‌تر می‌شود:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
throw new KeyNotFoundException($"No calendar system for ID {id} exists");
```

</div>

<div dir="rtl" style="text-align: right;">

این به نظر یک مسئله بزرگ نمی‌آید، اما من از اینکه الان مجبور باشم بدون الحاق رشته (*String Interpolation*) کار کنم متنفرم.

اینها فقط برجسته‌ترین ویژگی‌هایی (*Features*) هستند که به بهبود نسبت سیگنال به نویز (*Signal-to-Noise Ratio*) کد (*Code*) شما کمک می‌کنند. می‌توانستم از دستورات static و عملگر شرطی null (*Null Conditional Operator*) در سی‌شارپ 6 (*C# 6*) و همچنین تطبیق الگو (*Pattern Matching*)، تجزیه (*Deconstruction*) و متغیرهای out در سی‌شارپ 7 (*C# 7*) نیز نشان دهم. به جای گسترش این فصل برای ذکر هر ویژگی (*Feature*) در هر نسخه، بیایید به یک ویژگی (*Feature*) برویم که انقلابی‌تر (*Revolutionary*) از تکاملی (*Evolutionary*) است: LINQ.

## 1.1.3 دسترسی ساده به داده (*Data Access*) با LINQ

اگر از توسعه‌دهندگان (*Developers*) سی‌شارپ (*C#*) بپرسید که چه چیزی را در مورد سی‌شارپ (*C#*) دوست دارند، احتمالاً به LINQ اشاره خواهند کرد. شما قبلاً برخی از ویژگی‌هایی (*Features*) را که منجر به LINQ می‌شوند، دیده‌اید، اما رادیکال‌ترین آنها عبارات کوئری (*Query Expressions*) هستند. این کد (*Code*) را در نظر بگیرید:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
var offers =
    from product in db.Products
    where product.SalePrice <= product.Price / 2
    orderby product.SalePrice
    select new {
        product.Id, product.Description,
        product.SalePrice, product.Price
    };
```

</div>

<div dir="rtl" style="text-align: right;">

این اصلاً شبیه سی‌شارپ (*C#*) قدیمی نیست. تصور کنید به سال 2007 برگردید و این کد (*Code*) را به یک توسعه‌دهنده (*Developer*) که از سی‌شارپ 2 (*C# 2*) استفاده می‌کند، نشان دهید و سپس توضیح دهید که این دارای بررسی زمان کامپایل (*Compile-Time Checking*) و پشتیبانی IntelliSense است و منجر به یک کوئری (*Query*) کارآمد پایگاه داده (*Database Query*) می‌شود. اوه، و اینکه می‌توانید از همان سینتکس (*Syntax*) برای مجموعه‌های (*Collections*) معمولی نیز استفاده کنید.

پشتیبانی برای کوئری (*Query*) داده‌های خارج از فرآیند (*Out-of-Process Data*) از طریق درختان عبارت (*Expression Trees*) فراهم می‌شود. اینها کد (*Code*) را به عنوان داده (*Data*) نمایش می‌دهند، و یک فراهم کننده LINQ می‌تواند کد (*Code*) را تجزیه و تحلیل کند تا آن را به SQL یا سایر زبان‌های کوئری (*Query Languages*) تبدیل کند. اگرچه این بسیار جالب است، من به ندرت خودم از آن استفاده می‌کنم، زیرا اغلب با پایگاه‌های داده (*Databases*) SQL کار نمی‌کنم. من با مجموعه‌های (*Collections*) درون حافظه (*In-Memory*) کار می‌کنم، و همیشه از LINQ استفاده می‌کنم، چه از طریق عبارات کوئری (*Query Expressions*) و چه فراخوانی متدها (*Method Calls*) با عبارات لامبدا (*Lambda Expressions*).

LINQ فقط ابزارهای (*Tools*) جدیدی به توسعه‌دهندگان (*Developers*) سی‌شارپ (*C#*) نداد؛ بلکه ما را تشویق کرد که در مورد تبدیل داده (*Data Transformations*) به روشی جدید بر اساس برنامه‌نویسی تابعی (*Functional Programming*) فکر کنیم. این بیش از دسترسی به داده (*Data Access*) را تحت تأثیر قرار می‌دهد. LINQ انگیزه اولیه را برای پذیرش ایده‌های تابعی (*Functional Ideas*) بیشتر فراهم کرد، اما بسیاری از توسعه‌دهندگان (*Developers*) سی‌شارپ (*C#*) این ایده‌ها را پذیرفته و آنها را فراتر برده‌اند.

سی‌شارپ 4 (*C# 4*) یک تغییر رادیکال (*Radical Change*) از نظر تایپ پویا (*Dynamic Typing*) ایجاد کرد، اما فکر نمی‌کنم این به اندازه LINQ بر توسعه‌دهندگان (*Developers*) تأثیر گذاشت. سپس سی‌شارپ 5 (*C# 5*) آمد و دوباره بازی را تغییر داد، این بار با توجه به ناهمزمانی (*Asynchrony*).

## 1.1.4 ناهمزمانی (*Asynchrony*)

ناهمزمانی (*Asynchrony*) برای مدت طولانی در زبان‌های اصلی (*Mainstream Languages*) دشوار بوده است. زبان‌های تخصصی‌تر (*Niche Languages*) از ابتدا با در نظر گرفتن ناهمزمانی (*Asynchrony*) ایجاد شده‌اند، و برخی از زبان‌های تابعی (*Functional Languages*) آن را نسبتاً آسان کرده‌اند، زیرا یکی از کارهایی است که به طور منظم انجام می‌دهند. اما سی‌شارپ 5 (*C# 5*) سطح جدیدی از وضوح را در برنامه‌نویسی (*Programming*) ناهمزمانی (*Asynchrony*) در یک زبان (*Language*) اصلی (*Mainstream Language*) با ویژگی‌ای (*Feature*) که معمولاً به عنوان async/await شناخته می‌شود، به ارمغان آورد. این ویژگی (*Feature*) شامل دو بخش مکمل (*Complementary Parts*) در اطراف متدهای (*Methods*) ناهمزمان (*Async*) است:

- متدهای (*Methods*) ناهمزمان (*Async*) نتیجه‌ای را تولید می‌کنند که یک عملیات ناهمزمان (*Asynchronous Operation*) را بدون هیچ تلاشی از طرف توسعه‌دهنده (*Developer*) نشان می‌دهد. این نوع نتیجه (*Result Type*) معمولاً Task یا Task<T> است.
- متدهای (*Methods*) ناهمزمان (*Async*) از عبارات await برای مصرف عملیات ناهمزمان (*Asynchronous Operations*) استفاده می‌کنند. اگر متد (*Method*) سعی کند یک عملیات (*Operation*) را که هنوز کامل نشده است await کند، متد (*Method*) به صورت ناهمزمان (*Asynchronously*) متوقف می‌شود تا زمانی که عملیات (*Operation*) کامل شود و سپس ادامه می‌یابد.

</div>


<div dir="rtl" style="text-align: right;">

> **نکته**: به طور دقیق‌تر، می‌توانم اینها را توابع ناهمزمان (*Asynchronous Functions*) بنامم، زیرا متدهای (*Methods*) ناشناس (*Anonymous Methods*) و عبارات لامبدا (*Lambda Expressions*) نیز می‌توانند ناهمزمان (*Asynchronous*) باشند.

دقیقاً منظور از عملیات ناهمزمان (*Asynchronous Operation*) و توقف ناهمزمان (*Pausing Asynchronously*) جایی است که کار دشوار می‌شود، و من سعی نخواهم کرد اکنون آن را توضیح دهم. اما نتیجه این است که می‌توانید کدی (*Code*) بنویسید که ناهمزمان (*Asynchronous*) است اما بیشتر شبیه کد (*Code*) همزمان (*Synchronous Code*) است که با آن آشناتر هستید. حتی به روشی طبیعی امکان همزمانی (*Concurrency*) را فراهم می‌کند. به عنوان مثال، این متد (*Method*) ناهمزمان (*Asynchronous*) را در نظر بگیرید که ممکن است از یک کنترل کننده رویداد (*Event Handler*) Windows Forms فراخوانی شود:

</div>

<div dir="ltr" style="text-align: left;">

```csharp
private async Task UpdateStatus()
{
    Task<Weather> weatherTask = GetWeatherAsync();
    Task<EmailStatus> emailTask = GetEmailStatusAsync();
    // دو عملیات را همزمان شروع می‌کند
    Weather weather = await weatherTask;
    EmailStatus email = await emailTask;
    // به صورت ناهمزمان منتظر می‌ماند تا کامل شوند
    weatherLabel.Text = weather.Description;
    inboxLabel.Text = email.InboxCount.ToString();
    // رابط کاربری را به روز می‌کند
}
```

</div>

<div dir="rtl" style="text-align: right;">

علاوه بر شروع دو عملیات (*Operations*) به صورت همزمان و سپس انتظار برای نتایج آنها، این نشان می‌دهد که چگونه async/await از زمینه‌های همگام‌سازی (*Synchronization Contexts*) آگاه است. شما رابط کاربری (*User Interface*) را به روز می‌کنید، که فقط در یک رشته UI (*UI Thread*) قابل انجام است، با وجود شروع و انتظار برای عملیات‌های (*Operations*) طولانی مدت. قبل از async/await، این پیچیده و مستعد خطا (*Error Prone*) بود.

من ادعا نمی‌کنم که async/await یک راه‌حل جادویی (*Silver Bullet*) برای ناهمزمانی (*Asynchrony*) است. این به طور جادویی تمام پیچیدگی‌هایی (*Complexity*) را که به طور طبیعی با این حوزه همراه است، حذف نمی‌کند. در عوض، به شما اجازه می‌دهد با حذف بسیاری از کد (*Code*) تکراری (*Boilerplate Code*) که قبلاً مورد نیاز بود، بر جنبه‌های ذاتاً دشوار ناهمزمانی (*Asynchrony*) تمرکز کنید.

تمام ویژگی‌هایی (*Features*) که تا کنون دیده‌اید با هدف ساده‌تر کردن کد (*Code*) هستند. آخرین جنبه‌ای که می‌خواهم ذکر کنم کمی متفاوت است.

## 1.1.5 تعادل بین کارایی (*Efficiency*) و پیچیدگی (*Complexity*)

اولین تجربه‌هایم با جاوا (*Java*) را به خاطر می‌آورم؛ کاملاً تفسیر شده و به طرز دردناکی کند بود. پس از مدتی، کامپایلرهای (*Compilers*) JIT (Just-In-Time) اختیاری در دسترس قرار گرفتند، و در نهایت تقریباً مسلم تلقی شد که هر پیاده‌سازی (*Implementation*) جاوا (*Java*) به صورت JIT-compiled خواهد بود.

به دست آوردن عملکرد خوب جاوا (*Java*) تلاش زیادی می‌طلبید. این تلاش اگر زبان (*Language*) با شکست مواجه می‌شد، اتفاق نمی‌افتاد. اما توسعه‌دهندگان (*Developers*) پتانسیل را دیدند و از قبل احساس بهره‌وری بیشتری نسبت به قبل داشتند. سرعت توسعه (*Speed of Development*) و تحویل (*Delivery*) اغلب می‌تواند مهمتر از سرعت برنامه (*Application Speed*) باشد.

سی‌شارپ (*C#*) در وضعیت کمی متفاوتی قرار داشت. زمان اجرای زبان مشترک (*Common Language Runtime - CLR*) از همان ابتدا بسیار کارآمد بود. پشتیبانی زبان (*Language Support*) برای تعامل آسان با کد (*Code*) بومی (*Native Code*) و برای کد (*Code*) ناامن (*Unsafe Code*) حساس به عملکرد (*Performance-Sensitive*) با اشاره‌گرها (*Pointers*) نیز کمک می‌کند. عملکرد سی‌شارپ (*C#*) با گذشت زمان به بهبود خود ادامه می‌دهد. (با لبخندی کنایه‌آمیز خاطرنشان می‌کنم که مایکروسافت (*Microsoft*) اکنون به طور گسترده کامپایل JIT لایه‌ای (*Tiered JIT Compilation*) را مانند کامپایلر (*Compiler*) JIT HotSpot جاوا (*Java*) معرفی می‌کند.)

اما بارهای کاری (*Workloads*) مختلف تقاضاهای عملکرد (*Performance Demands*) متفاوتی دارند. همانطور که در بخش 1.2 خواهید دید، سی‌شارپ (*C#*) اکنون در طیف شگفت‌انگیزی از پلتفرم‌ها (*Platforms*) از جمله بازی (*Gaming*) و میکروسرویس‌ها (*Microservices*) استفاده می‌شود که هر دو می‌توانند الزامات عملکردی (*Performance Requirements*) دشواری داشته باشند.

ناهمزمانی (*Asynchrony*) به رفع عملکرد (*Performance*) در برخی موقعیت‌ها کمک می‌کند، اما سی‌شارپ 7 (*C# 7*) صریح‌ترین نسخه حساس به عملکرد (*Performance-Sensitive Release*) است. ساختارهای (*Structs*) فقط خواندنی (*Read-Only*) و سطح وسیع‌تری برای ویژگی‌های ref به جلوگیری از کپی‌برداری اضافی (*Redundant Copying*) کمک می‌کنند. ویژگی Span<T> که در فریم‌ورک‌های (*Frameworks*) مدرن وجود دارد و توسط انواع ref-like struct پشتیبانی می‌شود، تخصیص غیرضروری (*Unnecessary Allocation*) و جمع‌آوری زباله (*Garbage Collection*) را کاهش می‌دهد. امید به وضوح این است که در صورت استفاده دقیق، این تکنیک‌ها (*Techniques*) نیازهای توسعه‌دهندگان (*Developers*) خاص را برآورده خواهند کرد.

من کمی احساس ناراحتی در مورد این ویژگی‌ها (*Features*) دارم، زیرا هنوز برای من پیچیده به نظر می‌رسند. نمی‌توانم در مورد یک متد (*Method*) با استفاده از یک پارامتر in به وضوح یک متد (*Method*) با پارامترهای (*Parameters*) مقداری (*Value Parameters*) معمولی استدلال کنم، و مطمئن هستم که مدتی طول می‌کشد تا با آنچه می‌توانم و نمی‌توانم با متغیرهای محلی ref و بازگشتی‌های ref انجام دهم، راحت شوم.

امید من این است که این ویژگی‌ها (*Features*) در حد اعتدال استفاده شوند. آنها کد (*Code*) را در موقعیت‌هایی که از آنها سود می‌برند ساده خواهند کرد، و بدون شک توسط توسعه‌دهندگانی (*Developers*) که آن کد (*Code*) را نگهداری می‌کنند، مورد استقبال قرار خواهند گرفت. من مشتاقانه منتظر آزمایش این ویژگی‌ها (*Features*) در پروژه‌های شخصی (*Personal Projects*) و راحت‌تر شدن با تعادل بین بهبود عملکرد (*Improved Performance*) و افزایش پیچیدگی کد (*Increased Code Complexity*) هستم.

</div>


<div dir="rtl" style="text-align: right;">

من نمی‌خواهم این نکته هشدار را بیش از حد بلند بیان کنم. من گمان می‌کنم تیم سی‌شارپ (*C#*) انتخاب درستی برای گنجاندن ویژگی‌های (*Features*) جدید انجام داده است، صرف نظر از اینکه من چقدر از آنها در کارم استفاده خواهم کرد. من فقط می‌خواهم اشاره کنم که نیازی نیست از یک ویژگی (*Feature*) فقط به این دلیل که وجود دارد، استفاده کنید. تصمیم خود را برای پذیرش پیچیدگی (*Complexity*) آگاهانه بگیرید. صحبت از پذیرش، سی‌شارپ 7 (*C# 7*) یک فرامک ویژگی (*Meta-Feature*) جدید را به ارمغان آورد: استفاده از شماره‌های نسخه فرعی (*Minor Version Numbers*) برای اولین بار از زمان سی‌شارپ 1 (*C# 1*).

## 1.1.6 تکامل با سرعت: استفاده از نسخه‌های فرعی (*Minor Versions*)

مجموعه شماره‌های نسخه (*Version Numbers*) برای سی‌شارپ (*C#*) عجیب است، و این واقعیت که بسیاری از توسعه‌دهندگان (*Developers*) به طور قابل درک بین فریم‌ورک (*Framework*) و زبان (*Language*) سردرگم می‌شوند، آن را پیچیده‌تر می‌کند. (به عنوان مثال، سی‌شارپ 3.5 وجود ندارد. نسخه 3.0 .NET Framework با سی‌شارپ 2 (*C# 2*) عرضه شد، و 3.5 .NET با سی‌شارپ 3 (*C# 3*) عرضه شد.) سی‌شارپ 1 (*C# 1*) دو نسخه داشت: سی‌شارپ 1.0 و سی‌شارپ 1.2. بین سی‌شارپ 2 (*C# 2*) و سی‌شارپ 6 (*C# 6*) شامل، فقط نسخه‌های اصلی (*Major Versions*) وجود داشتند که معمولاً توسط یک نسخه جدید از ویژوال استودیو (*Visual Studio*) پشتیبانی می‌شدند.

سی‌شارپ 7 (*C# 7*) این روند را شکست: نسخه‌های سی‌شارپ 7.0، سی‌شارپ 7.1، سی‌شارپ 7.2 و سی‌شارپ 7.3 وجود داشتند که همگی در ویژوال استودیو 2017 (*Visual Studio 2017*) در دسترس بودند. من بسیار محتمل می‌دانم که این الگو در سی‌شارپ 8 (*C# 8*) نیز ادامه یابد. هدف این است که به ویژگی‌های (*Features*) جدید اجازه داده شود تا با بازخورد کاربر (*User Feedback*) به سرعت تکامل یابند. اکثریت ویژگی‌های (*Features*) سی‌شارپ 7.1-7.3 تنظیمات (*Tweaks*) یا گسترش‌هایی (*Extensions*) بر ویژگی‌های (*Features*) معرفی شده در سی‌شارپ 7.0 بوده‌اند.

نوسانات (*Volatility*) در ویژگی‌های (*Features*) زبان (*Language*) می‌تواند گیج‌کننده باشد، به ویژه در سازمان‌های بزرگ. ممکن است نیاز به تغییر یا ارتقاء زیرساخت (*Infrastructure*) زیادی باشد تا اطمینان حاصل شود که نسخه (*Version*) جدید زبان (*Language*) به طور کامل پشتیبانی می‌شود. بسیاری از توسعه‌دهندگان (*Developers*) ممکن است ویژگی‌های (*Features*) جدید را با سرعت‌های متفاوتی یاد بگیرند و به کار گیرند. حداقل، ممکن است کمی ناخوشایند باشد که زبان (*Language*) بیشتر از آنچه به آن عادت کرده‌اید تغییر کند.

به همین دلیل، کامپایلر (*Compiler*) سی‌شارپ (*C#*) به طور پیش‌فرض از اولین نسخه فرعی (*Minor Version*) آخرین نسخه اصلی (*Major Version*) که از آن پشتیبانی می‌کند، استفاده می‌کند. اگر از یک کامپایلر (*Compiler*) سی‌شارپ 7 (*C# 7*) استفاده کنید و هیچ نسخه زبانی (*Language Version*) را مشخص نکنید، به طور پیش‌فرض شما را به سی‌شارپ 7.0 محدود می‌کند. اگر می‌خواهید از یک نسخه فرعی (*Minor Version*) بعدی استفاده کنید، باید آن را در فایل پروژه (*Project File*) خود مشخص کنید و به ویژگی‌های (*Features*) جدید بپیوندید. می‌توانید این کار را به دو روش انجام دهید، اگرچه آنها تأثیر یکسانی دارند. می‌توانید فایل پروژه (*Project File*) خود را مستقیماً ویرایش کنید تا یک عنصر <LangVersion> در یک <PropertyGroup> اضافه کنید، مانند این:

</div>

<div dir="ltr" style="text-align: left;">

```xml
<PropertyGroup>
    ...
    <LangVersion>latest</LangVersion>
</PropertyGroup>
```

</div>

![Figure1.1](https://github.com/alirezark70/CSharpInDepth/blob/master/assets/figure1.1.jpg)

<div dir="rtl" style="text-align: right;">

اگر از ویرایش مستقیم فایل‌های پروژه (*Project Files*) خوشتان نمی‌آید، می‌توانید در ویژوال استودیو (*Visual Studio*) به خصوصیات پروژه (*Project Properties*) بروید، تب Build را انتخاب کنید و سپس روی دکمه Advanced در پایین سمت راست کلیک کنید. کادر گفتگوی Advanced Build Settings که در شکل 1.1 نشان داده شده است، باز می‌شود تا به شما امکان دهد نسخه زبان (*Language Version*) مورد نظر خود و سایر گزینه‌ها را انتخاب کنید.

این گزینه در کادر گفتگو جدید نیست، اما اکنون بیشتر از نسخه‌های قبلی احتمالاً می‌خواهید از آن استفاده کنید. مقادیر قابل انتخاب به شرح زیر است:

<div dir="ltr" style="text-align: left;">

- default: اولین انتشار آخرین نسخه اصلی (*Major Version*)
- latest: آخرین نسخه (*Version*)
- A specific version number: به عنوان مثال، 7.0 یا 7.3

</div>

این تغییر نسخه کامپایلری (*Compiler Version*) که اجرا می‌کنید نیست؛ بلکه مجموعه ویژگی‌های زبان (*Language Features*) در دسترس شما را تغییر می‌دهد. اگر سعی کنید از چیزی استفاده کنید که در نسخه مورد نظر شما موجود نیست، پیام خطای کامپایلر (*Compiler Error Message*) معمولاً توضیح می‌دهد که کدام نسخه برای آن ویژگی (*Feature*) لازم است. اگر سعی کنید از یک ویژگی زبان (*Language Feature*) استفاده کنید که برای کامپایلر (*Compiler*) کاملاً ناشناخته است (به عنوان مثال، استفاده از ویژگی‌های سی‌شارپ 7 با یک کامپایلر (*Compiler*) سی‌شارپ 6)، پیام خطا معمولاً کمتر واضح است.

سی‌شارپ (*C#*) به عنوان یک زبان (*Language*) از زمان اولین انتشار خود راه طولانی را طی کرده است. پلتفرمی (*Platform*) که روی آن اجرا می‌شود چطور؟

## 1.2 یک پلتفرم (*Platform*) در حال تکامل

چند سال اخیر برای توسعه‌دهندگان (*Developers*) دات‌نت (.NET) هیجان‌انگیز بوده است. مقدار مشخصی از ناامیدی نیز وجود دارد، زیرا هم مایکروسافت (*Microsoft*) و هم جامعه (*Community*) دات‌نت (.NET) با پیامدهای مدل توسعه بازتر (*More Open Development Model*) کنار می‌آیند. اما نتیجه کلی کار سخت بسیاری از افراد قابل توجه است.

برای سال‌های متمادی، اجرای کد (*Code*) سی‌شارپ (*C#*) تقریباً همیشه به معنای اجرا بر روی ویندوز (*Windows*) بود. معمولاً به معنای یک برنامه سمت کلاینت (*Client-Side App*) نوشته شده در Windows Forms یا Windows Presentation Foundation (WPF) یا یک برنامه سمت سرور (*Server-Side App*) نوشته شده با ASP.NET و احتمالاً در حال اجرا پشت Internet Information Server (IIS) بود. گزینه‌های دیگر برای مدت طولانی در دسترس بوده‌اند، و پروژه Mono به ویژه سابقه غنی‌ای دارد، اما جریان اصلی توسعه (*Development*) دات‌نت (.NET) هنوز بر روی ویندوز (*Windows*) بود.

همانطور که این را در ژوئن 2018 می‌نویسم، دنیای دات‌نت (.NET) بسیار متفاوت است. برجسته‌ترین توسعه .NET Core است، یک زمان اجرا (*Runtime*) و فریم‌ورک (*Framework*) که قابل حمل (*Portable*) و متن باز (*Open Source*) است، به طور کامل توسط مایکروسافت (*Microsoft*) در چندین سیستم عامل (*Operating Systems*) پشتیبانی می‌شود و ابزارهای توسعه (*Development Tooling*) ساده‌ای دارد. تنها چند سال پیش، این غیرقابل تصور بود. به این یک IDE قابل حمل (*Portable*) و متن باز (*Open Source*) در قالب Visual Studio Code را اضافه کنید، و یک اکوسیستم (*Ecosystem*) پر رونق دات‌نت (.NET) با توسعه‌دهندگانی (*Developers*) خواهید داشت که بر روی انواع پلتفرم‌های (*Platforms*) محلی کار می‌کنند و سپس بر روی انواع پلتفرم‌های (*Platforms*) سرور (*Server*) مستقر می‌شوند.

</div>


<div dir="rtl" style="text-align: right;">

اشتباه است که بیش از حد بر روی .NET Core تمرکز کنیم و بسیاری از روش‌های دیگر اجرای سی‌شارپ (*C#*) این روزها را نادیده بگیریم. Xamarin یک تجربه موبایل (*Mobile Experience*) چند پلتفرمی (*Multiplatform*) غنی را فراهم می‌کند. فریم‌ورک (*Framework*) GUI آن (Xamarin Forms) به توسعه‌دهندگان (*Developers*) امکان می‌دهد رابط‌های کاربری (*User Interfaces*) را ایجاد کنند که در دستگاه‌های (*Devices*) مختلف تا حدودی یکنواخت هستند، جایی که مناسب است، اما می‌توانند از پلتفرم (*Platform*) زیربنایی نیز بهره ببرند.

Unity یکی از محبوب‌ترین پلتفرم‌های (*Platforms*) توسعه بازی (*Game-Development*) در جهان است. با یک زمان اجرا (*Runtime*) Mono سفارشی و کامپایل پیش از زمان (*Ahead-of-Time Compilation*)، می‌تواند چالش‌هایی را برای توسعه‌دهندگان (*Developers*) سی‌شارپ (*C#*) که به محیط‌های (*Environments*) زمان اجرای (*Runtime*) سنتی‌تر عادت دارند، ایجاد کند. اما برای بسیاری از توسعه‌دهندگان (*Developers*)، این اولین یا شاید تنها تجربه آنها با این زبان (*Language*) است.

این پلتفرم‌های (*Platforms*) پرکاربرد، به دور از تنها پلتفرم‌هایی (*Platforms*) هستند که سی‌شارپ (*C#*) را می‌سازند. من اخیراً با Try .NET و Blazor برای اشکال بسیار متفاوتی از تعامل مرورگر (*Browser*)/سی‌شارپ (*C#*) کار می‌کردم.

Try .NET به کاربران امکان می‌دهد کد (*Code*) را در یک مرورگر (*Browser*) با تکمیل خودکار (*Autocompletion*) بنویسند و سپس آن کد (*Code*) را بسازند و اجرا کنند. این برای آزمایش سی‌شارپ (*C#*) با حداقل مانع ورود عالی است.

Blazor یک پلتفرم (*Platform*) برای اجرای مستقیم صفحات Razor در یک مرورگر (*Browser*) است. اینها صفحاتی نیستند که توسط یک سرور (*Server*) رندر (*Rendered*) شده و سپس در مرورگر (*Browser*) نمایش داده شوند؛ کد (*Code*) رابط کاربری (*User-Interface Code*) در داخل مرورگر (*Browser*) با استفاده از نسخه‌ای از زمان اجرا (*Runtime*) Mono که به WebAssembly تبدیل شده است، اجرا می‌شود. ایده یک زمان اجرا (*Runtime*) کامل که زبان میانی (*Intermediate Language - IL*) را از طریق موتور جاوا اسکریپت (*JavaScript Engine*) در یک مرورگر (*Browser*) اجرا می‌کند، نه تنها در رایانه‌های کامل بلکه در تلفن‌های همراه، تنها چند سال پیش برای من پوچ به نظر می‌رسید. خوشحالم که توسعه‌دهندگان (*Developers*) دیگر تخیل بیشتری دارند. بسیاری از نوآوری‌ها در این فضا تنها با یک جامعه (*Community*) همکار و بازتر از همیشه امکان‌پذیر شده است.

## 1.3 یک جامعه (*Community*) در حال تکامل

من از زمان سی‌شارپ 1.0 در جامعه (*Community*) سی‌شارپ (*C#*) فعالیت داشته‌ام، و هرگز آن را به این اندازه پر جنب و جوش که امروز هست، ندیده‌ام. وقتی من شروع به استفاده از سی‌شارپ (*C#*) کردم، آن را به عنوان یک زبان برنامه‌نویسی "سازمانی" (*Enterprise*) می‌دیدند، و احساس سرگرمی و کاوش نسبتاً کمی وجود داشت. با این پیشینه، اکوسیستم (*Ecosystem*) متن باز (*Open Source*) سی‌شارپ (*C#*) در مقایسه با سایر زبان‌ها، از جمله جاوا (*Java*) که آن نیز یک زبان (*Language*) سازمانی (*Enterprise*) محسوب می‌شد، نسبتاً آهسته رشد کرد. در حدود زمان سی‌شارپ 3، جامعه (*Community*) alt.NET فراتر از جریان اصلی توسعه (*Development*) دات‌نت (.NET) را بررسی می‌کرد، و این در برخی جهات به عنوان مخالفت با مایکروسافت (*Microsoft*) تلقی می‌شد.

در سال 2010، مدیر بسته NuGet (ابتدا NuPack) راه‌اندازی شد، که تولید و مصرف کتابخانه‌های کلاس (*Class Libraries*) را، چه تجاری و چه متن باز (*Open Source*)، بسیار آسان‌تر کرد. حتی با وجود اینکه مانع دانلود یک فایل زیپ (*Zip File*)، کپی کردن یک DLL در مکانی مناسب، و سپس اضافه کردن یک مرجع (*Reference*) به آن، چندان مهم به نظر نمی‌رسد، هر نقطه اصطکاک می‌تواند توسعه‌دهندگان (*Developers*) را منصرف کند.

> **نکته**: مدیران بسته (*Package Managers*) دیگری به غیر از NuGet حتی زودتر توسعه یافتند، و پروژه OpenWrap که توسط Sebastien Lambla توسعه یافت، به ویژه تأثیرگذار بود.

به سرعت به سال 2014 می‌رویم، مایکروسافت (*Microsoft*) اعلام کرد که پلتفرم کامپایلر (*Compiler Platform*) Roslyn آن قرار است تحت چتر بنیاد جدید دات‌نت (.NET Foundation) متن باز (*Open Source*) شود. سپس .NET Core با اسم رمز اولیه Project K اعلام شد؛ DNX بعداً آمد، و به دنبال آن ابزارهای .NET Core که اکنون منتشر شده و پایدار هستند. سپس ASP.NET Core آمد. و Entity Framework Core. و Visual Studio Code. لیست محصولاتی که واقعاً در گیت‌هاب (*GitHub*) زندگی می‌کنند و نفس می‌کشند، ادامه دارد.

فناوری (*Technology*) مهم بوده است، اما پذیرش جدید متن باز (*Open Source*) توسط مایکروسافت (*Microsoft*) برای یک جامعه (*Community*) سالم به همان اندازه حیاتی بوده است. بسته‌های متن باز (*Open Source*) شخص ثالث (*Third-Party*) شکوفا شده‌اند، از جمله کاربردهای نوآورانه برای Roslyn و ادغام‌ها در ابزارهای .NET Core که به درستی حس می‌شوند.

هیچ یک از اینها در خلاء اتفاق نیفتاده است. رشد رایانش ابری (*Cloud Computing*) باعث می‌شود .NET Core برای اکوسیستم (*Ecosystem*) دات‌نت (.NET) حتی مهم‌تر از آنچه در غیر این صورت بود، باشد؛ پشتیبانی از لینوکس (*Linux*) اختیاری نیست. اما از آنجا که .NET Core در دسترس است، اکنون هیچ چیز خاصی در مورد بسته‌بندی یک سرویس ASP.NET Core در یک ایمیج داکر (*Docker Image*)، استقرار آن با Kubernetes، و استفاده از آن به عنوان تنها بخشی از یک برنامه بزرگتر که می‌تواند شامل زبان‌های (*Languages*) زیادی باشد، وجود ندارد. گرده‌افشانی متقابل ایده‌های خوب بین بسیاری از جوامع همیشه وجود داشته است، اما اکنون قوی‌تر از همیشه است.

شما می‌توانید سی‌شارپ (*C#*) را در یک مرورگر (*Browser*) یاد بگیرید. می‌توانید سی‌شارپ (*C#*) را در هر جایی اجرا کنید. می‌توانید در مورد سی‌شارپ (*C#*) در Stack Overflow و بی‌شمار سایت‌های دیگر سوال بپرسید. می‌توانید در بحث در مورد آینده زبان (*Language*) در مخزن گیت‌هاب (*GitHub Repository*) تیم سی‌شارپ (*C#*) شرکت کنید. کامل نیست؛ ما هنوز کار جمعی برای انجام دادن داریم تا جامعه (*Community*) سی‌شارپ (*C#*) را تا حد امکان برای همه استقبال‌کننده کنیم، اما از قبل در جایگاه عالی قرار داریم.

</div>


<div dir="rtl" style="text-align: right;">

## 1.4 یک کتاب در حال تکامل

شما در حال خواندن ویرایش چهارم C# in Depth هستید. اگرچه این کتاب با همان سرعت زبان (*Language*)، پلتفرم (*Platform*) یا جامعه (*Community*) تکامل نیافته است، اما تغییر کرده است. این بخش به شما کمک می‌کند تا بفهمید چه چیزی در این کتاب پوشش داده شده است.

### 1.4.1 پوشش سطح مختلط (*Mixed-Level Coverage*)

اولین ویرایش C# in Depth در آوریل 2008 منتشر شد، که به طور اتفاقی همزمان با پیوستن من به گوگل (*Google*) بود. در آن زمان، می‌دانستم که بسیاری از توسعه‌دهندگان (*Developers*) سی‌شارپ 1 را به خوبی می‌شناختند، اما سی‌شارپ 2 و سی‌شارپ 3 را در حین کار بدون درک کامل از نحوه قرار گرفتن قطعات در کنار هم، فرا می‌گرفتند. هدف من رفع این شکاف با غوطه ور شدن در زبان (*Language*) با عمقی بود که به خوانندگان کمک می‌کرد نه تنها بفهمند هر ویژگی (*Feature*) چه کاری انجام می‌دهد، بلکه بفهمند چرا به این صورت طراحی شده است.

با گذشت زمان، نیازهای توسعه‌دهندگان (*Developers*) تغییر می‌کند. به نظر من جامعه (*Community*) درک عمیق‌تری از زبان (*Language*) را تقریباً از طریق اسمز (*Osmosis*) جذب کرده است، حداقل برای نسخه‌های (*Versions*) اولیه. دستیابی به درک عمیق‌تر از زبان (*Language*) یک تجربه جهانی نخواهد بود، اما برای ویرایش چهارم، می‌خواستم تأکید بر نسخه‌های (*Versions*) جدیدتر باشد. هنوز فکر می‌کنم درک تکامل (*Evolution*) زبان (*Language*) نسخه به نسخه مفید است، اما نیاز کمتری به بررسی جزئیات هر ویژگی (*Feature*) در سی‌شارپ 2-4 وجود دارد.

> **نکته**: نگاه کردن به زبان (*Language*) یک نسخه در یک زمان، بهترین راه برای یادگیری زبان (*Language*) از ابتدا نیست، اما اگر می‌خواهید آن را عمیقاً درک کنید، مفید است. من از همین ساختار برای نوشتن کتابی برای مبتدیان سی‌شارپ (*C# Beginners*) استفاده نمی‌کنم.

من همچنین به کتاب‌های ضخیم علاقه ندارم. نمی‌خواهم C# in Depth ترسناک، سخت برای نگه داشتن یا سخت برای نوشتن باشد. نگهداری 400 صفحه پوشش برای سی‌شارپ 2-4 به درستی حس نمی‌شد. به همین دلیل، پوشش خود را از آن نسخه‌ها فشرده کرده‌ام. هر ویژگی (*Feature*) ذکر شده است، و در جایی که احساس می‌کنم مناسب است، به جزئیات می‌پردازم، اما عمق کمتری نسبت به ویرایش سوم وجود دارد. از پوشش در ویرایش چهارم به عنوان مروری بر موضوعاتی که از قبل می‌دانید و برای کمک به شما در تعیین موضوعاتی که می‌خواهید بیشتر در مورد آنها در ویرایش سوم بخوانید، استفاده کنید. می‌توانید پیوندی برای دسترسی به یک نسخه الکترونیکی (*Electronic Copy*) از ویرایش سوم را در www.manning.com/books/c-sharp-in-depth-fourth-edition پیدا کنید. نسخه‌های 5-7 زبان (*Language*) در این ویرایش با جزئیات بیشتری پوشش داده شده‌اند. ناهمزمانی (*Asynchrony*) هنوز یک موضوع دشوار برای درک است، و ویرایش سوم بدیهی است که سی‌شارپ 6 یا 7 را اصلاً پوشش نمی‌دهد.

نوشتن، مانند مهندسی نرم‌افزار (*Software Engineering*)، اغلب یک عمل تعادلی است. امیدوارم تعادلی که بین جزئیات و ایجاز ایجاد کرده‌ام، برای شما کارساز باشد.

> **نکته**: اگر یک نسخه فیزیکی (*Physical Copy*) از این کتاب دارید، قویاً شما را تشویق می‌کنم که در آن یادداشت‌برداری کنید. نقاطی را که مخالف هستید یا بخش‌هایی که به ویژه مفید هستند، یادداشت کنید. انجام این کار محتوا را در حافظه شما تقویت می‌کند و یادداشت‌ها بعداً به عنوان یادآوری عمل خواهند کرد.

</div>
