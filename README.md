<div align="center">
  
  <!-- HEADER BANNER -->
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=700&size=30&duration=3000&pause=500&color=F0B90B&center=true&vCenter=true&width=600&lines=Leila+LNT;Trader+%26+Financial+Developer;Pine+Script+%7C+MQL4+%7C+MQL5;Algorithmic+Trading+Expert" alt="Typing SVG" />
  
  <br/>
  
  <p>
    <img src="https://img.shields.io/badge/Pine%20Script-2.0+-brightgreen?style=for-the-badge&logo=tradingview&color=F0B90B" />
    <img src="https://img.shields.io/badge/MQL5-Expert-blue?style=for-the-badge&logo=meta&color=F0B90B" />
    <img src="https://img.shields.io/badge/MQL4-Developer-orange?style=for-the-badge&logo=meta&color=F0B90B" />
    <img src="https://img.shields.io/badge/Trader-Professional-gold?style=for-the-badge&logo=tradingview&color=F0B90B" />
  </p>
  
  <br/>
  
  <!-- SOCIAL BADGES -->
  <p>
    <a href="https://t.me/YourTelegram" target="_blank">
      <img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" />
    </a>
    <a href="https://wa.me/YourPhoneNumber" target="_blank">
      <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" />
    </a>
    <a href="https://linkedin.com/in/YourLinkedIn" target="_blank">
      <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
    </a>
    <a href="https://github.com/leilalnt" target="_blank">
      <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
    </a>
    <a href="mailto:your.email@gmail.com">
      <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
    </a>
  </p>
  
  <br/>
  
  <img src="https://capsule-render.vercel.app/api?type=waving&color=F0B90B&height=100&section=footer" width="100%" />
  
</div>

---

## 👩‍💻 درباره من

> **برنامه‌نویس حرفه‌ای پاین اسکریپت و متاتریدر | تریدر فعال بازارهای مالی**

سلام! من **لیلا** هستم، یک برنامه‌نویس و تریدر با تجربه در زمینه **سیستم‌های معاملاتی الگوریتمی** و **تحلیل تکنیکال**. بیش از ۳ سال است که در بازارهای مالی فعالیت می‌کنم و استراتژی‌های معاملاتی را به کدهای قابل اجرا در پلتفرم‌های معروف تبدیل می‌کنم.

### 🔥 توانایی‌های من:

- ✍️ **نویسندگی پاین اسکریپت** (TradingView) - از اندیکاتورهای ساده تا استراتژی‌های پیشرفته
- 🤖 **توسعه ربات‌های معاملاتی** در متاتریدر ۴ و ۵ (MQL4/MQL5)
- 📊 **تحلیل تکنیکال** و شناسایی الگوهای سودآور
- 🧠 **مدیریت ریسک** و بهینه‌سازی پورتفولیو
- 🎯 **آموزش** مفاهیم تریدینگ و برنامه‌نویسی مالی

---

## 🛠️ پروژه‌های شاخص

### 🔹 اندیکاتورهای پاین اسکریپت

| نام پروژه | توضیحات | وضعیت |
|-----------|---------|--------|
| **🦅 ابر‌ترند هوشمند** | ترکیب ابر‌ترند با فیلتر نویز و سیگنال‌های ورود دقیق | ✅ منتشر شده |
| **📊 ویو‌آلرت پرو** | هشداردهنده چندزمانه با تشخیص الگوهای کندلی و واگرایی RSI | ✅ منتشر شده |
| **🎯 اسکالپر سریع** | اندیکاتور مخصوص اسکالپ با تایم‌فریم‌های پایین | 🔄 در حال توسعه |

### 🔹 ربات‌های متاتریدر

| نام پروژه | پلتفرم | توضیحات |
|-----------|---------|---------|
| **🤖 ربات طلایی** | MQL5 | ربات اسکالپر تمام‌اتوماتیک با مدیریت سرمایه پویا |
| **📈 ترندفالوور** | MQL4 | ربات دنبال‌کننده روند با فیلترهای هوشمند |
| **⚡ بریک‌اوت‌ر** | MQL5 | شناسایی و معامله در نوک شکست‌ها |

---

## 📚 نمونه کدها

### نمونه کد پاین اسکریپت (استراتژی ساده)

```pinescript
//@version=5
strategy("استراتژی دنبال‌کننده روند", overlay=true, margin_long=100, margin_short=100)

// اندیکاتورها
fastMA = ta.sma(close, 10)
slowMA = ta.sma(close, 30)

// شرایط ورود
longCondition = ta.crossover(fastMA, slowMA)
shortCondition = ta.crossunder(fastMA, slowMA)

// اجرای معاملات
if (longCondition)
    strategy.entry("Long", strategy.long)

if (shortCondition)
    strategy.entry("Short", strategy.short)

// نمایش
plot(fastMA, color=color.green, linewidth=2)
plot(slowMA, color=color.red, linewidth=2)
