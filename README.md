# PrecisionCare Admin Operations Panel 🏥

Dedicated Operations & Diagnostic Management Portal for **PrecisionCare Diagnostic Centre**.

Designed specifically for administrators, lab managers, and diagnostic coordinators to manage real-time patient requests, diagnostic test catalogs, category hierarchies, sample collection dispatches, and lab reports.

---

## 🌟 Key Features

- **Dynamic Diagnostic Catalog & Category Management:**
  - Full CRUD operations on diagnostic categories (e.g. Digital X-Ray, Blood Tests, ECG & Cardio, Ultrasound, PFT, Health Packages, and custom categories).
  - Add, edit, and delete categories with live icon selection and automatic test count badges.
  - Strict category isolation: browsing a category isolates tests exclusively belonging to that department.
  - Test creation flow with auto-selected categories and on-the-fly category addition.
- **Booking Operations & Live Queues:**
  - Real-time Firestore stream of patient appointment requests.
  - Status updates: Pending, Accepted, Sample Collected, Processing, Completed, Cancelled.
  - Instant dispatch assignment to field technicians and phlebotomists.
- **Lab Report Generation & Uploads:**
  - Direct PDF lab report uploads (powered by ImgBB & Cloud Storage).
  - Automatic push notification reminders to patients upon report publication.
- **Prescription & Field Order Printing:**
  - Print patient diagnostic slips and doctor prescriptions directly from the web browser.
- **Promotional Banners & Deals:**
  - Upload and manage home promotional banners with accurate 2:1 aspect ratio locking.
- **Staff & Technician Directory:**
  - Add and manage phlebotomists, radiologists, pathologists, and technicians with phone, qualification, and vehicle details.

---

## 🚀 Running Locally

```bash
# Get dependencies
flutter pub get

# Run on Chrome
flutter run -d chrome
```

---

## 🌐 Deploying to Vercel

```bash
# Build web release bundle
flutter build web --release

# Output is ready in build/web/
```

Configured with `vercel.json` for single-page routing (`/index.html`) and CORS headers.
