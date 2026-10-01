# Faceless Shorts Automation V6

Web app untuk membuat YouTube Shorts faceless: TOPIC → AI SCRIPT → FOOTAGE → AI VOICE → SUBTITLE → RENDER MP4.

## Isi V6
- Next.js web app
- Supabase Auth + database
- OpenAI Responses API untuk script
- Pixabay video search
- OpenAI TTS
- WebVTT subtitle generator
- FFmpeg render worker untuk MP4 1080×1920

## Deploy web ke Vercel
1. Upload seluruh isi folder ini ke repository GitHub.
2. Import repository ke Vercel.
3. Tambahkan environment variables:
   - NEXT_PUBLIC_SUPABASE_URL
   - NEXT_PUBLIC_SUPABASE_ANON_KEY
   - OPENAI_API_KEY (Secret)
   - PIXABAY_API_KEY (Secret)
   - OPENAI_TEXT_MODEL=gpt-5.6
   - OPENAI_TTS_VOICE=coral
4. Deploy.

Jangan beri prefix NEXT_PUBLIC_ pada API key rahasia.

## Render worker
Vercel menangani web app, sedangkan FFmpeg sebaiknya dijalankan di worker/server terpisah. `worker/run-all.mjs` dapat menjalankan pipeline lokal/server dengan Node.js dan FFmpeg.

## Catatan lisensi
Gunakan footage yang memang diizinkan untuk digunakan kembali dan selalu periksa ketentuan lisensi sumber sebelum publikasi.
