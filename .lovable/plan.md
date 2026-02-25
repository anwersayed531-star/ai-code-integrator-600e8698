

# خطة إضافة API Keys لمشروع ZAS Site Translator

## الخطوة 1: ربط المشروع بـ GitHub
- هتروح إعدادات المشروع (Settings) → GitHub → Connect
- هتربط الـ repo: `anwersayed531-star/zas-site-translator`
- الكود هينزل تلقائيًا في المشروع ده

## الخطوة 2: تفعيل Supabase/Cloud
- بعد ما الكود ينزل، هنتأكد إن Supabase متربط بالمشروع
- ده ضروري عشان نقدر نخزن الـ API keys بأمان كـ secrets

## الخطوة 3: إضافة الـ 4 API Keys كـ Supabase Secrets
هنضيف الـ secrets التالية:
1. **GROQ_API_KEY** - لمزود الترجمة الأساسي (Groq Cloud)
2. **GOOGLE_AI_API_KEY** - لمزود الترجمة الثانوي (Google AI Studio)  
3. **CLOUDFLARE_ACCOUNT_ID** + **CLOUDFLARE_API_TOKEN** - لمزود الترجمة الاحتياطي (Cloudflare Workers AI)
4. **CEREBRAS_API_KEY** - لمساعد ZAS AI (الشات بوت)

## الخطوة 4: اختبار الوظائف
- اختبار ترجمة كود HTML من لغة للغة تانية
- اختبار مساعد ZAS AI (الشات بوت)
- التأكد إن الـ fallback بين المزودين شغال (Groq → Google → Cloudflare)

## ملاحظة مهمة
مش هنغير أي حاجة في الكود - بس هنضيف الـ API keys اللي المشروع محتاجها عشان يشتغل.

