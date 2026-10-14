# 🌍 AgriVee 360
### Complete Farm Management. One Platform.

<p align="center">
  <img src="logo.png" alt="AgriVee 360 Logo" width="300"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.38.6-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Firebase-Firestore-FF6F00?style=for-the-badge&logo=firebase&logoColor=white" />
  <img src="https://img.shields.io/badge/Platform-Android%20%7C%20iOS-1B5E20?style=for-the-badge&logo=android&logoColor=white" />
  <img src="https://img.shields.io/badge/Made%20in-South%20Africa%20🇿🇦-007A4D?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-In%20Development-F9A825?style=for-the-badge" />
</p>

---

## 📱 About AgriVee 360

**AgriVee 360** is South Africa's most comprehensive livestock and farm management application — built specifically for South African farmers managing cattle, sheep, goats, pigs, poultry and horses.

> *"Die boer se digitale assistent. The digital assistant every South African farmer deserves."*

South Africa has **35,000+ commercial farmers** and hundreds of thousands of smallholder farmers still managing livestock records, health histories, breeding cycles and farm finances on **paper or basic spreadsheets**. This costs them time, money, and livestock lives.

**AgriVee 360 changes that.**

---

## ✅ Core Features

### 🐄 Animal Identification & Records
- Register every animal with tag number and photo
- QR code and barcode ear tag scanning
- Full lineage tracking — sire (father) and dam (mother)
- Animal photo gallery with date stamps
- Support for cattle, sheep, pigs, goats, poultry and horses
- Search by tag number, name or species
- Full animal profile with complete history

### 💉 Health & Vaccination Timeline
- Record all injections, vaccinations and treatments
- Automatic reminders for upcoming vaccinations
- Disease outbreak alerts specific to your region
- Vet contact directory — call directly from the app
- Export health records to PDF
- Colour coded status — green (up to date), gold (due soon), red (overdue)

### 🐣 Breeding Management
- Heat cycle tracking per female animal
- Notifications when animals are ready for mating
- Pregnancy tracking with expected delivery date
- Alerts for expected delivery, lambing and calving
- Record breeding pairs (sire + dam)
- Offspring automatically linked to parents

### 📊 Growth & Production Tracking
- Weight tracking over time with visual growth charts
- Daily milk production tracking per animal
- Egg production tracking for poultry flocks
- Compare growth against breed averages
- Weekly and monthly production summaries

### 💰 Finance & Profit Tracker
- Record all income and expenses
- Track feed costs, vet bills, medicine and sales
- Monthly and annual profit/loss reports
- Export financial reports to PDF or Excel
- Share reports via WhatsApp or email
- Receipt photo capture

### 📦 Feed & Stock Inventory
- Track feed, medicine and equipment stock levels
- Automatic low-stock alerts before you run out
- Supplier contact directory
- Expiry date tracking for medicines
- Restock reminders

### 🗺️ GPS Farm Map
- Interactive map of your entire farm
- Mark grazing camps, water points, kraals and paddocks
- Assign animals or herds to specific locations
- Monitor camp capacity in real time
- Add, edit and remove locations

### 👥 Multi-User Access
- Farm owner account with full access
- Farm worker accounts with role-based permissions
- Full activity log — who did what and when
- Invite workers via email directly from the app

### 🔔 Smart Notifications & Reminders
- Push notifications for all upcoming tasks
- Daily farm summary every morning
- Disease outbreak alerts for your province
- Low stock alerts
- Payment reminders

### 🌟 Premium Features
- Live livestock market prices (cattle, sheep, pigs)
- Live weather forecast for your farm location
- Animal value estimator based on live market prices
- Digital animal movement certificates (PDF)
- Batch management for large herds
- Transport and movement log
- Feed calculator based on herd size
- Farm diary with daily notes
- Animal condition scoring guide
- Referral reward system

---

## 💰 Subscription Plans

