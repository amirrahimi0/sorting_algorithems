<div dir=rtl align=justify>

<img src="https://aut.ac.ir/templates/tmpl_modern01/images/logo_fa.png" alt="Amirkabir University Logo" width="200" align=left>
<font size=6>
<br>
<b>ساختمان داده و الگوریتم ها</b>
<br>
</font>

<font size=3>
<b>الگوریتم های مرتب سازی</b>
<br>
<b>
استاد : اردشیر دولتی
</b>
</font>
<hr color="#999999" >


<div dir="rtl" style="text-align: justify;">
<font size=5>
<p dir="rtl" style="text-align: justify;">   
    <b>Bubble Sort</b>
</font>
</p>
مرتب‌سازی حبابی یک الگوریتم ساده برای مرتب‌سازی لیست‌ها است. این الگوریتم با پیمایش لیست و مقایسه عناصر مجاور کار می‌کند و در صورت نیاز آنها را جابجا می‌کند. این کار تا زمانی ادامه می‌یابد که هیچ جابجایی در لیست رخ ندهد، به این معنی که لیست مرتب شده است.
</div>

<font size=5>
<p dir="rtl" style="text-align: justify;">
<b>
مراحل الگوریتم
</b>
</p>
</font>
<p dir="rtl" style="text-align: justify;">
1. ابتدا یک متغیر i را برای پیمایش لیست از ابتدا تا انتها در نظر بگیرید.
</p>
<p dir="rtl" style="text-align: justify;">
2. در هر مرحله، عنصر i را با عنصر بعدی (i+1) مقایسه کنید.
</p>
<p dir="rtl" style="text-align: justify;">
3. اگر عنصر i بزرگتر از عنصر i+1 باشد، آنها را جابجا کنید.
</p>
<p dir="rtl" style="text-align: justify;">
4. متغیر i را یک واحد افزایش دهید و مراحل 2 و 3 را تا زمانی که i به انتهای لیست (n-1) نرسد، تکرار کنید.
</p>
<p dir="rtl" style="text-align: justify;">
5. مراحل 2 تا 4 را تا زمانی که هیچ جابجایی در لیست رخ ندهد، تکرار کنید.
</p>

<hr style="border-top: dotted 3px; background-color: transparent;">


<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
۱. تکرار اول (مقایسه و جابجایی)
</b>
</p>
</font>
<ul dir="rtl" style="text-align: justify; ">
  <li>از شاخص (ایندکس) اول شروع می‌کنیم و اولین و دومین عنصر را مقایسه می‌کنیم.</li>  
  <li>اگر عنصر اول از عنصر دوم بزرگتر باشد، آنها را جابجا می‌کنیم.</li>
  <li>حالا عنصر دوم و سوم را مقایسه می‌کنیم. در صورت نیاز (قرار نداشتن به ترتیب صعودی) آنها را هم جابجا می‌کنیم.</li> 
  <li>همین روند را تا آخرین عنصر ادامه می‌دهیم.</li>
</ul>
</br>




$$
i=0
$$

$$
j=0 \qquad % Adds some space after i=0
\begin{aligned}
\underset{\uparrow}{\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}}
\underset{\uparrow}{\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\end{aligned}
$$

$$
j=1 \qquad 
\begin{aligned}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}}
\underset{\uparrow}{\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\end{aligned}
$$

$$
j=2 \qquad 
\begin{aligned}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\end{aligned}
$$


$$
j=3 \qquad 
\begin{aligned}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}}
\underset{\uparrow}{\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}}
\hspace{1cm}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 4  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\end{aligned}
$$

<hr style="border-top: dotted 3px; background-color: transparent;">

<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
2. تکرارهای باقیمانده
</b>
</p>
</font>
<ul dir="rtl" style="text-align: justify; ">
  <li>این فرآیند برای تکرارهای باقیمانده نیز ادامه می یابد.</li>  
  <li>پس از هر تکرار، بزرگترین عنصر در میان عناصر مرتب نشده در انتها قرار می گیرد.</li>
</ul>
</br>



$$
i=1
$$

