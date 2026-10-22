<div align="center">
<svg xmlns="http://www.w3.org/2000/svg" width="1200" height="340" viewBox="0 0 1200 340">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#0D0221"/>
      <stop offset="0.55" stop-color="#1A0B3B"/>
      <stop offset="1" stop-color="#2A0F3F"/>
    </linearGradient>
    <linearGradient id="name" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0" stop-color="#A78BFA">
        <animate attributeName="stop-color" values="#A78BFA;#F472B6;#F59E0B;#A78BFA" dur="6s" repeatCount="indefinite"/>
      </stop>
      <stop offset="1" stop-color="#F472B6">
        <animate attributeName="stop-color" values="#F472B6;#F59E0B;#A78BFA;#F472B6" dur="6s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    <linearGradient id="screen" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0" stop-color="#7C3AED"/>
      <stop offset="1" stop-color="#F472B6"/>
    </linearGradient>
    <linearGradient id="bar" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0" stop-color="#7C3AED"/>
      <stop offset="0.5" stop-color="#F472B6"/>
      <stop offset="1" stop-color="#F59E0B"/>
    </linearGradient>
    <radialGradient id="glow" cx="0.5" cy="0.5" r="0.5">
      <stop offset="0" stop-color="#7C3AED" stop-opacity="0.55"/>
      <stop offset="1" stop-color="#7C3AED" stop-opacity="0"/>
    </radialGradient>
    <clipPath id="clip"><rect width="1200" height="340" rx="24"/></clipPath>
  </defs>

  <style>
    .sans{font-family:'Segoe UI',Ubuntu,'Helvetica Neue',Arial,sans-serif}
    .mono{font-family:'JetBrains Mono',Consolas,'Courier New',monospace}
    .star{animation:tw 3s ease-in-out infinite}
    @keyframes tw{0%,100%{opacity:.15}50%{opacity:1}}
    .in{opacity:0;animation:up .9s ease forwards}
    @keyframes up{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:translateY(0)}}
    .float{animation:fl 5s ease-in-out infinite}
    @keyframes fl{0%,100%{transform:translateY(0)}50%{transform:translateY(-10px)}}
    .blink{animation:bl 1s steps(1) infinite}
    @keyframes bl{50%{opacity:0}}
    .pulse{animation:pu 1.8s ease-out infinite;transform-origin:center;transform-box:fill-box}
    @keyframes pu{0%{transform:scale(1);opacity:.8}100%{transform:scale(3);opacity:0}}
    .load{animation:ld 2.4s ease-in-out infinite;transform-origin:left;transform-box:fill-box}
    @keyframes ld{0%{transform:scaleX(.15)}60%,100%{transform:scaleX(1)}}
  </style>

  <g clip-path="url(#clip)">
    <rect width="1200" height="340" fill="url(#bg)"/>

    <!-- stars -->
    <g fill="#E9D5FF">
      <circle class="star" cx="60" cy="40" r="1.6"/>
      <circle class="star" cx="180" cy="300" r="1.2" style="animation-delay:.4s"/>
      <circle class="star" cx="320" cy="28" r="1.4" style="animation-delay:1.1s"/>
      <circle class="star" cx="540" cy="310" r="1.8" style="animation-delay:.7s"/>
      <circle class="star" cx="610" cy="50" r="1.2" style="animation-delay:1.6s"/>
      <circle class="star" cx="700" cy="290" r="1.5" style="animation-delay:.2s"/>
      <circle class="star" cx="1150" cy="40" r="1.6" style="animation-delay:1.3s"/>
      <circle class="star" cx="1120" cy="300" r="1.3" style="animation-delay:.9s"/>
      <circle class="star" cx="780" cy="30" r="1.1" style="animation-delay:2s"/>
      <circle class="star" cx="420" cy="300" r="1.2" style="animation-delay:2.4s"/>
      <circle class="star" cx="30" cy="200" r="1.4" style="animation-delay:1.8s"/>
      <circle class="star" cx="1180" cy="170" r="1.2" style="animation-delay:.5s"/>
    </g>

    <!-- glow + orbits -->
    <circle cx="930" cy="170" r="190" fill="url(#glow)"/>
    <g fill="none" stroke="#A78BFA" stroke-opacity="0.35">
      <circle cx="930" cy="170" r="85" stroke-dasharray="4 8">
        <animateTransform attributeName="transform" type="rotate" from="0 930 170" to="360 930 170" dur="30s" repeatCount="indefinite"/>
      </circle>
      <circle cx="930" cy="170" r="125" stroke-dasharray="2 10">
        <animateTransform attributeName="transform" type="rotate" from="360 930 170" to="0 930 170" dur="45s" repeatCount="indefinite"/>
      </circle>
      <circle cx="930" cy="170" r="160" stroke-opacity="0.18"/>
    </g>

    <!-- orbiting dots -->
    <g>
      <animateTransform attributeName="transform" type="rotate" from="0 930 170" to="360 930 170" dur="8s" repeatCount="indefinite"/>
      <circle cx="1015" cy="170" r="6" fill="#F472B6"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="rotate" from="120 930 170" to="-240 930 170" dur="12s" repeatCount="indefinite"/>
      <circle cx="1055" cy="170" r="5" fill="#F59E0B"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="rotate" from="200 930 170" to="560 930 170" dur="16s" repeatCount="indefinite"/>
      <circle cx="1090" cy="170" r="4" fill="#A78BFA"/>
    </g>

    <!-- phone -->
    <g class="float">
      <rect x="880" y="80" width="100" height="180" rx="18" fill="#0D0221" stroke="#A78BFA" stroke-width="2"/>
      <rect x="889" y="92" width="82" height="156" rx="11" fill="#150733"/>
      <rect x="914" y="96" width="32" height="5" rx="2.5" fill="#2A0F3F"/>
      <rect x="897" y="110" width="66" height="44" rx="8" fill="url(#screen)" opacity="0.9"/>
      <rect x="897" y="162" width="66" height="7" rx="3.5" fill="url(#bar)" class="load"/>
      <rect x="897" y="176" width="46" height="6" rx="3" fill="#4C1D95"/>
      <rect x="897" y="190" width="30" height="30" rx="7" fill="#2E1065"/>
      <rect x="933" y="190" width="30" height="30" rx="7" fill="#2E1065"/>
      <rect x="897" y="228" width="66" height="12" rx="6" fill="#F472B6" opacity="0.85"/>
    </g>

    <!-- floating tech pills -->
    <g class="sans" font-size="13" font-weight="600">
      <g class="float" style="animation-delay:.3s">
        <rect x="760" y="70" width="78" height="28" rx="14" fill="#1E0B45" stroke="#7C3AED"/>
        <text x="799" y="89" text-anchor="middle" fill="#C4B5FD">Flutter</text>
      </g>
      <g class="float" style="animation-delay:1.2s">
        <rect x="1030" y="62" width="112" height="28" rx="14" fill="#1E0B45" stroke="#F472B6"/>
        <text x="1086" y="81" text-anchor="middle" fill="#FBCFE8">React Native</text>
      </g>
      <g class="float" style="animation-delay:2s">
        <rect x="740" y="240" width="80" height="28" rx="14" fill="#1E0B45" stroke="#F59E0B"/>
        <text x="780" y="259" text-anchor="middle" fill="#FDE68A">Next.js</text>
      </g>
      <g class="float" style="animation-delay:.8s">
        <rect x="1045" y="250" width="90" height="28" rx="14" fill="#1E0B45" stroke="#F59E0B"/>
        <text x="1090" y="269" text-anchor="middle" fill="#FDE68A">Firebase</text>
      </g>
      <g class="float" style="animation-delay:1.6s">
        <rect x="1080" y="156" width="92" height="28" rx="14" fill="#1E0B45" stroke="#7C3AED"/>
        <text x="1126" y="175" text-anchor="middle" fill="#C4B5FD">Supabase</text>
      </g>
    </g>

    <!-- left text -->
    <g class="in" style="animation-delay:.1s">
      <text x="70" y="98" class="mono" font-size="20" fill="#F472B6">&gt; hello world, I'm<tspan class="blink" fill="#F59E0B"> _</tspan></text>
    </g>
    <g class="in" style="animation-delay:.4s">
      <text x="66" y="168" class="sans" font-size="66" font-weight="800" letter-spacing="2" fill="url(#name)">SARFARAZ ALAM</text>
    </g>
    <g class="in" style="animation-delay:.7s">
      <text x="70" y="210" class="sans" font-size="25" font-weight="600" fill="#E9D5FF">Cross-Platform App Developer</text>
    </g>
    <g class="in" style="animation-delay:1s">
      <text x="70" y="244" class="mono" font-size="15" fill="#A1A1C2">Android · iOS · Web  —  Flutter · React Native · Next.js</text>
    </g>
    <g class="in" style="animation-delay:1.3s">
      <rect x="70" y="266" width="300" height="34" rx="17" fill="#14532D" fill-opacity="0.35" stroke="#22C55E" stroke-opacity="0.6"/>
      <circle cx="92" cy="283" r="5" fill="#22C55E" class="pulse"/>
      <circle cx="92" cy="283" r="5" fill="#22C55E"/>
      <text x="106" y="288" class="sans" font-size="14" font-weight="600" fill="#BBF7D0">Open for freelance &amp; full-time</text>
    </g>

    <!-- bottom animated line -->
    <rect x="0" y="334" width="1200" height="6" fill="url(#bar)" opacity="0.9">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/>
    </rect>
  </g>
