# Bozor Savati

Toshkent bozor narxlari asosida byudjetingizga mos **oziq-ovqat hamda gigiyena va tozalik** savatini tuzib beradigan veb-platforma.

Byudjetni (masalan, 1 000 000 so'm), muddatni va oila tarkibini kiritasiz. Platforma 87 ta mahsulot ichidan eng arzon va to'yimli xarid ro'yxatini tuzadi.

## Imkoniyatlar

- **Savat tuzish:** byudjet, muddat (1 hafta, 2 hafta, 1 oy), oila tarkibi va savat turi (Tejamkor, Muvozanatli, Sog'lom) bo'yicha avtomatik taklif.
- **Savat tarkibi:** hammasi, faqat oziq-ovqat yoki faqat gigiyena va tozalik.
- **Kunma-kun xarid rejasi:** har kuni nima va qancha olish, limit nazorati, haqiqiy xarajatni kiritish.
- **Taomnoma:** savatdagi mahsulotlardan har kunlik nonushta, tushlik va kechki ovqat uchun o'zbek taomlari.
- **Savatni tahrirlash:** sudrab tartiblash, katalogdan qo'shish, almashtirish, o'zgarishlar tarixi va bekor qilish.
- **So'z va ovoz bilan boshqarish:** "piyoz kerak emas", "piyozni 18 kilo qil", "turp o'rniga nima bor?", "faqat oziq-ovqat". O'zbekcha (lotin va kirill) hamda ruscha tushuniladi.
- **"Nega shuncha?" izohlari:** har bir mahsulot miqdori qanday hisoblangani.
- **Mavsumiy maslahatlar:** narx prognozi va almashtirish takliflari.
- **Narx tarixi grafigi:** ochiq manbalardagi va siz yozgan narxlar.
- **Chek kiritish:** rasm yoki matn orqali. Avtomatik o'qish faqat claude.ai ichida ishlaydi.
- **Bozorlar solishtiruvi:** Toshkentdagi 15 ta bozor va supermarket tarmoqlari. Joylashuvingizga qarab masofa, yo'l narxi va eng foydali joy ko'rsatiladi.

## Ishga tushirish

Platforma bitta HTML faylidan iborat, o'rnatish talab qilinmaydi:

1. `index.html` faylini brauzerda oching, yoki
2. GitHub Pages'ni yoqing: Settings → Pages → Branch: `main` / root.

Kiritgan ma'lumotlaringiz (narxlar, tahrirlar, xarajatlar) faqat sizning brauzeringizda (`localStorage`) saqlanadi.

## Fayllar

| Fayl | Tavsif |
|---|---|
| `index.html` | Platformaning o'zi: HTML, CSS va JavaScript bitta faylda |
| `img/` | 87 ta mahsulot rasmi (PNG, 256×256, shaffof fon) |
| `Toshkent_oziq_ovqat_narxlari_va_oylik_byudjet.xlsx` | Narxlar jadvali, oylik byudjet kalkulyatori va tahlil |

## Cheklovlar

- Narxlar **taxminiy** (oktyabr 2026) va ochiq manbalar asosida hisoblangan: Kun.uz, Zamin.uz, PUL24, Daryo.uz (Numbeo), Vaqt.uz, Anhor.uz, Stat.uz. Bozor va do'konga qarab ±10–15% farq bo'lishi tabiiy.
- Bozorlar joylashuvi, narx darajalari va mavsumiy prognoz taxminiy model asosida.
- Supermarket filiallari ro'yxati to'liq emas, to'liq ro'yxat uchun 2GIS'ga havola berilgan.
- Chekni rasmdan o'qish, manzil qidirish va murakkab savollar uchun Claude kerak. Bu imkoniyatlar faqat platforma claude.ai'da ochilganda ishlaydi, GitHub Pages'da esa yashiriladi.
- Ovozli kiritish brauzerning nutqni tanish funksiyasidan foydalanadi (o'zbek tili Chrome'da). Ishlamasa, qurilma klaviaturasining diktovkasi bilan gapiring.

## Kutubxonalar

- [SortableJS](https://github.com/SortableJS/Sortable) 1.15.0: sudrab tartiblash uchun.
- Google Fonts: Unbounded, Onest, IBM Plex Mono.