$$
j=0 \qquad % Adds some space after i=0
\begin{aligned}
\underset{\uparrow}{\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}}
\underset{\uparrow}{\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 4  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\hspace{1cm}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 4  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\end{aligned}
$$

$$
j=1 \qquad 
\begin{aligned}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}}
\underset{\uparrow}{\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}}
\hspace{0cm}
\begin{array}{|c|}
\hline 4  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\hspace{1cm}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 4  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\end{aligned}
$$

$$
j=2 \qquad 
\begin{aligned}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 4  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\hspace{1cm}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 4  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\end{aligned}
$$

<hr style="border-top: dotted 3px; background-color: transparent;">

<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
پیچیدگی زمانی
</b>
</p>
</font>

<p dir="rtl" style="text-align: justify; ">
مرتب‌سازی حبابی در بدترین حالت پیچیدگی زمانی O(n^2) دارد. این به این معنی است که زمان اجرا با مجذور طول لیست (n) افزایش می‌یابد. دلیل این امر این است که در بدترین حالت، الگوریتم مجبور است برای هر عنصر لیست (n)، n-1 مقایسه انجام دهد.
</p>

<p dir="rtl" style="text-align: justify; ">
<b>
بدترین حالت پیچیدگی زمانی
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>اگر بخواهیم لیست را به ترتیب صعودی مرتب کنیم و لیست به ترتیب نزولی باشد، بدترین حالت رخ می‌دهد.</li>  
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
بهترین حالت پیچیدگی زمانی
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>اگر لیست از قبل مرتب شده باشد، نیازی به مرتب‌سازی وجود ندارد و بهترین حالت اتفاق می‌افتد.</li>  
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
پیچیدگی زمانی در حالت میانگین
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>این حالت زمانی رخ می‌دهد که عناصر لیست به صورت نامرتب (نه صعودی و نه نزولی) در کنار هم قرار گرفته باشند.</li>  
</ul>
</br>


$$
\begin{array}{|c|c|c|c|}
\hline \text { Worst Time } & \text { Best Time } & \text { Average } & \text { Sorting Algorithm } \\
\hline O\left(n^2\right) & O(n) & O\left(n^2\right) & \text { Bubble Sort } \\
\hline
\end{array}
$$


<hr style="border-top: dotted 3px; background-color: transparent;">
<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
مزایا و معایب
</b>
</p>
</font>
<p dir="rtl" style="text-align: justify; ">
<b>
مزایا:
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>ساده و قابل فهم</li>  
  <li>پیاده‌سازی آسان</li>
  <li>برای لیست‌های کوچک کارآمد</li>
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
معایب:
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>در بدترین حالت پیچیدگی زمانی O(n^2) دارد</li>  
  <li>برای لیست‌های بزرگ ناکارآمد</li>
</ul>
</br>
<hr color="#999999" >

<div dir="rtl" style="text-align: justify;">
<font size=5>
<p dir="rtl" style="text-align: justify;">   
    <b>Insertion Sort</b>
</font>
</p>
Insertion Sort یک الگوریتم مرتب‌سازی کارآمد است که بر اساس مرتب‌سازی فهرستی از کارت‌ها عمل می‌کند. فرض کنید فهرستی از اعداد دارید و می‌خواهید آن‌ها را به ترتیب صعودی مرتب کنید. Insertion Sort با در نظر گرفتن اولین عنصر به عنوان زیرفهرست مرتب‌شده شروع می‌شود. سپس، به طور مکرر عنصر بعدی را در نظر می‌گیرد و آن را در جایگاه صحیح آن درون زیرفهرست مرتب‌شده قرار می‌دهد.
</div>
</br>

