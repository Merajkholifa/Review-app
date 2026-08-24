# Icon package

GitHub repo-র রুটে (বা `assets/` ফোল্ডারে) এই ফাইলগুলো আপলোড করে, HTML ফাইলের `<head>`-এ এই লাইনগুলো যোগ করে দিন:

```html
<link rel="icon" type="image/x-icon" href="favicon.ico">
<link rel="icon" type="image/png" sizes="32x32" href="favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png">
<link rel="manifest" href="site.webmanifest">
<meta name="theme-color" content="#e3a23a">
```

যদি ফাইলগুলো `assets/` এর মতো কোনো সাবফোল্ডারে রাখেন, তাহলে `href="favicon.ico"` কে `href="assets/favicon.ico"` — এভাবে path বদলে দিতে হবে।

## ফাইল লিস্ট
- `favicon.ico` — ব্রাউজার ট্যাব আইকন (16/32/48/64px)
- `favicon-16x16.png`, `favicon-32x32.png` — ছোট সাইজ আইকন
- `apple-touch-icon.png` (180x180) — আইফোনে হোমস্ক্রিনে যোগ করলে
- `android-chrome-192x192.png`, `android-chrome-512x512.png` — অ্যান্ড্রয়েড / PWA আইকন
- `site.webmanifest` — PWA ম্যানিফেস্ট, `android-chrome-*` আইকনগুলো এখানে রেফারেন্স করা আছে
