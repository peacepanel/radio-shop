# Radio Shop — GitHub Edition

واجهة ستاتيكية على GitHub Pages تقرأ المنتجات وقائمة الأغاني من Google Sheets عامة عبر واجهة GViz (بدون GAS).

## المتطلبات
- Google Sheets عامة (أو Published to the web).
- تعبئة الشيتات كما يلي.

## الشيتات
### 1) Sheet: Playlists (ضمن PLAYLISTS_SSID)
أضف ورقة باسم **Playlists** بعناوين الأعمدة بالضبط:

| period | title | src | duration |
|--------|-------|-----|----------|
| morning | Sunny Morning | https://your-domain/audio/track1.mp3 | 139 |
| day     | Energy        | https://your-domain/audio/track2.mp3 | 155 |
| night   | Calm Night    | https://your-domain/audio/track3.mp3 | 198 |

> **src** يجب أن يكون رابط MP3 مباشر. يُفضل استضافة الملفات في نفس الريبو داخل مجلد `audio/` ثم استعمال رابط GitHub Pages.

### 2) Sheet: Config (ضمن PRODUCTS_SSID)
ورقة باسم **Config**، العمود **A** يحوي أسماء أوراق المنتجات (الفئات)، سطر لكل اسم، ابتداء من **A2**.

مثال:
