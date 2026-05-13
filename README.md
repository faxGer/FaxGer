## Hi there 👋

<!--
**faxGer/FaxGer** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
# 📦 FaxGer Global Logistics - Web Portal

FaxGer হলো একটি আধুনিক ইন্টারন্যাশনাল কুরিয়ার সার্ভিস ম্যানেজমেন্ট সিস্টেম। এই পোর্টালটি মূলত **Google Apps Script (GAS)** এবং **GitHub Pages** এর সমন্বয়ে তৈরি করা হয়েছে, যা ব্যবহারকারীদের পার্সেল ট্র্যাকিং, রেট ক্যালকুলেশন এবং কোম্পানির সার্ভিস সম্পর্কে বিস্তারিত তথ্য প্রদান করে।

## 🚀 Live Demo
আপনার ডোমেইন ব্যবহার করে সরাসরি এক্সেস করুন:
- **🏠 Home Page:** [www.faxger.com](https://www.faxger.com)
- **🔍 Tracking Page:** [www.faxger.com/?p=track](https://www.faxger.com/?p=track)
- **💰 Rate Chart:** [www.faxger.com/?p=rate](https://www.faxger.com/?p=rate)

---

## 🛠 Tech Stack
- **Frontend:** HTML5, CSS3 (Tailwind CSS), JavaScript
- **Backend:** Google Apps Script (GAS)
- **Database:** Google Sheets (Linked via GAS)
- **Hosting:** GitHub Pages
- **Domain:** Namecheap Custom Domain Integration

---

## 📂 Project Structure

### 1. GitHub (Deployment Layer)
GitHub-এ মূলত একটি ডাইনামিক `index.html` ফাইল রয়েছে যা কুয়েরি প্যারামিটার (`?p=`) এর ওপর ভিত্তি করে Google Apps Script থেকে সঠিক ইন্টারফেসটি লোড করে।
- `index.html`: মূল গেটওয়ে ফাইল যা আইফ্রেম (Iframe) এর মাধ্যমে ব্যাকএন্ডকে যুক্ত করে।

### 2. Google Apps Script (Logic Layer)
আপনার Google অ্যাকাউন্টে এই স্ক্রিপ্টগুলো রান করছে:
- `Code.gs`: রাউটিং লজিক হ্যান্ডেল করে।
- `home.html`: মেইন ল্যান্ডিং পেজ।
- `track.html`: রিয়েল-টাইম ট্র্যাকিং সিস্টেম।
- `rate.html`: শিপিং রেট ক্যালকুলেটর।

---

## ⚙️ How It Works
এই প্রজেক্টটি একটি **Single Entry Point** লজিক ব্যবহার করে:
1. ইউজার যখন `faxger.com/?p=track` এ প্রবেশ করে, তখন ব্রাউজার জাভাস্ক্রিপ্ট প্যারামিটার `p` এর ভ্যালু (`track`) সংগ্রহ করে।
2. এই ভ্যালুটি Google Apps Script-এর Web App URL-এর সাথে যুক্ত হয়ে আইফ্রেমের ভেতরে নির্দিষ্ট পেজটি লোড করে।
3. এর ফলে ইউজার আপনার কাস্টম ডোমেইনেই থাকে, কিন্তু ডেটা এবং ফাংশনালিটি আসে Google Script থেকে।

---

## 🔧 Installation & Setup
আপনি যদি এই প্রজেক্টটি ক্লোন করতে চান:
1. আপনার Google Apps Script প্রোজেক্টে `Code.gs` এবং HTML ফাইলগুলো আপলোড করুন।
2. স্ক্রিপ্টটি **Web App** হিসেবে ডিপ্লয় করুন (Access: *Anyone*)।
3. GitHub-এর `index.html` ফাইলে আপনার **Deployment URL**-টি আপডেট করুন।
4. GitHub Settings থেকে **Custom Domain** এবং Namecheap DNS কনফিগার করুন।

---

## 👨‍💻 Author
**Tonmoy Sarker** *Sales Officer, Uttara Zone* *FaxGer Global Logistics* ---

### 📝 License
This project is private and intended for **FaxGer Global Logistics**.
