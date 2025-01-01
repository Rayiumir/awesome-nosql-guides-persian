# راهنمای عالی NoSQL [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> فهرست انتخاب شده از منابع و پیوندها در مورد *استفاده از* پایگاه داده های NoSQL و مواردی که هنگام تصمیم گیری برای استفاده از آن باید به دنبال آنها باشید.

تعریف پایه ای از پایگاه داده NoSQL را می توان در ویکی پدیا به صورت زیر یافت:

> به دلیل محدودیت‌های کلاسیک SQL و مدرن شدن دنیای اینترنت و اطلاعات، کاربران و مدیران بخش داده‌ها به ارائه ایده‌های جدید با تمرکز بر تفکر «یک قالب مطابق با همه» یا “One size fits all” پرداخته‌اند که در آن قید و بندهای سیستم قبلی تا حد امکان موجود نباشد.
در مدل NoSQL بنا به شیوه‌های مختلف، دیگر نیاز به طراحی و زمان طولانی برای طراحی پایگاه داده‌ها نمی‌باشد. در برخی از سرویس‌های NoSQL الگوریتم‌های هوشمندی هم به کار رفته‌است که دیگر نیازی به طراحی پایگاه داده نمی‌باشد و بر اساس ورودی‌های برنامه‌نویس و کاربر و تعیین نوع نیازمندی‌ها و پلتفرم و شرایط محیطی دیگر، نوع ذخیره‌سازی و مدیریت داده‌ها پیاده‌سازی می‌شود. 