</svg>

<img src="https://capsule-render.vercel.app/api?type=venom&height=260&color=0:0D0221,50:7C3AED,100:F472B6&text=SARFARAZ%20ALAM&fontColor=FFFFFF&fontSize=60&fontAlignY=42&desc=Cross-Platform%20App%20Developer%20%E2%80%A2%20Android%20%E2%80%A2%20iOS%20%E2%80%A2%20Web&descAlignY=64&descSize=18&animation=twinkling&stroke=F59E0B&strokeWidth=1" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=2800&pause=900&color=F472B6&center=true&vCenter=true&width=760&lines=I+build+apps+for+Android+%2B+iOS+%2B+Web;Flutter+%26+Dart+%E2%80%94+pixel-perfect+UI;React+Native+%2B+Next.js+%E2%80%94+every+screen;Firebase+%C2%B7+Supabase+%C2%B7+Cloudinary+backends;From+Postman+tests+to+live+on+GoDaddy+%F0%9F%9A%80" />

<br/>

<a href="https://www.linkedin.com/in/sarfaraj-alam-536b51291/"><img src="https://img.shields.io/badge/LinkedIn-1A0B3B?style=for-the-badge&logo=linkedin&logoColor=F472B6"/></a>
<a href="mailto:sarfarajbabu748@gmail.com"><img src="https://img.shields.io/badge/Hire%20Me-1A0B3B?style=for-the-badge&logo=gmail&logoColor=F59E0B"/></a>
<a href="https://pub.dev/packages/taplatch"><img src="https://img.shields.io/badge/pub.dev-1A0B3B?style=for-the-badge&logo=dart&logoColor=A78BFA"/></a>
<img src="https://komarev.com/ghpvc/?username=thesarfaraj9794&label=VISITORS&color=7C3AED&style=for-the-badge"/>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 👨‍💻 About Me

