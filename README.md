# 🎙️ Dubber Studio (Web Edition)

> **Web Voice Cloning & AI Dubbing Platform**  
> បំប្លែងពីកម្មវិធីកុំព្យូទ័រទៅជា Web Version ដំណើរការផ្ទាល់លើ Browser និងអាច Deploy ទៅកាន់ GitHub Pages បានភ្លាមៗ!

![Dubber Studio Banner](./assets/cover-studio-C1LkVHMJ.png)

---

## 🌟 អំពី Dubber Studio (Overview)

**Dubber Studio** គឺជាកំណែ Web Version ពេញលេញដែលត្រូវបានបំប្លែងចេញពីកម្មវិធី **Dubber បីសាច [ Clone សម្លេង Pro ].exe**។ កំណែ Web នេះដំណើរការដោយផ្ទាល់នៅលើ Browser (Client-side) ដោយមិនចាំបាច់មាន Backend Server ស្មុគស្មាញឡើយ ហើយអាចបង្ហោះ (Hosting) ដោយផ្ទាល់នៅលើ **GitHub Pages** បានដោយឥតគិតថ្លៃ ១០០%។

---

## ✨ លក្ខណៈពិសេសចម្បង (Key Features)

1. **Standalone Web Application (Zero Server Dependency)**:
   - ដំណើរការនៅលើ Browser គ្រប់ប្រភេទ (Chrome, Edge, Firefox, Safari, Brave)
   - គ្មានបញ្ហា License ចាក់សោរ (Permanent Lifetime Pro License Unlocked)
2. **33 Bundled Cloned Voice Profiles (កាតាឡុកសម្លេង ៣៣ តួអង្គ)**:
   - រួមបញ្ចូលសម្លេងគំរូដូចជា: *Male 1, Female 1, Toddler, Princess, Aunt, Old Woman, Calm Man, Confident Man, តួ ព្រះនាង, ព្រះនាងធំ, យាយចាស់, អាម៉ាត, អ្នកបម្រើប្រុស...*
   - អាចបន្ថែម និង Upload Voice Profile ផ្ទាល់ខ្លួនបាន
3. **Multi-Engine Voice Synthesis**:
   - **Microsoft Edge TTS**: សម្លេងច្បាស់ល្អកម្រិតខ្ពស់
   - **Google Translate Khmer TTS Engine**: គាំទ្រការបញ្ចេញសម្លេងភាសាខ្មែរបានយ៉ាងត្រឹមត្រូវ
   - **Web Speech API**: ដំណើរការ Offline ដោយស្វ័យប្រវត្តិនៅលើឧបករណ៍
4. **Interactive Timeline & Audio Waveform**:
   - បង្ហាញ Waveform នៃសម្លេងតាមរយៈ **Web Audio API**
   - អាចកាត់ត (Cut/Trim), Split, និងកំណត់ពេលវេលា Subtitle បានយ៉ាងលម្អិត
5. **Subtitle Import & Export**:
   - គាំទ្រ Format `.srt`, `.vtt`, `.txt`
   - បកប្រែភាសា និង Dub សម្លេងស្វ័យប្រវត្តិតាមជួរនីមួយៗ
6. **Cover Studio (Thumbnail & 3D Title Creator)**:
   - ឧបករណ៍រចនា Poster / Thumbnail និងអក្សរ 3D Title
   - រួមបញ្ចូល 179+ Graphic Assets, Mascots, Patterns និង Stickers

---

## 🚀 របៀបបើកដំណើរការលើម៉ាស៊ីនផ្ទាល់ (Run Locally)

### ជម្រើសទី ១: ប្រើ Node.js (ណែនាំ)
```bash
# ចូលទៅកាន់ Folder គម្រោង
cd Dubber-Bisach-Web

# បើកដំណើរការ Web Server
npm start
# ឬ
node test_server.js
```
បន្ទាប់មកបើក Browser ហើយចូលទៅកាន់: **`http://localhost:8080`**

### ជម្រើសទី ២: ប្រើ Python HTTP Server
```bash
python -m http.server 8080
```

---

## 🌐 របៀប Deploy និង Hosting ទៅកាន់ GitHub Pages ដោយផ្ទាល់ (Direct GitHub Pages Deployment)

គម្រោងនេះត្រូវបានរៀបចំរួចជាស្រេចនូវ **GitHub Actions Workflow** នៅក្នុង `.github/workflows/deploy.yml` និងឯកសារ `.nojekyll`។

### ជំហានទី ១: បង្កើត GitHub Repository ថ្មី
1. ចូលទៅកាន់ [github.com/new](https://github.com/new)
2. ដាក់ឈ្មោះ Repository របស់អ្នក (ឧទាហរណ៍: `dubber-studio`)
3. ជ្រើសរើស **Public** រួចចុច **Create repository**

### ជំហានទី ២: Push កូដទាំងអស់ទៅកាន់ GitHub
បើក Terminal នៅក្នុង Folder `Dubber-Bisach-Web` រួចវាយពាក្យបញ្ជាខាងក្រោម:

```bash
git init
git add .
git commit -m "Initial release of Dubber Studio Web"
git branch -M main
git remote add origin https://github.com/<YOUR-USERNAME>/<YOUR-REPO-NAME>.git
git push -u origin main
```

### ជំហានទី ៣: បើកដំណើរការ GitHub Pages
1. ចូលទៅកាន់ **Settings** នៃ Repository របស់អ្នកនៅលើ GitHub
2. នៅ Menu ខាងឆ្វេង ចុចលើ **Pages**
3. នៅក្រោម **Build and deployment > Source**:
   - ជ្រើសរើស **GitHub Actions** (Workflow នឹង Deploy ដោយស្វ័យប្រវត្តិនៅរាល់ពេល push កូដ)
   - *ឬ* ជ្រើសរើស **Deploy from a branch** > ជ្រើសរើស `main` branch និង `/ (root)` folder រួចចុច **Save**
4. រង់ចាំប្រហែល ១ នាទី អ្នកនឹងទទួលបាន Link គេហទំព័រផ្ទាល់ខ្លួន:  
   👉 **`https://<YOUR-USERNAME>.github.io/<YOUR-REPO-NAME>/`**

---

## 📂 រចនាសម្ព័ន្ធឯកសារ (Project Structure)

```text
Dubber-Bisach-Web/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions deployment automation
├── assets/                     # UI components, React bundle, mascots, icons
│   ├── index-Bs5qzE0C.js       # App logic (Branded to Dubber Studio)
│   ├── index-BQmrldh6.css      # Modern Glassmorphism Styling
│   └── *.png                   # 179+ Graphic assets and mascots
├── voice-profiles/             # 33 Cloned Voice Audio Samples & Metadata
│   ├── index.json              # Voice catalog definition
│   └── *.wav / *.mp3           # Audio reference models
├── khmer-fonts/                # Stylized Khmer Typography
├── avatars/                    # Avatar presets
├── logos/                      # Logos and brand graphics
├── background-music/           # Ambient background tracks
├── desktop-web-bridge.js       # Complete Client-side Desktop IPC Bridge & TTS
├── index.html                  # Modern entrypoint with Dubber Studio branding
├── test_server.js              # Lightweight local HTTP server
├── package.json                # Project configuration and scripts
├── .nojekyll                   # GitHub Pages bypass marker
└── README.md                   # Full documentation in Khmer & English
```

---

## 📄 អាជ្ញាប័ណ្ណ (License)

Dubber Studio Web Edition ត្រូវបានចេញផ្សាយក្រោមអាជ្ញាប័ណ្ណ **MIT License**។