برای پایگاه داده های NoSQL واقعی، به سایت های
[اینجا](https://github.com/sindresorhus/awesome#databases),
[اینجا](https://hostingdata.co.uk/nosql-database/),
[اینجا](https://db-engines.com/en/ranking),
[اینجا](https://dbdb.io/),
[اینجا](https://github.com/igorbarinov/awesome-data-engineering#databases), یا
[اینجا](https://github.com/kahun/awesome-sysadmin#nosql). همچنین، نباید با سیستم مدیریت پایگاه داده رابطه ای اشتباه شود، [NoSQL](http://www.strozzi.it/cgi-bin/CSA/tw7/I/en_US/nosql/Home%20Page).


## فهرست محتوا

- [مروری بر NoSQL](#overview-of-nosql)
- [ساختار داده ها و مدل سازی](#data-structures-and-modeling)
- [Trade-Offs در قضیه CAP/Brewer](#trade-offs-in-capbrewers-theorem)
- [اطلاعات با منبع جمعی](#crowd-sourced-information)
- [Graph Databases](#graph-databases)
- [Criticisms and Debates](#criticisms-and-debates)
- [Miscellaneous](#miscellaneous)


## Overview of NoSQL 

- [Introduction To NoSQL - Martin Fowler (54:52)](https://www.youtube.com/watch?v=qI_g07C_Q5I)

<p align="right"> سخنرانی ارائه شده در GOTO 2012 به عنوان مقدمه ای عالی برای پایگاه های داده NoSQL، انواع پایگاه های داده NoSQL، تاریخچه، مزایا و معایب آنها، و نحوه و زمان استفاده them.
</p>

- [NoSQL Distilled](https://martinfowler.com/books/nosql.html)

<p align="right">کتاب بسیار قابل هضم و مقرون به صرفه ای است که پایگاه های داده مختلف NoSQL را توصیف می کند و به شما کمک می کند تا تصمیم بگیرید که آیا استفاده از پایگاه داده NoSQL برای پروژه شما مناسب است یا خیر.
</p>

- [Seven Databases in Song (1:43)](https://www.youtube.com/watch?v=jyx8iP5tfCI)

<p align="right">ویدئو سرگرم کننده از سال 2012 در مورد هفت پایگاه داده (شش NoSQL) با نمای کلی بسیار فشرده از نحوه کار هر کدام.
</p>

- [NoSQL Databases: a Survey and Decision Guidance (2016)](https://medium.baqend.com/nosql-databases-a-survey-and-decision-guidance-ea7823a822d)

<p align="right">"این جعبه ابزار NoSQL به ما اجازه می دهد تا یک درخت تصمیم ساده استخراج کنیم تا به متخصصان و محققان کمک کند تا نامزدهای احتمالی سیستم را بر اساس الزامات برنامه مرکزی فیلتر کنند."
</p>

- [Data Management in the Cloud: Limitations and Opportunities (PDF)](http://www.cs.umd.edu/~abadi/papers/abadi-cloud-ieee09.pdf)

<p align="right">Abadi (2009) محدودیت ها و فرصت های مدیریت داده و تجزیه و تحلیل داده ها را در فضای ابری مورد بحث قرار می دهد.
</p>

- [10 NoSQL Misconceptions](https://web.archive.org/web/20210701080816/https://www.dummies.com/programming/big-data/10-nosql-misconceptions/)

<p align="right">برخی تصورات غلط در مورد پایگاه های داده NoSQL در رابطه با موضوعاتی مانند چیستی آنها، انطباق با ACID و امنیت.
</p>

- [10 Reasons Developers Love NoSQL](https://web.archive.org/web/20210701080841/https://www.dummies.com/programming/big-data/10-reasons-developers-love-nosql/)

<p align="right"> لیستی از ده استدلال برای اینکه چرا توسعه دهندگان دوست دارند از پایگاه داده NoSQL استفاده کنند.
</p>

- [Distribution, Data, Deployment: Software Architecture Convergence in Big Data Systems (PDF)](https://resources.sei.cmu.edu/library/asset-view.cfm?assetID=90909)

<p align="right">گورتون و کلاین (2014) مقاله ای برای بحث در مورد نگرانی های مهندسی نرم افزار هنگام برخورد با سیستم های کلان داده از نظر توزیع، داده و استقرار. دسترسی از اینجا.
  [اینجا](https://doi.org/10.1109/MS.2014.51)
</p>

- [Use cases for NoSQL (2017)](https://stackoverflow.com/questions/2875432/use-cases-for-nosql)

<p align="right">حث در مورد Stack Overflow در مورد بهترین موارد استفاده برای استفاده از پایگاه‌های داده NoSQL بر روی پایگاه‌های داده سنتی SQL.
</p>

- [Five Common Data Stores and When to Use Them (2019)](https://shopify.engineering/five-common-data-stores-usage)

<p align="right">مقاله پنج ذخیره‌گاه داده رایج (پایگاه داده رابطه‌ای، غیرمرتبط (“ NoSQL") پایگاه داده، ذخیره کلید-مقدار، موتور جستجوی متن کامل، صف پیام) و ویژگی های آنها.
</p>

- [NoSQL Databases (PDF)](https://web.archive.org/web/20190927222738/https://www.christof-strauch.de/nosqldbs.pdf)

<p align="right">یک صفحه 149 صفحه‌ای که انگیزه‌ها و دلایل منطقی برای پایگاه های داده NoSQL و مفاهیم، ​​تکنیک ها و الگوهای رایج در میان این پایگاه های داده. آخرین به روز رسانی در حدود 2011.
</p>

- [NoSQL Data Architecture & Data Governance: Everything You Need to Know (2018)](https://www.dataversity.net/nosql-data-architecture-data-governance-everything-need-know/)

<p align="right">مروری بر موارد مختلف معماری پایگاه داده NoSQL با نمودار.
</p>

- [NoSQL vs SQL: Demystifying NoSQL Databases (2019)](https://build5nines.com/nosql-vs-sql-demystifying-nosql-databases/)

<p align="right">نمای کلی و نمونه‌هایی از انواع طرح‌های پایگاه داده NoSQL، در حالی که قضیه CAP را پوشش می‌دهد.
</p>

- [Comparing Database Types: How Database Types Evolved to Meet Different Needs](https://www.prisma.io/dataguide/intro/comparing-database-types)

<p align="right">مروری خوب بر پایگاه های داده به طور کلی و نحوه تفاوت انواع پایگاه داده NoSQL و می تواند مفید باشد.
</p>

- [The NoSQL Ecosystem](https://www.aosabook.org/en/nosql.html)

<p align="right">فصلی که توسط آدام مارکوس از کتاب "معماری برنامه های کاربردی منبع باز" نوشته شده است، این فصل بیشتر به سمت معماران سیستم مورد نیاز است. برای یادگیری درک عمیق تر از نحوه ساخت این سیستم ها.
</p>

- [What is NoSQL - Amazon AWS](https://aws.amazon.com/nosql/)
<p align="right">مروری عالی در سطح بالا از پایگاه‌های داده NoSQL و نحوه مقایسه آنها با فناوری‌ها و اصطلاحات پایگاه داده SQL. به عنوان صفحه فرود برای خدمات AWS آمازون برای گزینه های NoSQL از ارزش کلید (Amazon DynamoDB)، سند (Amazon DocumentDB)، نمودار (Amazon Neptune)، حافظه داخلی (Amazon ElastiCache)، و موتور جستجو (Amazon Elasticsearch) پایگاه داده عمل می کند.
</p>

- [NoSQL vs. SQL: Important Differences & Which One Is Best for Your Project (2021) - Upwork](https://www.upwork.com/resources/nosql-vs-sql)

<p align="right"> توضیح مقایسه پایگاه‌های داده SQL و NoSQL، همراه با ارائه برخی توصیه ها در مورد اینکه چه راه حل پایگاه داده برای مورد استفاده شما مناسب است.
</p>

- [NoSQL Database Tutorial – Full Course for Beginners (2:54:52)](https://www.youtube.com/watch?v=xh4gy1lbL2k)

<p align="right"> مدرس Ania Kubow چهار نوع پایگاه داده NoSQL را بررسی می کند و دو دست را ارائه می دهد. در پروژه ها برای آزمایش با آنچه مورد بررسی قرار گرفت.
</p>

## Data Structures and Modeling

- [Structure Your Database](https://firebase.google.com/docs/database/android/structure-data) 

<p align="right">اگر پایگاه داده شما از JSON استفاده می کند، بهترین روش ها (از سال 2018) برای ساختار داده های شما.</p>

- [NoSQL Data Modeling Techniques (2012)](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)
- 
<p align="right">این مقاله مقایسه کوتاهی از خانواده‌های سیستم NoSQL از دیدگاه مدل‌سازی داده ارائه می‌کند و چندین تکنیک مدل‌سازی رایج را هضم می‌کند.</p> 

- [Data Models For MongoDB](https://www.mongodb.com/docs/manual/data-modeling/) 

<p align="right">مدل‌سازی داده‌ها به MongoDB کمک می‌کند، از اعتبارسنجی schema و الگوهای نمونه. با این حال، مفاهیم ممکن است به سایر پایگاه‌های داده NoSQL منتقل شوند.</p>

- [Data Models Will Be Beautiful Again (2016)](https://tdwi.org/articles/2016/11/22/data-models-will-be-beautiful-again.aspx) 
 
<p align="right">Essay استدلال می‌کند که با وجود پایگاه‌های داده بدون schema، مدل‌سازی متفکرانه پایگاه داده برای به دست آوردن دانش و بینش با استفاده از الگوریتم‌ها مهم است.</p>

- [Unified Data Modeling for Relational and NoSQL Databases](https://www.infoq.com/articles/unified-data-modeling-for-relational-and-nosql-databases/)

<p align="right">راه حلی برای مدیریت هر دو پایگاه داده NoSQL و رابطه ای با استفاده از تکنیک Unified Data Modeling.</p>

- [Unifying Relational, Document, Graph, and Temporal Data Models](https://fauna.com/blog/unifying-relational-document-graph-and-temporal-data-models)
 
<p align="right">الگوهایی برای کوئری ها در چندین پارادایم در یک پایگاه داده.</p>

- [How To Design Schema For Your NoSQL Database?](https://www.dataversity.net/how-to-design-schema-for-your-nosql-database/#) 

<p align="right">علی‌رغم باور عمومی مبنی بر اینکه NoSQL بدون schema است، این مقاله به تشریح این موضوع می‌پردازد که چگونه پایگاه‌های داده NoSQL از «طراحی مبتنی بر کوئری» پیروی می‌کنند و ملاحظات مربوط به این انعطاف‌پذیری در schema</p>


- [Best Practices for NoSQL Database Design (2012)](https://softwareengineering.stackexchange.com/q/158790/)

<p align="right">چند پاسخ و پیوند برای طراحی پایگاه داده NoSQL.</p>


## Trade-Offs in CAP/Brewer's Theorem

- [Visual Guide To NoSQL Systems (2010)](http://blog.nahurst.com/visual-guide-to-nosql-systems)

  <p align="right">نمایش بصری trade-offs در قضیه CAP در میان پایگاه‌های داده مختلف NoSQL.</p>

- [How to Choose The Right NoSQL Database For Your Application? (2018)](https://www.dataversity.net/choose-right-nosql-database-application/)

<p align="right">قضیه CAP را بررسی می کند و پایگاه های داده رایج NoSQL را به دسته های CAP ترسیم می کند تا به انتخاب یکی کمک کند.</p>

## Crowd-Sourced Information

- [/r/nosql](https://www.reddit.com/r/nosql/) 

<p align="right">صفحه Reddit در NoSQL در مورد سوالات عمومی و بحث هایی که ممکن است افراد در مورد پایگاه های داده NoSQL داشته باشند.</p>

- [[nosql] Tag On Stack Overflow](https://stackoverflow.com/tags/nosql/info)

<p align="right">روی Overflow تگ کنید</p>

- [Ask HN: Learning NoSQL, Papers and Books (2017)](https://news.ycombinator.com/item?id=15427932)

<p align="right">"به نظر شما، کدام مقاله ها و کتاب ها برای درک واقعی موضوع NoSQL اجباری هستند؟"</p>

- [Difference Between Scaling Horizontally And Vertically For Databases](https://stackoverflow.com/q/11707879/6873133)

<p align="right">اصطلاحات رایجی که در دنیای پایگاه داده درباره آنها صحبت می شود و در اینجا پاسخ هایی از سوی کاربران وجود دارد.</p>

- [NoSQL - Wikipedia](https://en.wikipedia.org/wiki/NoSQL)

<p align="right">پایگاه داده NoSQL در ویکی پدیا</p>

## Graph Databases

- [Graph Databases Use Cases](https://neo4j.com/use-cases/) - Although documents geared towards Neo4j, concepts are applicable to all graph databases.
- [How The ICIJ Used Neo4j To Unravel The Panama Papers - Mar Cabra (32:02)](https://www.youtube.com/watch?v=S20XMQyvANY) - Learn how graph databases were key to explore who were the main names connected to companies in tax havens, including 140 politicians in more than 50 countries.
- [Graph Databases For Beginners: The Basics Of Data Modeling](https://neo4j.com/blog/data-modeling-basics/) - Discusses the basics of modeling your data and which approach you should take.
- [Graph Data Modeling Guidelines](https://neo4j.com/developer/guide-data-modeling/) - Directly related to Neo4j, but possibly applicable to any graph database.
- [Graph Data Modeling Visualize Structure and Meaning](http://www.graphdatamodeling.com) - Brief introduction to graph data modeling and is an introduction to the book "Graph Data Modeling for NoSQL and SQL" by Thomas Frisendal.


## Criticisms and Debates

- [Addressing the NoSQL Criticism (2011)](https://www.bradley-holt.com/2011/07/addressing-the-nosql-criticism/) - Argues against nine criticisms to NoSQL databases as they apply to CouchDB, but may apply to others as well.
- [Thank You For Your Help NoSQL, But We Got It From Here (2020)](https://web.archive.org/web/20200913032621/https://www.memsql.com/blog/why-nosql-databases-wrong-tool-for-modern-application/) - Argument that NoSQL databases have pushed the evolution of databases given the problem of scaling, but now NewSQL has addressed those concerns (from the perspective of MemSQL).
- [The Five Stages Of NoSQL (2016)](https://sookocheff.com/post/opinion/the-five-stages-of-nosql/) - Stages of going through picking and using a NoSQL database mirroring the five stages of grief.
- [The Biggest Challenges Of Moving To NoSQL (2017)](https://dzone.com/articles/the-biggest-challenges-of-moving-to-nosql) - Speed and scalability and developer joy have been the gains found from enduring through challenges of moving to NoSQL.


## Miscellaneous

- [What As A NoSQL Database? Learn By Writing One In Python](https://web.archive.org/web/20201109032031/https://jeffknupp.com/blog/2014/09/01/what-is-a-nosql-database-learn-by-writing-one-in-python/) - Excellent tutorial in learning NoSQL vs RDBMS through building a toy database using Python.
- [Dynamo Vs Cassandra : Systems Design Of NoSQL Databases](https://sujithjay.com/data-systems/dynamo-cassandra/) - Blog post comparing and constrating system designs of two well known NoSQL databases.
- [Why You Should Build Your Wwn NoSQL Database](https://medium.com/@marceloboeira/why-you-should-build-your-own-nosql-database-9bbba42039f5) - Brief overview of NoSQL databases and the spectrum of schema, along with a very basic implementation of a NoSQL database using the Crystal programming language.
- [PostgreSQL, The NoSQL Database (2015)](https://www.linuxjournal.com/content/postgresql-nosql-database) - An argument for PostgreSQL being an alternative to NoSQL databases with NoSQL-like features using its new features like HStore (key-value store) and JSONB (document-based) as of Version 9.4.