<font size=5>
<p dir="rtl" style="text-align: justify;">
<b>
مراحل الگوریتم
</b>
</p>
</font>
<p dir="rtl" style="text-align: justify;">
1. اولین عنصر آرایه را به عنوان زیرفهرست مرتب‌شده در نظر بگیرید.
</p>
<p dir="rtl" style="text-align: justify;">
2. به ترتیب از عنصر دوم تا عنصر آخر آرایه را بررسی کنید.
</p>
<p dir="rtl" style="text-align: justify;">
3. برای هر عنصر، آن را با عناصر موجود در زیرفهرست مرتب‌شده مقایسه کنید.
</p>
<p dir="rtl" style="text-align: justify;">
4. اگر عنصر جاری از عنصری در زیرفهرست مرتب‌شده کوچکتر باشد، جایگاه آن عنصر را در زیرفهرست پیدا کنید و عنصر جاری را در آن جایگاه درج کنید.
</p>
<p dir="rtl" style="text-align: justify;">
5. مراحل 2 تا 4 را برای تمام عناصر باقی‌مانده آرایه تکرار کنید.
</p>

<hr style="border-top: dotted 3px; background-color: transparent;">


<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
مثال
</b>
</p>
</font>
<ul dir="rtl" style="text-align: justify; ">
  <li>عنصر اول (5) به عنوان زیرفهرست مرتب‌شده در نظر گرفته می‌شود.</li>  
  <li>عنصر دوم (3) با عنصر اول (5) مقایسه می‌شود.</li>
  <li>از آنجا که 3 < 5، عنصر 3 باید قبل از 5 قرار بگیرد.</li> 
  <li>عنصر 3 در جایگاه صحیح خود در زیرفهرست درج می‌شود.</li>
</ul>
</br>


$$
Initial State
$$

$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


<hr style="border-top: dotted 1px; background-color: transparent;">



$$
Iteration=1
$$

$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\underset{\uparrow}{\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
Final \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$

<hr style="border-top: dotted 1px; background-color: transparent;">

$$
Iteration=2
$$

$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\underset{\uparrow}{\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
Final \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$

<hr style="border-top: dotted 1px; background-color: transparent;">


$$
Iteration=3
$$

$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}}
\hspace{0cm}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\underset{\uparrow}{\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\hspace{1cm}
Final \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$



<hr style="border-top: dotted 1px; background-color: transparent;">


$$
Iteration=4
$$

$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}}
\begin{array}{|c|}
\hline   \\
\hline
\end{array}
\end{aligned}
$$


$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}}
\hspace{1cm}
SubList \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}}
\hspace{0cm}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\end{aligned}
$$



$$
\begin{aligned}
\begin{array}{|c|}
\hline 5  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  1 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 2  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}}
\hspace{1cm}
Final \longrightarrow  % Adds some space after i=0
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  2 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline  4 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  5 \\
\hline
\end{array}
\end{aligned}
$$
<hr style="border-top: dotted 3px; background-color: transparent;">
<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
پیچیدگی زمانی
</b>
</p>
</font>

<p dir="rtl" style="text-align: justify; ">
مرتب‌سازی  (Insertion Sort) نیز در بدترین حالت دارای پیچیدگی زمانی   O(n^2) است. این به این معناست که زمان اجرا با مجذور طول لیست افزایش می‌یابد. دلیل این امر این است که در بدترین حالت، الگوریتم برای هر عنصر لیست ، تمام عناصر قبلی را باید با آن مقایسه کند تا مکان مناسب برای قرار گرفتن آن را پیدا کند.
</p>

<p dir="rtl" style="text-align: justify; ">
<b>
بدترین حالت پیچیدگی زمانی
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>آرایه ورودی به صورت ترتیب نزولی مرتب است. در این صورت، هر عنصر باید در کل فهرست مرتب‌شده به عقب برگردد تا جایگاه درستش را بیابد. این حالت نیز پیچیدگی زمانی درجه دو  خواهد داشت - O(n^2).</li>  
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
بهترین حالت پیچیدگی زمانی
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>اگر لیست از قبل مرتب شده باشد، نیازی به مرتب‌سازی وجود ندارد و بهترین حالت اتفاق می‌افتآرایه ورودی از قبل مرتب است. در این صورت، هر عنصر تنها یک بار با عنصر قبلی خود مقایسه می‌شود. در نتیجه، پیچیدگی زمانی خطی خواهد بود - O(n).</li>  
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
پیچیدگی زمانی در حالت میانگین
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>آرایه ورودی به صورت تصادفی مرتب است. در این حالت، به صورت میانگین باید هر عنصر را با نصف عناصر مرتب‌شده قبلی مقایسه و جابه‌جا کنیم. این حالت منجر به پیچیدگی زمانی درجه دو  می‌شود - O(n^2).</li>  
</ul>
</br>