```dart
class SarfarazAlam extends Developer {
  final role      = 'Cross-Platform App Developer';
  final location  = 'India 🇮🇳';
  final platforms = ['Android', 'iOS', 'Web'];

  final frontend  = ['Flutter', 'Dart', 'React Native', 'Next.js'];
  final backend   = ['Firebase', 'Supabase', 'Cloud Functions', 'Cloudinary'];
  final apis      = ['REST APIs', 'Postman Testing', 'Third-party Integrations'];
  final shipping  = ['Firebase Hosting', 'GoDaddy Domains', 'Play Store', 'App Store'];

  String get motto => 'Idea ➜ Design ➜ Code ➜ Test ➜ Live 🚀';
}
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## ⚙️ How I Ship a Product

<div align="center">

| 🎨 **Design** | 💻 **Build** | 🧪 **Integrate & Test** | 🚀 **Deploy** |
|:---:|:---:|:---:|:---:|
| Figma · UI/UX | Flutter · React Native · Next.js | REST APIs · Postman | Firebase Hosting · GoDaddy |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧰 Tech Arsenal

<div align="center">

**📱 App Development**<br/><br/>
<img src="https://skillicons.dev/icons?i=flutter,dart,react,nextjs,ts,js&theme=dark&perline=6"/>

<br/><br/>

**☁️ Backend & Cloud**<br/><br/>
<img src="https://skillicons.dev/icons?i=firebase,supabase,nodejs,mongodb,mysql&theme=dark&perline=5"/>
<br/>
<img src="https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white"/>
<img src="https://img.shields.io/badge/Cloud%20Functions-FFCA28?style=for-the-badge&logo=firebase&logoColor=black"/>
<img src="https://img.shields.io/badge/Firestore-FF6F00?style=for-the-badge&logo=firebase&logoColor=white"/>

<br/><br/>

**🔗 APIs, Testing & Hosting**<br/><br/>
<img src="https://skillicons.dev/icons?i=postman,git,github,vercel&theme=dark&perline=4"/>
<br/>
<img src="https://img.shields.io/badge/REST%20APIs-7C3AED?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Firebase%20Hosting-DD2C00?style=for-the-badge&logo=firebase&logoColor=white"/>
<img src="https://img.shields.io/badge/GoDaddy-1BDBDB?style=for-the-badge&logo=godaddy&logoColor=black"/>

<br/><br/>

**📲 Platforms & Tools**<br/><br/>
<img src="https://skillicons.dev/icons?i=androidstudio,apple,vscode,figma&theme=dark&perline=4"/>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🏥 Restore Health Services
**Healthcare Marketplace**

Medicines, blood tests, doctor consultation and health services in one app.

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![REST API](https://img.shields.io/badge/REST_API-7C3AED?style=flat-square)

</td>
<td width="50%" valign="top">

### 🚗 Sampark
**QR Vehicle Communication**

Contact any vehicle owner by scanning a QR, without sharing personal numbers.

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛣️ RoadPulse
**Smart Road Safety Platform**

Report and track potholes, speed breakers and road hazards on a live map.

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Maps](https://img.shields.io/badge/Google_Maps-4285F4?style=flat-square&logo=googlemaps&logoColor=white)
![Dashboard](https://img.shields.io/badge/Dashboard-F472B6?style=flat-square)

</td>
<td width="50%" valign="top">

### 🧠 BrainBoost
**Offline Education App**

Offline lessons and MCQ practice for students, no internet needed.

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)
![Offline](https://img.shields.io/badge/Offline_First-F59E0B?style=flat-square)

</td>
</tr>
<tr>
<td colspan="2" valign="top" align="center">

### 🔗 TapLatch — Open-Source Flutter Package
Prevents accidental double-taps, with loading, success and cooldown states.

<a href="https://pub.dev/packages/taplatch"><img src="https://img.shields.io/pub/v/taplatch?style=for-the-badge&logo=dart&color=7C3AED&label=pub.dev"/></a>
<a href="https://pub.dev/packages/taplatch"><img src="https://img.shields.io/pub/likes/taplatch?style=for-the-badge&color=F472B6"/></a>

</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=thesarfaraj9794&show_icons=true&hide_border=true&bg_color=0D0221&title_color=F472B6&icon_color=A78BFA&text_color=E9D5FF&ring_color=F59E0B&rank_icon=github" height="170"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=thesarfaraj9794&layout=compact&hide_border=true&bg_color=0D0221&title_color=F472B6&text_color=E9D5FF" height="170"/>

<img src="https://streak-stats.demolab.com?user=thesarfaraj9794&hide_border=true&background=0D0221&ring=F472B6&fire=F59E0B&currStreakNum=FFFFFF&sideNums=FFFFFF&currStreakLabel=F472B6&sideLabels=C4B5FD&dates=A1A1C2&stroke=2E1065" width="70%"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=thesarfaraj9794&bg_color=0D0221&color=C4B5FD&line=F472B6&point=F59E0B&area=true&area_color=7C3AED&hide_border=true&radius=12" width="100%"/>

</div>

<div align="center">

### 🤝 Let's build something together

Freelance app, startup MVP or full-time role — I'm ready.

<a href="mailto:sarfarajbabu748@gmail.com"><img src="https://img.shields.io/badge/sarfarajbabu748@gmail.com-0D0221?style=for-the-badge&logo=gmail&logoColor=F472B6"/></a>

<img src="https://capsule-render.vercel.app/api?type=waving&height=140&color=0:F472B6,50:7C3AED,100:0D0221&section=footer" width="100%"/>

</div>
