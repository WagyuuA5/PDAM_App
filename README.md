<p align="center">
  <img src="https://github.com/user-attachments/assets/88457ded-a0f8-4e19-a907-66fe48b2d029" width="55" height="55" alt="PDAM Logo" />
  &nbsp;&nbsp;
  <strong style="font-size:1.8em">PDAM — Water Utility Management System</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.28.3-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Dart-3.10.1-0175C2?style=for-the-badge&logo=dart&logoColor=white" />
  <img src="https://img.shields.io/badge/License-Apache%202.0-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Platform-Android%20%7C%20iOS-lightgrey?style=for-the-badge&logo=flutter" />
  <img src="https://img.shields.io/badge/Backend-REST%20API-orange?style=for-the-badge&logo=postman&logoColor=white" />
</p>

<p align="center">
  A modern, cross-platform mobile application for managing water utility (PDAM) billing, customer data, services, and payment verification — built with Flutter and backed by a RESTful API.
</p>

---

## 📱 Overview

**PDAM** is a full-featured water utility management application designed for both **administrators** and **customers**. It streamlines the end-to-end workflow of water billing — from service tier configuration and customer registration, to bill generation, payment upload, and payment verification.

The app implements **role-based access control (RBAC)** with JWT authentication, providing distinct experiences and permissions for admin and customer roles.

---

## ✨ Key Features

### 🔐 Authentication
- JWT-based login with role detection (Admin / Customer)
- Secure token storage and automatic session management
- Role-aware navigation and UI rendering

### 👤 Admin Features
| Feature | Description |
|---|---|
| **Dashboard** | Overview of billing metrics, outstanding payments, pending verifications |
| **Customer Management** | Register, edit, search, and delete customer accounts |
| **Service Tier Management** | Create and manage tiered water pricing (e.g., Residential, Industrial) |
| **Bill Management** | Generate monthly bills per customer with auto-filled meter readings |
| **Payment Verification** | Accept or reject payment proofs submitted by customers |

### 🧾 Customer Features
| Feature | Description |
|---|---|
| **Statement Dashboard** | View total unpaid balance and 6-month average spending |
| **Bill History** | Full history with UNPAID, PENDING, and PAID statuses |
| **Pay Now** | Upload payment proof for pending bills |
| **Profile Management** | View account info, change settings, and logout |

---

## 📸 Screenshots

<p align="center">
  <img src="https://github.com/user-attachments/assets/8f54f542-2236-4d59-86b7-c26ea483c945" width="180" alt="Add New Bill" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/854f3810-f602-4dc8-b991-8b2beb708e25" width="180" alt="Payment Confirmation" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/c014cf21-d0c3-48ec-a30f-7ced6ce0a238" width="180" alt="Add New Service" />
</p>
<p align="center">
  <sub>Add New Bill &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Payment Confirmation &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Add New Service</sub>
</p>

<br/>

<p align="center">
  <img src="https://github.com/user-attachments/assets/ff39cb32-32cb-4cf7-8b58-2a0559905d74" width="180" alt="Register Customer" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/14ce5c98-7af6-40e9-992a-290963c273ec" width="180" alt="Manage Services" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/9806aa99-5aa7-4f31-bac4-f1e88f9af8fb" width="180" alt="Manage Bills" />
</p>
<p align="center">
  <sub>Register Customer &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Manage Services &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Manage Bills</sub>
</p>

<br/>

<p align="center">
  <img src="https://github.com/user-attachments/assets/eaf7ff60-fd1f-412f-ab2f-c58a62c00b64" width="180" alt="Admin Profile" />
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/04dea62f-382f-44de-a2cd-c919dd98d0b2" width="180" alt="Customer Profile" />
</p>
<p align="center">
  <sub>Admin Profile &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Customer Profile</sub>
</p>

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: Flutter 3.28.3 (stable channel)
- **Language**: Dart 3.10.1
- **DevTools**: 2.51.1
- **Engine**: `8bf2090718fea3655f466049a757f823898f0ad1`
- **Framework Revision**: `19074d12f7` (2025-11-20)