$$
\begin{array}{|c|c|c|c|}
\hline \text { Worst Time } & \text { Best Time } & \text { Average } & \text { Sorting Algorithm } \\
\hline O\left(n^2\right) & O(n) & O\left(n^2\right) & \text { Insertion Sort } \\
\hline
\end{array}
$$


<hr style="border-top: dotted 3px; background-color: transparent;">
<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
مزایا و معایب
</b>
</p>
</font>
<p dir="rtl" style="text-align: justify; ">
<b>
مزایا:
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>ساده برای پیاده‌سازی و درک/li>  
  <li>حافظه کمی مصرف می‌کند</li>
  <li>برای لیست‌های کوچک کارآمد</li>
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
معایب:
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>در بدترین حالت پیچیدگی زمانی O(n^2) دارد</li>  
  <li>برای لیست‌های بزرگ ناکارآمد</li>
</ul>
</br>
<hr color="#999999" >

<div dir="rtl" style="text-align: justify;">
<font size=5>
<p dir="rtl" style="text-align: justify;">   
    <b>Quick Sort</b>
</font>
</p>
مرتب‌سازی سریع (Quick Sort) یکی از الگوریتم‌های مشهور مرتب‌سازی داده‌ها است که از روش Divide and Conquer برای مرتب‌سازی آرایه‌ها استفاده می‌کند. این الگوریتم به طور کلی سریع‌تر از Insertion Sort است و برای مرتب‌سازی آرایه‌های بزرگ کارآمدتر عمل می‌کند.
</div>
</br>

<font size=5>
<p dir="rtl" style="text-align: justify;">
<b>
مراحل الگوریتم
</b>
</p>
</font>
<p dir="rtl" style="text-align: justify;">
1. انتخاب عنصر محوری: اولین عنصر آرایه را به عنوان عنصر محوری (pivot) انتخاب کنید.
</p>




<p dir="rtl" style="text-align: justify;">
2. تقسیم آرایه: آرایه را به دو بخش چپ و راست عنصر محوری تقسیم کنید.
<ul dir="rtl" style="text-align: justify; ">
  <li>بخش چپ: شامل تمام عناصر کوچکتر یا مساوی عنصر محوری</li> 
  <li>بخش راست: شامل تمام عناصر بزرگتر از عنصر محوری</li>   
</ul>
</p>
<p dir="rtl" style="text-align: justify;">
3. مرتب‌سازی بازگشتی:
<ul dir="rtl" style="text-align: justify; ">
  <li>بخش چپ: الگوریتم Quick Sort را به طور بازگشتی روی بخش چپ آرایه اجرا کنید./li> 
  <li>بخش راست: شامل تمام عناصر بزرگتر از عنصر محوری</li>   
</ul>
</p>
<p dir="rtl" style="text-align: justify;">
4. ترتیب نهایی: آرایه مرتب‌شده نهایی از ترکیب بخش‌های چپ و راست مرتب‌شده و عنصر محوری تشکیل می‌شود.
</p>

<hr style="border-top: dotted 3px; background-color: transparent;">



<font size=5>
<p dir="rtl" style="text-align: justify;">
<b>
روش‌های مختلف انتخاب عنصر محوری (Pivot)
</b>
</p>
</font>
<p dir="rtl" style="text-align: justify;">
انتخاب مناسب عنصر محوری نقش مهمی در عملکرد Quick Sort دارد. در اینجا روش‌های رایج انتخاب pivot شرح داده می‌شود:
</p>

<p dir="rtl" style="text-align: justify;">
1. انتخاب اولین یا آخرین عنصر:
<ul dir="rtl" style="text-align: justify; ">
  <li>ساده‌ترین روش است.</li> 
  <li>معایب: اگر آرایه ورودی تقریباً مرتب یا مرتب به صورت نزولی باشد، به‌شدت ناکارآمد است و منجر به پیچیدگی زمانی O(n^2) می‌شود.</li>   
