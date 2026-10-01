# Deploy Online V6

## GitHub
Upload **isi folder project**, bukan file ZIP dan bukan folder induk tambahan. Di repository, `package.json`, `app/`, `lib/`, dan `worker/` harus berada di root.

## Vercel
Import repository tersebut sebagai project Next.js. Setelah project dibuat, buka Settings → Environment Variables dan masukkan nilai dari Supabase serta API keys.

Untuk API key rahasia, gunakan Secret/environment variable server-side dan jangan menggunakan nama `NEXT_PUBLIC_*`.

## Setelah deploy
Buka URL `.vercel.app`, login dengan akun Supabase, lalu buat project Shorts.
