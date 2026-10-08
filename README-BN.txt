SSC CGL 2027 PERSONAL APP - VERSION 1

এই package-এ আছে:
- Daily goals + checkbox
- Daily completion %
- Weekly %
- Study streak
- SSC CGL subject/chapter tracker
- Chapter status
- Subject progress
- Offline local storage
- Installable PWA structure

গুরুত্বপূর্ণ:
বর্তমান build-এ "Login / Create local account" শুধু এই device-এর local account।
একই account দিয়ে অন্য ফোনে data পাওয়ার জন্য Firebase/Supabase backend credentials লাগবে।
Backend ছাড়া সত্যিকারের cloud login/sync দাবি করা যাবে না।

পরবর্তী production setup:
1. Firebase Authentication অথবা Supabase Auth চালু করুন।
2. Firestore/Supabase Database-এ user-specific goals, chapter status, revision, mock data রাখুন।
3. index.html-এর localStorage layer-কে backend API/SDK layer দিয়ে replace করুন।
4. HTTPS hosting-এর পরে PWA install করুন।
