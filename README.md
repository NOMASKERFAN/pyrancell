### **کلاس Client**

*کلاس Client واسط اصلی بین کاربر و APIهای MyIrancell است.
با ساختن یک نمونه از این کلاس و وارد کردن توکن JWT، می‌توانید به تمام متدهای حساب کاربری خود دسترسی داشته باشید — از اطلاعات پروفایل گرفته تا بسته‌های اینترنت، آهنگ پیشواز، و کدهای USSD. ودعوت....*


## **⚙️ ساخت و مقداردهی اولیه**

```python

from pyrancell import Client

token =""

bot = Client(token = token , platform="web")

```


### 🟡گرفتن اطلاعات اکانت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.my_info())
```


### 🔵گرفتن نام صاحب سیم کارت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.first_name())
```




### 🟣 گرفتن فامیلی صاحب اکانت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.last_name())
```



### 🔴گرفتن ایمیل صاحب اکانت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.get_email())
```



### 🏡 گرفتن ادرس خانه ثبت شده برای سیم کارت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.get_address_home())
```




### 🟤گرفتن تاریخ فعال سازی سیم کارت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.activation_date())
```





### ⚫گرفتن تلفن خانه


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.get_phone_home())
```




### 🟢گرفتن سریال سیم کارت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.sim_card_serial_number())
```



### 🟣گرفتن امار فعال بودن سیم کارت یا غیر فعال بودن


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.state_simcard())
```



### ✅دیدن بسته های اینترنت


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.View_Internet_packages())
```




### 🔵دیدن اهنگ های پیشواز


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.View_music_default())
```



### 🟡دیدن کد های دستوری


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.Viewing_command_codes())
```



### 🔲چک کردن که ایا کاربر ایرانسل من داره یا خیر


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.phone_has_app(phone=""))
```



### 💛دعوت کردن کاربر به ایرانسل من و دریافت هدیه در صورت نصب


```python
from pyrancell import Client

token =""
bot = Client(token = token , platform="web")

print(bot.send_invite(phone=""))
```