</ul>
</p>
<p dir="rtl" style="text-align: justify;">
2. انتخاب تصادفی:
<ul dir="rtl" style="text-align: justify; ">
  <li>یک عنصر به صورت تصادفی از آرایه انتخاب می‌شود.</li> 
  <li>مزایا: احتمال بدترین حالت را کاهش می‌دهد.</li>   
  <li>معایب: تولید اعداد تصادفی  محاسباتی اضافی ایجاد می‌کند.</li>   
</ul>
</p>
<p dir="rtl" style="text-align: justify;">
3. انتخاب میانه (Median):
<ul dir="rtl" style="text-align: justify; ">
  <li>میانه، عنصر میانی است اگر آرایه مرتب بود.</li> 
  <li>مزایا: احتمال بدترین حالت را کاهش می‌دهمزایا: تقسیم آرایه را به بهترین صورت متعادل می‌کند.</li>   
  <li>معایب: پیدا کردن میانه واقعی، زمان‌بر است.</li>   
</ul>
</p>
<p dir="rtl" style="text-align: justify;">
4. میانه ‌از سه (Median-of-Three):
<ul dir="rtl" style="text-align: justify; ">
  <li>یافتن میانه از میان سه عنصر (اولین، میانی، آخرین) آرایه.</li> 
  <li>مزایا: متعادل‌سازی تقریبی را تضمین می‌کند و به اندازه پیدا کردن میانه دقیق زمان‌بر نیست.</li>   
  <li>معایب: پیدا کردن میانه واقعی، زمان‌بر است.</li>   
</ul>
</p>
<p dir="rtl" style="text-align: justify;">
5. روش تقریبی میانه:
<ul dir="rtl" style="text-align: justify; ">
  <li>چندین عنصر تصادفی را از آرایه انتخاب می‌شود، میانه این عناصر نمونه‌برداری شده به عنوان یک تقریب از میانه آرایه استفاده می‌شود.</li> 
  <li>مزایا: پیاده‌سازی سریع در عین داشتن احتمال معقول برای انتخاب یک عنصر محوری متعادل.</li>     
</ul>
</p>
<hr style="border-top: dotted 1px; background-color: transparent;">

<p dir="rtl" style="text-align: justify;">
انتخاب عنصر محوری خوب برای کارآمدی Quick Sort حیاتی است. بدترین حالت منجر به پیچیدگی زمانی مرتبه  O(n^2) می شود (حتی بدتر از Insertion Sort). اما در حالت ایده آل، با بهینه‌سازی انتخاب عنصر محوری، پیچیدگی متوسط Quick Sort به  O(n log n) می‌رسد که کارآمدتر از بسیاری از الگوریتم‌های مرتب‌سازی است.
</p>






<ul dir="rtl" style="text-align: justify; ">
  <li>هیچ روش مطلقی برای انتخاب عنصر محوری وجود ندارد. انتخاب مناسب به ویژگی‌های خاصی از داده ورودی بستگی دارد.</li> 
  <li>برای آرایه‌های تصادفی، انتخاب تصادفی و "میانه از سه" معمولاً به خوبی کار می‌کنند.</li>   
  <li>برای آرایه‌های تقریباً مرتب‌شده، انتخاب عنصر میانه یا به کار بردن روش تقریبی میانه بهتر عمل می‌کنند.</li>   
</ul>

<hr style="border-top: dotted 3px; background-color: transparent;">


<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
مثال
</b>
</font>
</p>
<p dir="rtl" style="text-align: justify; ">
فرض می‌کنیم قصد دارید آرایه زیر را با استفاده از مرتب‌سازی سریع (Quick Sort) که عنصر آخر آرایه را به عنوان عنصر محوری در نظر می‌گیرد، مرتب کنید. در اینجا گام‌های مرتب‌سازی شرح داده شده‌اند:
</p>
</br>











$$
\begin{aligned}
\begin{array}{|c|}
\hline 8  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 7  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  \color{green}{4} \\
\hline
\end{array}
\end{aligned}
$$


