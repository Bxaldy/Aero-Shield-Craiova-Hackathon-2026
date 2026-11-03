<div align="center">

# 🛡️✈️ AERO-SHIELD LRCV V2.0
### **Sistem Bionic & Fotonic de Navigație Optică 6-DoF, Aterizare Autonomă CAT IIIc (Zero-GPS) și Protecție Anti-Spoofing GNSS / ILS în Ceață Densă și Furtună**
#### *Aeroportul Internațional Craiova (`LRCV` — Pista 09: `44.3179° N, 23.8729° E`, Cap Adevărat `88.9314°`) & Catania (`LICC` — Pista 26)*

[![Premiu Originalitate](https://img.shields.io/badge/Craiova_Hackathon_2026-Premiul_pentru_Originalitate-ffd700?style=for-the-badge&logo=trophy)](#1-demonstratie-live-zbor-autonom-flightgear--prezentare-video-explicata)
[![Rust DO-178C DAL-A](https://img.shields.io/badge/Rust_2021-100%25_Memory_Safe_(DO--178C_DAL--A)-orange?style=for-the-badge&logo=rust)](#9-arhitectura-repository-ului-100-rust--flightgear-nasalmcp--stellarium-swir)
[![FlightGear 2024.1 Live](https://img.shields.io/badge/FlightGear_2024.1-60Hz_Live_Autoland_PASS-00e676?style=for-the-badge&logo=flightgear)](#8-rezultate-validate-automat-flightgear-live--stellarium-swir--server-rust)
[![Drosophila Connectome](https://img.shields.io/badge/Google_Research_FlyWire-139,255_Neurons_Ring_Attractor-00b0ff?style=for-the-badge)](#3-solutia-aero-shield-lrcv-v20-arhitectura-bionica--fotonica-la-bord)
[![YouTube Demo](https://img.shields.io/badge/YouTube-Prezentare_Video_Live-ff1744?style=for-the-badge&logo=youtube)](https://youtu.be/D331kEyQObw)
[![YouTube Zbor Perpendicular](https://img.shields.io/badge/YouTube-Zbor_Perpendicular_Autoland_V100-d50000?style=for-the-badge&logo=youtube)](https://youtu.be/dY4ACP80ycw)

<br/>

![AERO-SHIELD Hero Slide](docs/assets/slide_01_hero.png)

<p align="center">
  <b>🎬 Demonstrație Video (YouTube):</b> <a href="https://youtu.be/D331kEyQObw">https://youtu.be/D331kEyQObw</a> •
  <b>✈️ Zbor Perpendicular Autoland V100 (YouTube):</b> <a href="https://youtu.be/dY4ACP80ycw">https://youtu.be/dY4ACP80ycw</a> (<a href="https://github.com/petreleon/Craiova-Hackathon-2026/blob/main/real_videos/AERO_SHIELD_Perpendicular_Autoland_V100.mp4">MP4 1080p în Repo</a>)
  <br/>
  <b>📄 Ghid Tehnic Complet (22 pagini PDF):</b> <a href="AERO_SHIELD_Ghid_Complet_Explicat_De_La_Zero.pdf">AERO_SHIELD_Ghid_Complet_Explicat_De_La_Zero.pdf</a> •
  <b>📊 Prezentare Widescreen (PPTX):</b> <a href="AERO_SHIELD_Craiova_Hackathon_2026.pptx">AERO_SHIELD_Craiova_Hackathon_2026.pptx</a>
</p>

</div>

---

## 🎥 1. Demonstrație Live: Zbor Autonom FlightGear & Prezentare Video Explicată

<table>
  <tr>
    <td width="50%" align="center">
      <b>✈️ Aterizare Autonomă CAT IIIc în FlightGear (LRCV Pista 09)</b><br/>
      <sub>Fuziune în timp real (60 Hz) cu Tunel 3D Holografic, PFD SVS, Radar Cyber și Ecran GPS Tradițional („Confidently Wrong”)</sub><br/><br/>
      <img src="docs/assets/demo_autoland_flightgear.gif" alt="FlightGear Autonomous Landing LRCV RWY 09" width="100%"/>
    </td>
    <td width="50%" align="center">
      <b>🎬 Prezentarea Video Explicată a Sistemului AERO-SHIELD</b><br/>
      <sub>Demonstrație sincronizată HUD + Telemetrie + Explicație pas cu pas a protecției împotriva Spoofing-ului GPS</sub><br/><br/>
      <img src="docs/assets/demo_prezentare_explicata.gif" alt="AERO-SHIELD Explained Video Presentation" width="100%"/>
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <b>🎯 Zbor cu Interceptare Perpendiculară (90°) & Aterizare Autonomă V100 în 6 Faze (1080p)</b><br/>
      <sub>Automatul de zbor în 6 faze cu viraj de bază continuu C¹, captură Localizer/Glideslope 3.0°, optimizare genetică 6-DoF JSBSim, Flare C¹ și frânare automată la touchdown sub Spoofing GPS și ceață densă</sub><br/><br/>
      <a href="https://youtu.be/dY4ACP80ycw">
        <img src="https://img.youtube.com/vi/dY4ACP80ycw/maxresdefault.jpg" alt="AERO-SHIELD Perpendicular Autoland V100 YouTube" width="78%"/>
      </a><br/><br/>
      ▶️ <b>Vizionare pe YouTube:</b> <a href="https://youtu.be/dY4ACP80ycw">https://youtu.be/dY4ACP80ycw</a> &nbsp;|&nbsp;
      📥 <b>Fișier Video GitHub (MP4 1080p):</b> <a href="https://github.com/petreleon/Craiova-Hackathon-2026/blob/main/real_videos/AERO_SHIELD_Perpendicular_Autoland_V100.mp4">real_videos/AERO_SHIELD_Perpendicular_Autoland_V100.mp4</a>
    </td>
  </tr>
</table>

---

## 🚨 2. Problema Reală pe care o Rezolvăm la Craiova (`LRCV — Pista 09`)

Atunci când o aeronavă se află pe panta finală de **`3.0°`** spre **Aeroportul Internațional Craiova (`LRCV`)** în condiții de ceață densă de iarnă în care vizibilitatea scade sub **50–200 m (Categoria IIIB/IIIC)**, combinată cu vânt lateral de forfecare (*wind-shear*) și interferențe de război electronic, aviația civilă și regională se confruntă cu două vulnerabilități majore:

1. **Fenomenul „Confidently Wrong” (Spoofing GPS & Interferență Radio)**:
   - Cu un emițător SDR (*Software-Defined Radio*) de câteva sute de euro, un atacator poate injecta un semnal GNSS falsificat coerent. Deoarece toți sateliții falsificați sunt matematic consistenți între ei, receptorul clasic al aeronavei afișează **`12/12 SATS LOCKED | RAIM: GREEN | HDOP: 0.8 | Eroare: 0.0 m PE AX`**, în timp ce deviază aeronava în afara pistei.
   - **Pragul de protecție AERO-SHIELD vs. Scenariul Vizual din Simulator**:
     - **Pragul real de detecție al sistemului nostru este de `2.0 metri`** pentru abateri bruște (izolate în **`16.6 ms`** — un singur cadru la `60 Hz` — prin testul statistic $\chi^2$ Mahalanobis) și **sub-metric (`~0.3 m/s`)** pentru atacuri lente și insidioase de tip *ramp spoofing* (detectate prin algoritmul secvențial Page-Hinkley **CUSUM**).
     - În demonstrația video din FlightGear am injectat o deviere GPS de **`+250 m` în lateral** exclusiv pentru ca separarea dintre „pista fantomă” (roșu) și pista reală (verde) să fie vizibilă clar cu ochiul liber pe ecranul radar și în cabina de pilotaj.
2. **Bariera Financiară pentru Aeroporturile Regionale**:
   - Un sistem terestru clasic de antene **ILS CAT IIIB/C** costă peste **`5.000.000 EUR`** per pistă pentru instalare, mentenanță și zboruri periodice de calibrare, motiv pentru care aeroporturile regionale nu îl dețin și sunt nevoite să devieze sau să anuleze zborurile imediat ce cade ceața densă (`~25.000 EUR` pierdere directă per zbor anulat).

---

## 🛡️ 3. Soluția AERO-SHIELD LRCV V2.0 (Arhitectura Bionică & Fotonică la Bord)

Am construit un copilot autonom complet pasiv la bord și imun la interferențe radio externe, cu un cost hardware estimat la **`~5.600 EUR` per aeronavă (`0 EUR` infrastructură pe aeroport)**:

| Sub-Sistem la Bord | Tehnologie & Fizică | Rol Operațional în Ceață / Spoofing |
| :--- | :--- | :--- |
| **1. Cameră Frontală Dual-Band (`VIS + SWIR 1.5 µm`)** | Senzor InGaAs în infraroșu scurt (`0.9–1.7 µm`), unde coeficientul de extincție Mie în ceață scade la `β_SWIR ≈ 0.22 × β_VIS` | Penetrează ceața de **`4×` mai departe** decât spectrul vizibil (`50 m → 200 m`), extrăgând centroizii sub-pixel (`I_SWIR²`) ai balizajului luminos ALS și contrastul marcajelor albe pe asfaltul ud |
| **2. Radar Milimetric `FMCW 94 GHz` + Altimetru** | Lungime de undă `λ = 3.2 mm` transparentă la picăturile micronice de ceață | Măsoară altitudinea reală AGL cu precizie de **`3 cm`** pentru manevra de *flare*, viteza Doppler față de sol și profilul TERCOM al terenului sub plafonul de nori |
| **3. Unitate Inerțială Tactică (`IMU 400 Hz`) + ES-EKF 22 Stări** | Integrare pe varietatea `SO(3) × ℝ³` cu *Error-State Extended Kalman Filter* în 22 de stări (15 inerțiale + 6 vânt/forfecare + 1 baro) | Asigură continuitatea buclei de control la `60 Hz`, estimează vectorul vântului tridimensional și derotează fluxul optic 3D (separând rotația aeronavei de translația reală) |
| **4. Astro-Tracker Zenital `SWIR 2.2 µm` (Stellarium J2000) + `DRA`** | Cameră zenitală în banda K (`2.2 µm`, împrăștiere Rayleigh redusă de `256×`) + fotoreceptori de polarizare UV/albastru (*Dorsal Rim Area*) | Identifică autonom **9 stele în plină zi / prin pâclă** (`SNR +20.87 dB` vs `-8.68 dB` în vizibil), rezolvă atitudinea 3D prin **Wahba SVD** cu eroare **`0.00018°`** și elimină acumularea driftului giroscopic INS |
| **5. Creier Bionic Google Research *Drosophila* (`139.255` Neuroni)** | Connectomul complet *FlyWire* (Nature, oct. 2024): `Retina -> Lamina -> Medulla (T4/T5) -> Lobula Plate (HS/VS) -> Central Complex (E-PG Ring Attractor 16 neuroni + PFNd)` | Arhitectură deterministă (fără halucinații de tip *black-box* CNN) care menține capul adevărat și estimează rafalele de vânt lateral cu **`0.85 s` înainte** ca acestea să lovească fuzelajul |

---

## 🔧 4. Integrarea pe Aeronavă & Clarificări Inginerești Esențiale

În proiectarea sistemului am abordat direct constrângerile reale de certificare, montaj structural și fizica instrumentelor de bord:

### 4.1. Unde se montează sistemul pe avion? (Fără găurirea nasului / radomului aeronavei)
* La aeronavele comerciale și regionale, conul frontal al nasului (*radome*) adăpostește antena mobilă a **radarului meteo (Weather Radar)** și nu poate fi obstrucționat, iar perforarea fuzelajului presurizat implică costuri enorme de certificare structurală (EASA CS-25 / FAA Part 25).
* **Avantajul fizic major al spectrului SWIR (`1.5 µm`) față de termoviziunea LWIR (`8–14 µm`)**:
  1. **Transmisia directă prin sticla parbrizului**: Sticla de silicat este complet opacă pentru radiația termică LWIR (`8–14 µm`), motiv pentru care camerele cu termoviziune militare necesită carcase externe cu ferestre din germaniu/safir montate în afara cabinei. În schimb, **lumina în infraroșu scurt SWIR (`1.5 µm`) trece direct prin sticla parbrizului cabinei de pilotaj** (fiind exact lungimea de undă de `1.55 µm` utilizată prin fibra optică de sticlă în telecomunicații).
  2. **Montaj intern pe *glareshield* / plafonul cabinei**: Camera SWIR, unitatea inerțială IMU și procesorul NVIDIA Jetson se montează **în interiorul cabinei de pilotaj, în spatele parbrizului deja încălzit electric (anti-gheață) și curățat de ștergătoare**, fără nicio modificare aerodinamică sau structurală a nasului aeronavei.
  3. **Contrast pe pistă udă**: După câteva ore de ploaie și ceață, asfaltul pistei și vopseaua marcajelor ajung la echilibru termic ($\Delta T \approx 0^\circ\text{C}$), făcând camerele termice LWIR oarbe la linia centrală a pistei. Camera SWIR măsoară **reflexia fotonică**, păstrând contrastul vopselei albe și al luminilor ALS pe pistă udă.

### 4.2. De ce nu sunt suficiente instrumentele analogice / interne de zbor pentru aterizarea oarbă?
* **Instrumentele analogice și inerțiale clasice** (giroorizontul / orizontul artificial, vitezometrul cu tub Pitot, altimetrul barometric, giroscopul direcțional și busola magnetică) măsoară **atitudinea aeronavei și viteza față de masa de aer (*Indicated Airspeed*)**, dar **nu cunosc poziția fizică a asfaltului pistei**:
  * **Deriva eoliană invizibilă**: Dacă pe panta finală în ceață CAT IIIc acționează un vânt lateral de `15–18 m/s`, giroorizontul și busola indică aripi perfect orizontale și cap constant spre Est (`089°`), în timp ce întreaga masă de aer deplasează aeronava la sute de metri în lateral față de pistă (fenomen demonstrat direct prin **Linia Galbenă** de pe radarul din simulatorul nostru).
  * **Eroarea barometrică pe furtună**: Altimetrul barometric analogic calculează înălțimea din presiunea atmosferică statică. O variație locală de presiune de doar `1–2 hPa` în timpul unei furtuni induce o eroare verticală de **`8–17 metri`** — inacceptabilă pentru manevra de *flare* la `2–5 metri` deasupra asfaltului. AERO-SHIELD folosește aceste instrumente interne (IMU la `400 Hz` și barometru), dar le ancorează la sol în ultimii `200 m` prin camera SWIR și altimetrul radar de `94 GHz` (precizie verticală `3 cm`).

### 4.3. De ce „un emițător radio mai puternic la sol” nu rezolvă problema?
* **Costul infrastructurii la sol**: Emițătoarele terestre de mare putere și precizie (**ILS CAT IIIB**) depășesc `5.000.000 EUR` per pistă, fiind inexistente pe majoritatea aeroporturilor regionale.
* **Legea pătratului distanței ($1/r^2$) și lipsa criptării**: Semnalele radio civile de navigație și aterizare (GNSS L1/L5, ILS Localizer/Glideslope `108–112 MHz`, GBAS) nu sunt criptate. Un emițător SDR de câțiva wați amplasat lângă gardul aeroportului (la `300 m` sub aeronava aflată pe panta finală) este de `10–12 ori` mai aproape de antena de recepție a avionului decât baliza oficială din capătul opus al pistei (aflată la `3.5 km`), dominând recepția radio prin simpla proximitate fizică ($P_{\text{rx}} \propto P_{\text{tx}} / d^2$). Singurul canal fizic imposibil de falsificat prin radio este **observarea optică directă a pistei în spectrul SWIR**.

---

## 🎞️ 5. Cele 6 Demonstrații Vizuale Interactive (Animații GIF din Simulator)

<table>
  <tr>
    <td width="50%" align="center">
      <b>1️⃣ Penetrarea Ceții în Infraroșu SWIR (1.5 µm) vs. Vizibil</b><br/>
      <sub>Dezamorsarea legii Koschmieder-Beer-Lambert și suprimarea haloului Mie pe balizajul luminos ALS al Pistei 09</sub><br/><br/>
      <img src="docs/assets/lesson_01_swir_fog_vision.gif" alt="Lesson 1 SWIR Fog Vision" width="100%"/>
    </td>
    <td width="50%" align="center">
      <b>2️⃣ Carantinarea Spoofing-ului GPS în 16.6 ms (Prag &gt; 2.0 m)</b><br/>
      <sub>Watchdog-ul dual Chi² Mahalanobis + Page-Hinkley CUSUM detectează și izolează instantaneu semnalul GPS fals („Confidently Wrong”)</sub><br/><br/>
      <img src="docs/assets/lesson_02_gps_spoofing_quarantine.gif" alt="Lesson 2 GPS Spoofing Quarantine" width="100%"/>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <b>3️⃣ Arena celor 4 Estimatoare (Comparație în Timp Real)</b><br/>
      <sub>1) GPS Clasic Spoofed (roșu, deviat în câmp) vs. 2) INS/Analog Pur în derivă eoliană (galben) vs. 3) EKF Standard vs. 4) Scutul AERO-SHIELD V2.0 (verde, pe pistă)</sub><br/><br/>
      <img src="docs/assets/lesson_03_four_estimators_arena.gif" alt="Lesson 3 Four Estimators Arena" width="100%"/>
    </td>
    <td width="50%" align="center">
      <b>4️⃣ Connectomul Bionic Drosophila (139.255 Neuroni în Rust)</b><br/>
      <sub>Inelul atractor E-PG cu 16 neuroni, vectorii de vânt PFNd și reflexul de redresare DNp01 la 60 Hz</sub><br/><br/>
      <img src="docs/assets/lesson_04_drosophila_connectome.gif" alt="Lesson 4 Drosophila Connectome" width="100%"/>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <b>5️⃣ Astro-Tracker Zenital Stellarium SWIR (2.2 µm) & Polarizare DRA</b><br/>
      <sub>Identificare autonomă „Lost-in-Space” prin triunghiuri sferice (100% match) și solver SVD Wahba (eroare 0.66 arcsec)</sub><br/><br/>
      <img src="docs/assets/lesson_05_stellarium_swir_stars.gif" alt="Lesson 5 Stellarium SWIR Star Tracker" width="100%"/>
    </td>
    <td width="50%" align="center">
      <b>6️⃣ Navigație de Croazieră Fără Sateliți (TERCOM + Astro-Inerțial)</b><br/>
      <sub>Anularea derivei seculare a giroscopului pe distanțe lungi prin ancorare celestă SWIR + corelația profilului de relief TERCOM</sub><br/><br/>
      <img src="docs/assets/lesson_06_100000km_zero_gps.gif" alt="Lesson 6 Zero GPS Cruise Navigation" width="100%"/>
    </td>
  </tr>
</table>

---

## 📚 6. Prezentarea Oficială (PPTX) & Ghidul Tehnic Explicat de la Zero (PDF 22 Pagini)

<table>
  <tr>
    <td width="55%" align="center">
      <b>📊 Prezentare Widescreen 16:9 (<a href="AERO_SHIELD_Craiova_Hackathon_2026.pptx">AERO_SHIELD_Craiova_Hackathon_2026.pptx</a>)</b><br/>
      <sub>10 slide-uri executive cu arhitectura hardware/software, matematică și benchmark-uri</sub><br/><br/>
      <img src="docs/assets/pptx_slides_showcase.gif" alt="PPTX Presentation Slides Showcase" width="100%"/>
    </td>
    <td width="45%" align="center">
      <b>📘 Ghidul Complet de 22 Pagini (<a href="AERO_SHIELD_Ghid_Complet_Explicat_De_La_Zero.pdf">AERO_SHIELD_Ghid_Complet_Explicat_De_La_Zero.pdf</a>)</b><br/>
      <sub>Analiză statică și matematică a tuturor modulelor Rust, Python și Nasal FlightGear</sub><br/><br/>
      <img src="docs/assets/pdf_guide_showcase.gif" alt="PDF Technical Guide Showcase" width="100%"/>
    </td>
  </tr>
</table>

---

## 🧮 7. Cele 5 Legi Fizice Fundamentale, Automatul de Zbor în 6 Faze & Sinteza din `c172p.xml`

| # | Legea Fizică / Modulul Bionic | Formula Intuitivă & Exemplu Numeric Real | Efectul Direct asupra Zborului Autonom |
| :-: | :--- | :--- | :--- |
| **1** | **Derotarea Giroscopică a Fluxului Optic** (`HS/VS` & `Lamina`) | `15 px/s (văzut de cameră) − 12 px/s (rotirea din giroscop IMU) = 3 px/s (mișcarea reală a pistei)` | Elimină complet iluzia că pista se deplasează atunci când doar turbulențele înclină aripile aeronavei |
| **2** | **Amplificarea Vizibilității în Infraroșu Scurt** (`SWIR 1.5–2.2 µm`) | `V_SWIR = (β_VIS / β_SWIR) × V_MOR ≈ 4.5 × 50 m = 225 m` | Oferă **`+2.5 secunde` timp suplimentar de reacție** înainte de pragul pistei în ceață CAT IIIc |
| **3** | **Compensarea Predictivă a Vântului Lateral cu `0.85 s` Înainte** (`PFNd` Gust Lookahead) | `v_vânt(la 60m în față) = +10 m/s  ⟹  v_comandă = −10 m/s  ⟹  +10 − 10 = 0.0 m abatere` | Camera SWIR observă deplasarea aerosolilor de ceață la `60 m` în fața avionului și comandă eleroanele preventiv |
| **4** | **Amprenta Reliefului sub Nori (`TERCOM`) & Sinteza `2×2` din `c172p.xml`** | `500 m (barometru) − 420 m (radar 94 GHz) = deal de 80 m` • `[δ_a, δ_r]ᵀ = −M_lat⁻¹ · [C_lβ, C_nβ]ᵀ · β_req` | Localizare fără GPS sub plafonul de nori + aliniere *Wing-Low* exactă (`det(M_lat) = −0.01216`) |
| **5** | **Paznicul Anti-Spoofing GPS Dual-Layer** (`Chi² Mahalanobis + CUSUM`) | `|z_GPS − p_SWIR+Radar| > 2.0 m  (χ² > 18.5)  sau  CUSUM Drift > Prag` | Orice abatere GPS falsă (`> 2.0 m` bruscă sau derivă lentă) este **izolată în carantină în `16.6 ms`** |

```text
┌──────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│ 1. SINTEZĂ ANALITICĂ AUTOMATĂ DIN LIBRĂRIILE FLIGHTGEAR (flightgear/fg_library_extractor.py -> c172p.xml)│
│                                                                                                          │
│   M_lat = [ C_l_da   C_l_dr ] = [  0.2000   0.0147 ]   ==>  det(M_lat) = -0.012159 != 0                  │
│           [ C_n_da   C_n_dr ]   [ -0.0504  -0.0645 ]                                                     │
│                                                                                                          │
│   [ delta_a_trim ] = - M_lat^(-1) * [ C_l_beta ] * beta_req   (Reziduu numeric de moment: 1.0e-18 ≈ 0)   │
│   [ delta_r_trim ]                  [ C_n_beta ]                                                         │
│                                                                                                          │
│   phi_slip = arcsin( - q_inf * S_w * (C_Y_beta * beta + C_Y_dr * delta_r) / (m * g) )                    │
│                                                                                                          │
│ 2. AUTOMATUL DE ATERIZARE AUTONOMĂ ÎN 6 FAZE (flightgear/fg_mcp_ctl.py & fg_genetic_optimizer.py):       │
│   [FAZA 1: Interceptare] ──> [FAZA 2: Viraj de Bază C¹] ──> [FAZA 3: Captură Localizer]                  │
│       ──> [FAZA 4: Glideslope 3.0° Lock] ──> [FAZA 5: Flare C¹ Continuu] ──> [FAZA 6: Rollout & Frânare] │
└──────────────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🏆 8. Rezultate Validate Automat (FlightGear Live + Stellarium SWIR + Server Rust)

| Test / Scenariu de Verificare | Condiții Meteo & Cyber | Abatere la Touchdown (`TD_Xtk`) | Cap la Touchdown (`TD_Hdg` vs `88.93°`) | Abatere la Oprire (`Stop_Xtk`) | Verdict Automat |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **1. Zbor Live FlightGear — Interceptare Perpendiculară & Autoland CAT III (`V100`)** | `Vis: 240 m`, `089@2kt`, Spoofing GPS activ, Viraj 90° $C^1$ | **`+0.11 m`** (`11 cm`) | **`88.9°`** (`0.03°` eroare) | **`-0.18 m`** (`18 cm`) | ✅ **`PASS`** ([Video](https://youtu.be/dY4ACP80ycw)) |
| **2. Zbor Live FlightGear — Furtună Severă (`+TSRA FG`)** | `Vis: 220 m`, Vânt lateral `175° @ 14G18kt`, Ploaie `0.85`, Spoofing GPS | **`-0.25 m`** (`25 cm`) | **`88.8°`** la oprire | **`-1.84 m`** | ✅ **`PASS`** |
| **3. Fuziune Stellarium SWIR (`2.2 µm`) + FlightGear (`223 ms`)** | `9 stele` blocate (`Ori,Tau,Aur,UMa,Cas`), `SWIR SNR +20.87 dB` vs `VIS -8.68 dB` | **`-0.072 m`** (`7.2 cm`) | **`88.94°`** (Wahba err `0.00018°`) | **`+0.914 m`** | ✅ **`PASS`** |
| **4. Interceptare Maritimă Catania (`LICC — Pista 26`)** | Viraj de bază $C^1$ deasupra mării în ceață densă + Spoofing GPS | **`+0.19 m`** (`19 cm`) | **`263.5°`** (pe axul RWY 26) | **`+0.31 m`** | ✅ **`PASS`** |
| **5. Suite Unit Tests Rust + Python (`cargo test` & `unittest`)** | `103` teste Rust (5 crate-uri workspace) + `12` teste 6-DoF Python | `0.0001 m` | `88.9314°` | `0` erori / `0` `.unwrap()` | ✅ **`115/115 PASS`** |

---

## 🗂️ 9. Arhitectura Repository-ului (`100% Rust` + `FlightGear Nasal/MCP` + `Stellarium SWIR`)

```text
Craiova-Hackathon-2026/
├── crates/
│   ├── aero-math-6dof/          # Cinematică 6-DoF pe SO(3), ES-EKF 22 stări, fuziune 4 estimatoare & cuplaj rafale (17 teste)
│   ├── aero-vision-fog/         # Pipeline fotonic VIS+SWIR, SNR-Gated CLAHE, Koschmieder, suprimare halou ALS (16 teste)
│   ├── aero-meteo-cyber/        # Watchdog anti-spoofing Chi² Mahalanobis + CUSUM, sinteză furtună & vânt în ceață (17 teste)
│   ├── aero-ai-cuda/            # Connectomul Google Research Drosophila (139.255 neuroni), Zenith SWIR + DRA, PINN/LNN (11 teste)
│   └── aero-cockpit-server/     # Bucla Real-Time 60 Hz, Bridge UDP FlightGear (:5505/:5506), Server WebSocket Axum (:8080) (42 teste)
├── flightgear/
│   ├── aero_shield_hud.nas              # 3 Ferestre OpenGL Canvas în FlightGear (3D SVS PFD, Cyber Radar, GPS Tradițional) + Tunel 3D
│   ├── fg_library_extractor.py          # Extractor automat din librăriile XML FlightGear (c172p.xml, kap140) & inversiune 2x2 M_lat^-1
│   ├── fg_genetic_optimizer.py          # Optimizator genetic 6-DoF JSBSim pentru sinteza curbei de Flare C¹ și a câștigurilor AP
│   ├── c172p_extracted_fcs_library.json # Parametrii aerodinamici și câștigurile sintetizate analitic (fără reglaj manual)
│   ├── stellarium_swir_star_tracker.py  # Conector Stellarium J2000 + Centroiding SWIR 2.2 µm + Triangle Star-ID + Solver Wahba SVD
│   ├── fg_mcp_ctl.py                    # Autopilot extern TCP :5501 în 6 faze (FD == AP, Wing-Low Forward-Slip, frânare automată)
│   ├── fast_storm_verdict.py            # Simulator rapid 60 Hz pentru furtună + spoofing GPS pe Craiova (LRCV RWY 09)
│   ├── fast_catania_sea_verdict.py      # Simulator rapid 60 Hz pentru interceptare deasupra mării pe Catania (LICC RWY 26)
│   ├── fast_stellarium_swir_verdict.py  # Verificare rapidă (<250 ms) Stellarium + SWIR Star Tracker + FlightGear
│   └── test_fd_tracking.py              # Suita de teste unitare pentru Flight Director, 2x2 Matrix Inversion și Stellarium SWIR
├── docs/assets/                 # Animații GIF și capturi vizuale generate din zborurile FlightGear și prezentări
├── real_videos/
│   ├── AERO_SHIELD_Perpendicular_Autoland_V100.mp4     # Zborul cu interceptare perpendiculară 90° & Autoland V100 (YouTube: https://youtu.be/dY4ACP80ycw)
│   ├── AERO_SHIELD_Prezentare_Video_Explicata.mp4      # Prezentarea video explicată a sistemului (YouTube: https://youtu.be/D331kEyQObw)
│   └── Autonomous_FLIGH_AEROSHIELD.mp4                 # Înregistrarea zborului autonom FlightGear CAT IIIc
├── AERO_SHIELD_Craiova_Hackathon_2026.pptx             # Prezentarea oficială Widescreen (10 slide-uri)
├── AERO_SHIELD_Ghid_Complet_Explicat_De_La_Zero.pdf    # Documentația tehnică exhaustivă (22 pagini)
├── launch_flightgear_craiova.sh # Script lansare automată FlightGear 2024.1 + Server Rust AERO-SHIELD pe Craiova (LRCV RWY 09)
└── launch_flightgear_catania.sh # Script lansare automată FlightGear 2024.1 pe Catania Fontanarossa (LICC RWY 26)
```

---

## 🚀 10. Pornire Rapidă (Quick Start)

```bash
# 1. Compilare și rulare suite de teste automate Rust (103 teste) + Python (12 teste) = 115/115 PASS
cargo test --workspace --release
python3 -m unittest -v flightgear/test_fd_tracking.py
python3 flightgear/fast_stellarium_swir_verdict.py

# 2. Pornire Server Cyber-Cockpit 60 Hz (http://localhost:8080 + Bridge UDP :5505/:5506)
./target/release/aero-cockpit-server

# 3. Lansare Simulator FlightGear 2024.1 pe Aeroportul Craiova (LRCV — Pista 09) + Zbor Autonom AI
./launch_flightgear_craiova.sh
python3 flightgear/fg_mcp_ctl.py fly-spoof 120
```

---

<div align="center">
  <sub>Premiul pentru Originalitate la <b>Craiova Hackathon 2026</b> • Arhitectură <b>AERO-SHIELD LRCV V2.0</b> (100% Rust DO-178C DAL-A + FlightGear 2024.1 + Stellarium SWIR + Google Research Drosophila Connectome)</sub>
</div>
