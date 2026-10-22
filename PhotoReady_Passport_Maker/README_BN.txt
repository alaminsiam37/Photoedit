PhotoReady — Passport Photo Maker
==================================

ফাইল:
- index.html : সম্পূর্ণ ওয়েবসাইট (HTML, CSS, JavaScript এক ফাইলে)

ফিচার:
- অ্যাকাউন্ট ছাড়াই ছবি আপলোড
- ব্রাউজারে AI background removal (IMG.LY package, esm.sh CDN থেকে লোড)
- সাদা/নীল/ধূসর/গোলাপি/custom background
- 35x45 mm, 33x48 mm এবং 2x2 inch output size
- brightness/contrast adjustment
- PNG download
- ছবির ফাইল কোনো PHP সার্ভারে পাঠানো হয় না; AI processing ব্রাউজারে হয়

গুরুত্বপূর্ণ:
- AI মডেল প্রথমবার CDN থেকে ডাউনলোড হবে, তাই ইন্টারনেট দরকার।
- প্রথমবার প্রসেসিং ধীর হতে পারে; দুর্বল ফোনে RAM কম থাকলে ব্যর্থ হতে পারে।
- Free hosting এই স্ট্যাটিক index.html হোস্ট করতে পারবে। PHP বা database প্রয়োজন নেই।
- AI background removal package-এর লাইসেন্স ও CDN availability প্রকাশের আগে যাচাই করুন।
- পাসপোর্ট/ভিসার সরকারি নিয়ম দেশভেদে আলাদা। এই টুল সরকারি অনুমোদন নিশ্চিত করে না।
- ছবির ক্রপ প্রাথমিকভাবে কেন্দ্রীভূত; সঠিক মুখের অবস্থান আছে কি না preview দেখে নিন।

InfinityFree-তে আপলোড:
1. InfinityFree-তে account তৈরি করে hosting account তৈরি করুন।
2. Control Panel > Online File Manager অথবা FTP খুলুন।
3. htdocs ফোল্ডারে যান।
4. default index2.html বা default welcome file থাকলে নিজের সাইটের সঙ্গে conflict এড়াতে সরিয়ে রাখুন (প্রয়োজনে আগে backup নিন)।
5. এই ZIP extract করে index.html ফাইলটি htdocs-এ upload করুন।
6. আপনার domain/subdomain খুলুন এবং ছবি দিয়ে পরীক্ষা করুন।
7. AI model লোড না হলে browser console/network, CDN access এবং internet connection পরীক্ষা করুন।

লোকাল টেস্ট:
index.html-এ ডাবল ক্লিক করে চালানোর বদলে VS Code Live Server বা Python-এর local HTTP server দিয়ে খুললে module import ভালোভাবে কাজ করে।