<p dir="rtl" >
<b>استفاده از اشاره‌گرها:</b> دو اشاره‌گر "چپ" و "راست" تعریف می‌شوند. اشاره‌گر چپ از ابتدای آرایه  و اشاره‌گر راست از انتهای آرایه (به جز عنصر محوری) شروع می‌کنند.
</p>





$$
\begin{aligned}
\underset{\uparrow}{\begin{array}{|c|}
\hline 8  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline 7  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}
\overset{\downarrow}{\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  \color{green}{4} \\
\hline
\end{array}
\end{aligned}
$$

<p dir="rtl" style="text-align: justify;">
<b>
مقایسه و جابجایی:
</b>
<ul dir="rtl" style="text-align: justify; ">
  <li>اشاره‌گر چپ: به سمت راست حرکت می‌کند و از کنار زدن عناصر کوچکتر از عنصر محوری عبور می‌کند. تا زمانی که به عنصری بزرگتر یا مساوی عنصر محوری برسد، متوقف می‌شود.</li> 
  <li>اشاره‌گر راست: به سمت چپ حرکت می‌کند و از کنار زدن عناصر بزرگتر از عنصر محوری عبور می‌کند. تا زمانی که به عنصری کوچکتر یا مساوی عنصر محوری برسد، متوقف می‌شود.</li>     
  <li>جابجایی: اگر اشاره‌گر چپ به عنصری کوچکتر از عنصر اشاره‌گر راست اشاره می‌کند، آن دو عنصر را جابجا می‌کنیم.</li>     
  <li>تکرار: این فرایند مقایسه و جابجایی تا زمانی که اشاره‌گر چپ و راست از یکدیگر عبور کنند، ادامه می‌یابد.</li>     
</ul>
</p>


$$
\begin{aligned}
&\begin{array}{l}
\text{8} > \text{4} \ \checkmark \\
\text{3} < \text{4} \ \checkmark
\end{array}
\quad
\underset{\uparrow}{\begin{array}{|c|}
\hline 8  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline 7  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}
\overset{\downarrow}{\begin{array}{|c|}
\hline  3 \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  \color{green}{4} \\
\hline
\end{array}
\end{aligned}
$$

<p dir="rtl" style="text-align: justify; ">
- 8 و 3 جابجا شده و اشاره گر ها به خانه های بعدی میروند.
</p>


$$
\begin{aligned}
&\begin{array}{l}
\text{7} > \text{4} \ \checkmark \\
\text{6} < \text{4} \ \times
\end{array}
\quad
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline 7  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\overset{\downarrow}{\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  8 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  \color{green}{4} \\
\hline
\end{array}
\end{aligned}
$$

<p dir="rtl" style="text-align: justify; ">
- اشاره گر چپ ثابت می ماند اشاره گر راست جلو میرود تا زمانی که عدد کوچکتر و یا از اشاره گر چپ عبور کند.
</p>


$$
\begin{aligned}
&\begin{array}{l}
\text{7} > \text{4} \ \checkmark \\
\text{1} < \text{4} \ \checkmark
\end{array}
\quad
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\underset{\uparrow}{\begin{array}{|c|}
\hline 7  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}
\hspace{0cm}
\overset{\downarrow}{\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  8 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  \color{green}{4} \\
\hline
\end{array}
\end{aligned}
$$

<p dir="rtl" style="text-align: justify; ">
- 7 و 1 جابجا شده و اشاره گر ها به خانه های بعدی میروند.
</p>

$$
\begin{aligned}
&\begin{array}{l}
\text{0} > \text{4} \ \times \\
\text{0} < \text{4} \ \checkmark
\end{array}
\quad
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\overset{\downarrow}{\underset{\uparrow}{\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}}}
\hspace{0cm}
\begin{array}{|c|}
\hline 7  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  8 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  \color{green}{4} \\
\hline
\end{array}
\end{aligned}
$$

<p dir="rtl" style="text-align: justify; ">
- اشاره گر چپ ثابت می ماند اشاره گر راست جلو میرود تا زمانی که عدد کوچکتر و یا از اشاره گر چپ عبور کند.
</p>



$$
\begin{aligned}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\overset{\downarrow}{\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}}
\hspace{0cm}
\underset{\uparrow}{\begin{array}{|c|}
\hline 7  \\
\hline
\end{array}}
\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  8 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  \color{green}{4} \\
\hline
\end{array}
\end{aligned}
$$


<p dir="rtl" style="text-align: justify; ">
-  اشاره‌گر چپ و راست از یکدیگر عبور کردند پس همه عناصر چپ و راست جابجا شدند.
</p>

<p dir="rtl" style="text-align: justify; ">
-  عنصر pivot با خانه اشاره گر چپ جابجا شده و تکرار اول ما تمام میشود.
</p>




$$
\begin{aligned}
\begin{array}{|c|}
\hline 3  \\
\hline
\end{array}
\begin{array}{|c|}
\hline 1  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  0 \\
\hline
\end{array}
\hspace{0cm}
\begin{array}{|c|}
\hline \color{green}{4}  \\
\hline
\end{array}
\begin{array}{|c|}
\hline  6 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  8 \\
\hline
\end{array}
\begin{array}{|c|}
\hline  7 \\
\hline
\end{array}
\end{aligned}
$$


<p dir="rtl" style="text-align: justify; ">
-  حال به همین ترتیب Quick sort را برای قسمت چپ و راست pivot انجام میدهیم.
</p>

<hr style="border-top: dotted 3px; background-color: transparent;">
<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
پیچیدگی زمانی
</b>
</p>
</font>

<p dir="rtl" style="text-align: justify; ">
مرتب‌سازی سریع (Quick Sort) در بدترین حالت، پیچیدگی زمانی O(n^2) دارد. به این معنی که زمان اجرا با مجذور طول لیست افزایش می‌یابد. دلیل این امر این است که در بدترین حالت، الگوریتم برای هر عنصر لیست، تمام عناصر قبلی را باید با آن مقایسه کند تا مکان مناسب برای قرار گرفتن آن را پیدا کند.
</p>

<p dir="rtl" style="text-align: justify; ">
<b>
بدترین حالت پیچیدگی زمانی
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>آرایه ورودی به صورت ترتیب نزولی مرتب است. در این حالت، هر عنصر باید در کل فهرست مرتب‌شده به عقب برگردد تا جایگاه درستش را بیابد. این حالت نیز پیچیدگی زمانی درجه دو خواهد داشت  O(n^2).</li>  
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
بهترین حالت پیچیدگی زمانی
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>آرایه ورودی از قبل مرتب است. در این حالت، هر عنصر تنها یک بار با عنصر قبلی خود مقایسه می‌شود. در نتیجه، پیچیدگی زمانی خطی خواهد بود  O(n).</li>  
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
پیچیدگی زمانی در حالت میانگین
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>آرایه ورودی به صورت تصادفی مرتب است. در این حالت، به صورت میانگین باید هر عنصر را با نصف عناصر مرتب‌شده قبلی مقایسه و جابه‌جا کنیم. این حالت منجر به پیچیدگی زمانی درجه دو می‌شود  O(n log n).</li>  
</ul>
</br>


$$
\begin{array}{|c|c|c|c|}
\hline \text { Worst Time } & \text { Best Time } & \text { Average } & \text { Sorting Algorithm } \\
\hline O(n^2) & O(n \log n) & O(n \log n) & \text { Quick Sort } \\
\hline
\end{array}
$$



<hr style="border-top: dotted 3px; background-color: transparent;">
<font size=5>
<p dir="rtl" style="text-align: justify; ">
<b>
مزایا و معایب
</b>
</p>
</font>
<p dir="rtl" style="text-align: justify; ">
<b>
مزایا:
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>سرعت: در حالت میانگین از مرتب‌سازی درج سریع‌تر است.</li>
  <li>کارایی: برای لیست‌های بزرگ کارآمدتر است.</li>
  <li>به حافظه اضافی نیاز ندارد.</li>
</ul>
</br>

<p dir="rtl" style="text-align: justify; ">
<b>
معایب:
</b>
</p>
<ul dir="rtl" style="text-align: justify; ">
  <li>در بدترین حالت O(n^2) است.</li>  
  <li>پیچیدگی پیاده‌سازی.</li>
</ul>
</br>
<hr color="#999999" >