| Feature | Basic | Premium |
|---|:---:|:---:|
| **Price** | **R350/month** | **R720/month** |
| Animal Records | ✅ Up to 50 | ✅ Unlimited |
| Health & Vaccination | ✅ | ✅ |
| Breeding Management | ✅ | ✅ |
| Growth Tracking | ✅ | ✅ |
| Weather Forecast (3-day) | ✅ | ✅ Full 7-day |
| Emergency Contacts | ✅ | ✅ |
| QR / Barcode Scanning | ❌ | ✅ |
| GPS Farm Map | ❌ | ✅ |
| Finance & Profit Tracker | ❌ | ✅ |
| Feed & Stock Inventory | ❌ | ✅ |
| Multi-User / Farm Workers | ❌ | ✅ |
| Export PDF & Excel | ❌ | ✅ |
| Disease Outbreak Alerts | ❌ | ✅ |
| Live Market Prices | ❌ | ✅ |
| Animal Value Estimator | ❌ | ✅ |
| Movement Certificates | ❌ | ✅ |
| Farm Analytics Dashboard | ❌ | ✅ |
| Photo Gallery | ❌ | ✅ |
| WhatsApp & Email Share | ❌ | ✅ |
| Offline Mode | ✅ | ✅ |
| Works in Afrikaans & English | ✅ | ✅ |
| Dark Mode | ✅ | ✅ |

### 🏢 Enterprise Plan
Custom pricing for agricultural co-operatives and organisations.
Contact: **agrivee360app@gmail.com**

---

## 🔧 Technology Stack

```
┌─────────────────────────────────────────────────────┐
│                   AGRIVEE 360 STACK                  │
├─────────────────┬───────────────────────────────────┤
│ Frontend        │ Flutter / FlutterFlow               │
│ Language        │ Dart / JavaScript / Node.js         │
│ Database        │ Google Firebase Firestore (NoSQL)   │
│ Authentication  │ Firebase Authentication             │
│ Cloud Functions │ Firebase Cloud Functions            │
│ Image Storage   │ Cloudinary (25GB free tier)         │
│ Payments        │ PayFast (South Africa)              │
│ Maps            │ Google Maps API                     │
│ Weather         │ OpenWeatherMap API                  │
│ Platform        │ Android & iOS                       │
│ Architecture    │ Offline-First / Cloud Sync          │
│ Distribution    │ Google Play Store / Apple App Store │
└─────────────────┴───────────────────────────────────┘
```

---

## 🗄️ Database Architecture

**10 Firestore Collections** designed for real-time sync and offline functionality:

```
AgriVee360 (Firebase Project)
│
├── 📁 users
│     └── userId → fullName, email, phone, farmName,
│                  farmLocation, plan, planStatus,
│                  paymentStatus, language, darkMode
│
├── 📁 animals
│     └── animalId → tagNumber, name, species, breed,
│                    gender, dateOfBirth, status,
│                    motherId, fatherId, farmId,
│                    photoUrl, photoGallery, qrCode,
│                    purchasePrice, purchaseDate
│
├── 📁 health_records
│     └── recordId → animalId, type, productName,
│                    dosage, date, nextDueDate,
│                    cost, administeredBy, notes
│
├── 📁 breeding_records
│     └── recordId → damId, sireId, matingDate,
│                    pregnancyConfirmed, expectedDelivery,
│                    actualDelivery, offspringIds, status
│
├── 📁 growth_records
│     └── recordId → animalId, date, weightKg,
│                    heightCm, bodyConditionScore,
│                    recordedBy, notes
│
├── 📁 production_records
│     └── recordId → animalId, type, date,
│                    quantity, unit, session, notes
│
├── 📁 finance_records
│     └── recordId → type, category, animalId,
│                    amount, description, supplier,
│                    date, receiptUrl, recordedBy,
│                    checkedBy, checkedDate
│
├── 📁 inventory
│     └── itemId → name, category, currentStock,
│                  unit, minimumStock, supplier,
│                  supplierContact, costPerUnit,
│                  lastRestocked, expiryDate
│
├── 📁 farm_map
│     └── locationId → name, type, latitude,
│                      longitude, assignedAnimals,
│                      capacity, currentCount, notes
│
└── 📁 notifications
      └── notifId → userId, animalId, type, title,
                    message, dueDate, isRead, isSent
```

---

## 📊 Project Status