### Backend
- **Base URL**: `https://learn.smktelkom-mlg.sch.id/pdam`
- **Architecture**: RESTful API with JWT Authentication
- **API Collection**: [Postman Collection — PDAM Backend](https://s.id/PDAM_Backend)
- **Auth Scheme**: Bearer Token (role-scoped: Admin / Customer)

---

## 📦 Libraries Used in This Project

| Library | Version | Purpose |
|---|---|---|
| [`dio`](https://pub.dev/packages/dio) | ^5.x | HTTP client for REST API communication |
| [`flutter_secure_storage`](https://pub.dev/packages/flutter_secure_storage) | ^9.x | Secure JWT token storage |
| [`provider`](https://pub.dev/packages/provider) | ^6.x | State management |
| [`go_router`](https://pub.dev/packages/go_router) | ^13.x | Declarative routing with role-based guards |
| [`image_picker`](https://pub.dev/packages/image_picker) | ^1.x | Pick payment proof images from gallery/camera |
| [`cached_network_image`](https://pub.dev/packages/cached_network_image) | ^3.x | Efficient network image loading with caching |
| [`intl`](https://pub.dev/packages/intl) | ^0.19.x | Date formatting and localization (IDR currency) |
| [`flutter_svg`](https://pub.dev/packages/flutter_svg) | ^2.x | SVG icon and asset rendering |
| [`shimmer`](https://pub.dev/packages/shimmer) | ^3.x | Skeleton loading effect for async data |
| [`lottie`](https://pub.dev/packages/lottie) | ^3.x | Animated illustrations and success states |
| [`dotted_border`](https://pub.dev/packages/dotted_border) | ^2.x | Dotted border for upload proof UI component |
| [`permission_handler`](https://pub.dev/packages/permission_handler) | ^11.x | Runtime permissions for camera and storage |
| [`equatable`](https://pub.dev/packages/equatable) | ^2.x | Value equality for model classes |
| [`json_annotation`](https://pub.dev/packages/json_annotation) | ^4.x | JSON serialization/deserialization |
| [`build_runner`](https://pub.dev/packages/build_runner) | ^2.x | Code generation (dev dependency) |
| [`json_serializable`](https://pub.dev/packages/json_serializable) | ^6.x | Auto-generate JSON converters (dev dependency) |
| [`flutter_launcher_icons`](https://pub.dev/packages/flutter_launcher_icons) | ^0.14.x | Custom app icon generation (dev dependency) |

> **Note:** Version numbers reflect the approximate ranges used during development. Refer to `pubspec.yaml` for pinned versions.

---

## 🚀 Getting Started

### Prerequisites

Ensure the following are installed on your machine:

- [Flutter SDK](https://docs.flutter.dev/get-started/install) `>= 3.28.0`
- [Dart SDK](https://dart.dev/get-dart) `>= 3.10.0`
- Android Studio / Xcode (for emulator or device deployment)
- [Postman](https://www.postman.com/) (optional, for API testing)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/WagyuuA5/pdam-flutter.git
cd pdam-flutter

# 2. Install dependencies
flutter pub get

# 3. Run code generation (for JSON serialization)
dart run build_runner build --delete-conflicting-outputs

# 4. Run the application
flutter run
```

### Environment Configuration

Create a `.env` file or update `lib/core/constants/api_constants.dart`:

```dart
const String baseUrl = 'https://learn.smktelkom-mlg.sch.id/pdam';
```

---

## 🔑 API Reference

The backend API is documented and tested using Postman.

- **Postman Collection**: [https://s.id/PDAM_Backend](https://s.id/PDAM_Backend)
- **Base URL**: `https://learn.smktelkom-mlg.sch.id/pdam`

### Authentication Endpoints

| Method | Endpoint | Role | Description |
|---|---|---|---|
| `POST` | `/auth/login` | Public | Login and receive JWT token |
| `POST` | `/auth/logout` | Auth | Invalidate current session token |

### Admin Endpoints

| Method | Endpoint | Role | Description |
|---|---|---|---|
| `GET` | `/customers` | Admin | Get all customers |
| `POST` | `/customers` | Admin | Register new customer |
| `PUT` | `/customers/:id` | Admin | Update customer data |
| `DELETE` | `/customers/:id` | Admin | Delete a customer |
| `GET` | `/services` | Admin | Get all service tiers |
| `POST` | `/services` | Admin | Create new service tier |
| `PUT` | `/services/:id` | Admin | Update service tier |
| `DELETE` | `/services/:id` | Admin | Delete service tier |
| `GET` | `/bills` | Admin | Get all bills |
| `POST` | `/bills` | Admin | Create new bill |
| `PUT` | `/bills/:id/verify` | Admin | Accept/reject payment proof |

### Customer Endpoints

| Method | Endpoint | Role | Description |
|---|---|---|---|
| `GET` | `/bills/me` | Customer | Get current user's bills |
| `POST` | `/bills/:id/pay` | Customer | Upload payment proof |
| `GET` | `/profile/me` | Customer | Get own profile |

---

## 📁 Project Structure

```
lib/
├── core/
│   ├── constants/         # API URLs, app constants
│   ├── errors/            # Custom exception classes
│   ├── network/           # Dio client, interceptors, token injection
│   └── utils/             # Formatters, validators, helpers
├── data/
│   ├── models/            # JSON-serializable data models
│   ├── repositories/      # Data layer (API calls)
│   └── datasources/       # Remote data sources
├── domain/
│   ├── entities/          # Business logic entities
│   └── usecases/          # Use case abstractions
├── presentation/
│   ├── auth/              # Login screen
│   ├── admin/
│   │   ├── dashboard/     # Admin home
│   │   ├── customers/     # Customer management
│   │   ├── services/      # Service tier management
│   │   └── bills/         # Bill management & verification
│   ├── customer/
│   │   ├── statements/    # Bill history & payment
│   │   └── profile/       # Customer profile
│   └── shared/
│       ├── widgets/       # Reusable UI components
│       └── theme/         # App theme, colors, typography
├── routes/                # GoRouter configuration with guards
└── main.dart
```

---

## 🔒 Role-Based Access

This app enforces strict role-based access control using JWT claims:

| Feature | Admin | Customer |
|---|:---:|:---:|
| View all customers | ✅ | ❌ |
| Register/Edit/Delete customers | ✅ | ❌ |
| Manage service tiers | ✅ | ❌ |
| Create bills | ✅ | ❌ |
| Verify payments | ✅ | ❌ |
| View own bills | ❌ | ✅ |
| Pay bills (upload proof) | ❌ | ✅ |
| View own profile | ✅ | ✅ |

---

## 🧪 Testing the API

Import the Postman collection and follow these steps:

1. **Login** as admin using `POST /auth/login` → copy the `token`
2. Set the token as a **Bearer Token** in your Postman environment
3. Test admin endpoints (create customer, create service, create bill)
4. **Switch token** to a customer account
5. Test customer endpoints (`GET /bills/me`, `POST /bills/:id/pay`)

> ⚠️ Common issues:
> - **409 Conflict**: Customer ID or username already exists
> - **404 Not Found**: Token context mismatch — verify you are using the correct role token
> - **401 Unauthorized**: Token expired or missing `Authorization: Bearer <token>` header

---

## 📄 License

```
Copyright 2026 Wahyu Ravi Anggoro

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

---

## 👨‍💻 Author

<table>
  <tr>
    <td align="center">
      <strong>Wahyu Ravi Anggoro</strong><br/>
      <code>@WagyuuA5</code><br/>
      Student at SMK Telkom Malang — 2026<br/>
      <a href="https://github.com/WagyuuA5">github.com/WagyuuA5</a>
    </td>
  </tr>
</table>

---

## 🙏 Acknowledgements

- [Flutter Team](https://flutter.dev) — for the amazing cross-platform framework
- [SMK Telkom Malang](https://smktelkom-mlg.sch.id) — for the backend infrastructure and project support
- All open-source library authors listed above

---

<p align="center">
  Made with ❤️ and 💧 by <strong>Wahyu Ravi Anggoro</strong> · SMK Telkom Malang · 2026
</p>
