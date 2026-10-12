AYAN TRAVELLING — MOBILE-ONLY INSTALL GUIDE

এই ফোল্ডারটি একটি PWA website package. এটি সরাসরি APK নয়। APK বানাতে Android build service/Android Studio প্রয়োজন। কম্পিউটার না থাকলে সহজ উপায় হলো HTTPS hosting-এ আপলোড করে Chrome থেকে Install করা।

মোবাইল থেকে:
1) ZIP extract করুন (Files app > Downloads > ZIP > Extract)।
2) Chrome-এ Netlify Drop বা আপনার বিদ্যমান hosting provider-এর upload page খুলুন।
3) Ayan_Travelling_Mobile_App ফোল্ডারের CONTENTS upload করুন—index.html, manifest.webmanifest, sw.js, icons ফোল্ডার একই জায়গায় থাকতে হবে।
4) Hosting থেকে পাওয়া HTTPS URL খুলুন Chrome-এ।
5) Chrome menu (⋮) > Add to Home screen / Install app চাপুন।
6) Home screen-এর Ayan Travelling আইকন থেকে খুলুন।

সতর্কতা:
- Firebase Cloud Sync কাজ করার জন্য Firebase Realtime Database rules/auth সঠিক ও নিরাপদ থাকতে হবে। এই package-এ HTML-এর Firebase config অপরিবর্তিত রাখা হয়েছে; এখানে cloud sync live test করা হয়নি।
- এই PWA install করতে APK ফাইল লাগে না। এটি হোম স্ক্রিনে অ্যাপের মতো খুলবে, কিন্তু আলাদা Android APK নয়।
- customer/ledger data-র একমাত্র কপি হিসেবে local storage-এর ওপর নির্ভর করবেন না; Firebase-এ data দেখা যাচ্ছে কি না যাচাই করুন।
