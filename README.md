# Thailand Government Lottery Portal (Mobile-First + Supabase + Vercel)

এই প্রজেক্টটি সরাসরি **GitHub + Supabase + Vercel** ব্যবহার করে লাইভ করার জন্য তৈরি করা হয়েছে।

## লাইভ করার ধাপসমূহ (Step-by-Step Setup):

### ধাপ ১: Supabase সেটআপ (Database & Realtime)
1. [Supabase.com](https://supabase.com)-এ লগইন করে একটি **New Project** তৈরি করুন।
2. বামপাশের মেনু থেকে **SQL Editor**-এ যান এবং ফোল্ডারে থাকা `supabase-schema.sql` ফাইলের সম্পূর্ণ কোডটি পেস্ট করে **Run** চাপুন।
3. এরপর **Project Settings -> API** থেকে নিচের দুটি তথ্য কপি করুন:
   - **Project URL**
   - **anon public key**
4. `config.js` ফাইলটি ওপেন করে `YOUR_SUPABASE_PROJECT_URL` এবং `YOUR_SUPABASE_ANON_KEY` এর জায়গায় আপনার তথ্য দুটি বসিয়ে সেভ করুন।

### ধাপ ২: GitHub আপলোড
1. [GitHub.com](https://github.com)-এ একটি নতুন Repository তৈরি করুন (যেমন: `thai-lottery-portal`)।
2. এই জিপ ফাইলের ভেতরের সব ফাইল (`index.html`, `config.js`, `vercel.json`, `supabase-schema.sql`, `README.md`) আপনার GitHub রিপোজিটরিতে আপলোড করুন।

### ধাপ ৩: Vercel-এ লাইভ (Deploy)
1. [Vercel.com](https://vercel.com)-এ GitHub দিয়ে লগইন করুন।
2. **Add New -> Project** ক্লিক করে আপনার `thai-lottery-portal` রিপোজিটরিটি সিলেক্ট করুন এবং **Deploy** বাটনে ক্লিক করুন।

### অ্যাডমিন প্যানেল ব্যবহারের নিয়ম:
- **পাবলিক ইউজার লিংক:** `https://your-site.vercel.app` (এখানে অ্যাডমিন প্যানেলের কোনো বাটন দেখা যাবে না)
- **অ্যাডমিন প্যানেল লিংক:** `https://your-site.vercel.app/#admin`
- **ডিফল্ট অ্যাডমিন পাসওয়ার্ড:** `admin123`
