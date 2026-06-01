# GitHub profile setup (2 minutes)

The iOS project repo is **not** modified. Only this profile README is added.

## 1. Create the profile repository on GitHub

1. Open https://github.com/new
2. Repository name: **`Oleksandr19942`** (must match your username exactly)
3. Visibility: **Public**
4. Check **Add a README file** — optional; you will overwrite it
5. Click **Create repository**

## 2. Push this README

```bash
cd "/Users/oleksandr.metelev/Projects/Oleksandr19942-profile"
git add README.md
git commit -m "Add GitHub profile README"
git remote add origin git@github.com:Oleksandr19942/Oleksandr19942.git
git push -u origin main
```

If `origin` already exists:

```bash
git remote set-url origin git@github.com:Oleksandr19942/Oleksandr19942.git
git push -u origin main
```

## 3. Profile settings (github.com → Settings → Profile)

| Field | Suggested value |
|-------|-----------------|
| **Name** | Oleksandr Meteliev |
| **Bio** | iOS Engineer · AI health & real-time apps · SwiftUI · App Store |
| **Company** | StartupSoft (or leave blank) |
| **Location** | Ukraine |
| **Website** | https://www.linkedin.com/in/oleksandr-meteliev-b2ab46209/ |

## 4. Pin repositories

On your profile → **Customize your pins**:

- If `ios` on your account is only a mirror of private work, consider **not pinning** it or make that repo **private**
- Pin public repos that best match your resume (when available)

## Security note

If `Oleksandr19942/ios` is a full copy of the 2ndOpinion app and is **public**, review it for secrets (API keys, `AISecrets.swift`, `GoogleService-Info.plist`) and prefer a **private** repo for production code.