| Milestone | Status | Date |
|---|:---:|---|
| Project concept and planning | ✅ Complete | June 2026 |
| Firebase project created | ✅ Complete | May 2026 |
| Firestore database — 10 collections | ✅ Complete | May 2026 |
| Firebase Authentication enabled | ✅ Complete | May 2026 |
| Security rules published | ✅ Complete | May 2026 |
| Android app registered | ✅ Complete | May 2026 |
| Cloudinary image storage | ✅ Complete | May 2026 |
| FlutterFlow project created | ✅ Complete | May 2026 |
| Firebase connected to FlutterFlow | ✅ Complete | May 2026 |
| 20 app screens designed by AI | ✅ Complete | June 2026 |
| Brand identity and logo | ✅ Complete | June 2026 |
| Subscription plans defined | ✅ Complete | June 2026 |
| Full database structure | ✅ Complete | May 2026 |
| Intellectual property documentation | ✅ Complete | June 2026 |
| Legal framework (EULA / T&Cs) | ✅ Complete | June 2026 |
| User manual (15 sections) | ✅ Complete | June 2026 |
| Google Play Store listing content | ✅ Complete | June 2026 |
| GitHub repository | ✅ Complete | September 2026 |
| PayFast payment integration | 🔄 In Progress | — |
| App screens finalised in FlutterFlow | 🔄 In Progress | — |
| Firebase connected to all screens | 🔄 In Progress | — |
| APK testing on device | ⏳ Coming Soon | — |
| Google Play Store launch | ⏳ Coming Soon | — |

---

## 🌍 Target Market

```
PRIMARY:
├── 35,000+ South African commercial farmers
├── Cattle, sheep, goat, pig and poultry farmers
└── Farmers currently using paper or spreadsheets

SECONDARY:
├── Agricultural co-operatives
│     (BKB, VKB, Senwes, NWK, OVK, TWK, Hinterland)
├── Smallholder and emerging farmers
└── Government farmer digitisation programmes

ENTERPRISE:
├── Co-op bulk licensing (R8,500–R75,000/month)
├── Annual contracts (R85,000–R750,000/year)
└── Government tenders (DAFF digitisation projects)
```

---

## 📱 App Screens

AgriVee 360 consists of **20 fully designed screens:**

```
Core Screens:
├── SplashScreen
├── LoginPage
├── RegisterPage
├── Dashboard

Animal Management:
├── AnimalRegistry
├── AnimalProfile
├── AddAnimal

Health & Breeding:
├── AddHealthRecord
├── BreedingHealth

Production & Finance:
├── ProductionGrowth
├── FinanceTracker
├── AddFinanceRecord

Management:
├── InventoryStock
├── FarmMap
├── NotificationsPage
├── FarmWorkersPage
├── ProfileSettings
├── SubscriptionSettings

Payment:
├── GracePeriodPage
└── AccountBlockedPage
```

---

## ⚖️ Legal & Intellectual Property

AgriVee 360 and all its contents — including source code, design, database structure, documentation and brand identity — are the exclusive intellectual property of **Brandon Gresse**, Republic of South Africa.

Protected under:
- **Copyright Act No. 98 of 1978** (South Africa)
- **Counterfeit Goods Act No. 37 of 1997** (South Africa)
- **Berne Convention** (180+ countries internationally)

```
© 2026 Brandon Gresse. All Rights Reserved.

Unauthorised reproduction, distribution, reverse
engineering or resale of this application or any
part thereof is strictly prohibited and constitutes
a criminal offence under South African law.
```

---

## 📩 Contact & Partnerships

**Brandon Gresse**
Founder & Lead Developer — AgriVee 360

| Contact | Details |
|---|---|
| 📧 Email | agrivee360app@gmail.com |
| 🌍 Location | South Africa |
| 🌐 Website | agrivee360.co.za (Coming Soon) |

**Open to:**
- 🤝 Agricultural co-operative partnerships
- 💰 Investor conversations
- 🏛️ Government tender discussions
- 🌾 AgriTech collaboration
- 📣 Beta farmer testers

---

## 🚀 Getting Started (For Developers)

> **Note:** This is a proprietary commercial application.
> The repository showcases the project architecture.
> Full source code access requires written authorisation.

### Prerequisites
```bash
Flutter SDK 3.38.6+
Dart 3.0+
Firebase CLI
FlutterFlow account
```

### Firebase Setup
```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login to Firebase
firebase login

# Select project
firebase use agrivee360
```

---

<p align="center">
  <strong>AgriVee 360</strong><br/>
  <em>Complete Farm Management. One Platform.</em><br/>
  <em>Die boer se digitale assistent.</em><br/><br/>
  Built with ❤️ for South African farmers 🌍🐄
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Proudly-South%20African-007A4D?style=for-the-badge" />
  <img src="https://img.shields.io/badge/English%20%7C%20Afrikaans-supported-1B5E20?style=for-the-badge" />
</p>
