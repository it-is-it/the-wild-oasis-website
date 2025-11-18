# 🌴 The Wild Oasis – Hotel Booking Website

**The Wild Oasis** is a modern, responsive hotel booking platform designed to offer guests a seamless experience for browsing and reserving cabins. Built with cutting-edge technologies, it delivers an intuitive booking flow, secure authentication, and a clean, elegant UI.

🔗 **Live Demo**: [https://the-wild-oasis-website-ishwor.vercel.app/](https://the-wild-oasis-website-ishwor.vercel.app/)
🧪 **Demo Login**: `test@test.com` / `test1234`

---

## 🧠 Motivation

> _"Creating delightful user experiences in the travel industry."_

This client-facing application complements the admin system and focuses on:

- 🎯 **User-centric design** – Smooth booking experience
- ⚡ **Performance** – Fast rendering with Next.js
- 🔒 **Security** – Reliable authentication and session handling
- 📱 **Responsiveness** – Pixel-perfect UI across devices

---

## 📸 Screenshots

### 🏠 Homepage

![Homepage](./public/assets/home.png)

### 🛏️ Cabin Listings

![Cabins](./public/assets/cabins.png)

### 🔍 Cabin Details

![Cabin Detail](./public/assets/cabin-detail.png)

### 📋 Reservation Process

![Reservation](./public/assets/reservation.png)

### 👤 Guest Profile

![Guest Profile](./public/assets/guest_profile.png)

### 🔐 Authentication

![Sign In](./public/assets/signIn.png)

### 👤 Account Management

![Account](./public/assets/account.png)

### ℹ️ About Page

![About](./public/assets/about.png)

---

## ✨ Key Features

### 1. Cabin Discovery & Listings

- Browse all cabins with high-quality images
- Filter by date, capacity, and preferences
- Availability indicators for each cabin

---

### 2. Cabin Details & Booking

- Detailed cabin descriptions with image galleries
- Interactive availability calendar
- Real-time pricing based on dates, guests, and discounts
- Easy-to-use booking form

---

### 3. Smart Reservation & Pricing

- Transparent cost breakdown (accommodation + extras)
- Availability validation before booking
- Flexible booking options for nights and guests

---

### 4. Secure Authentication & User Accounts

- Email/password and Google OAuth login
- Auto-created guest profiles on first login
- Manage bookings: view, edit, cancel
- Update profile details like nationality and ID

---

### 5. Responsive & Optimized UI

- Fully mobile-friendly design
- Smooth interactions on all devices
- Fast load times with SSR, SSG, and image optimization

---

## 💻 Tech Stack

### **Frontend**

- Next.js 14 (App Router)
- React 18
- Tailwind CSS

### **Backend & Auth**

- Supabase (database + storage + auth)
- NextAuth v5 (beta)

### **UI & Utilities**

- Heroicons
- react-day-picker
- date-fns

### **Performance**

- SSR + SSG
- Next.js Image Optimization

---

## 🛠️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/it-is-it/the-wild-oasis-client-website.git
cd the-wild-oasis-client-website
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Add Environment Variables

Create `.env.local`:

```env
# Supabase
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_anon_key

# NextAuth
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_nextauth_secret

# Optional OAuth
# GOOGLE_CLIENT_ID=
# GOOGLE_CLIENT_SECRET=
```

### 4. Run Locally

```bash
npm run dev
```

Visit: [http://localhost:3000](http://localhost:3000)

---

## 🏗️ Project Structure

```
/app
├── _components/           # Reusable UI components
├── _lib/                  # Auth, actions, Supabase client, data-service
├── _styles/               # Global styles
├── about/
├── account/
│   ├── page.js
│   └── profile/page.js
├── api/
├── cabins/
│   ├── page.js
│   └── [cabinId]/page.js
├── login/page.js
├── layout.js
├── page.js
├── error.js
├── loading.js
└── not-found.js
```

---

## 🎯 Core Pages & Routes

| Route          | Description                            |
| -------------- | -------------------------------------- |
| `/`            | Homepage with CTA                      |
| `/cabins`      | All cabins + filters                   |
| `/cabins/[id]` | Cabin details + gallery + availability |
| `/about`       | About the Wild Oasis                   |
| `/login`       | Google & credentials login             |
| `/account`     | Bookings, profile, and sign-out        |

---

## 🔐 Authentication Flow

### 1. Browse as Guest

- View cabins, details, and pricing without signing in

### 2. Sign In to Reserve

- Google or email/password
- Auto-creates guest profile on first login

### 3. Manage Account

- Edit guest data
- View, update, or cancel bookings
- Secure logout

---

## 📦 Available Scripts

```bash
npm run dev      # Dev server
npm run build    # Production build
npm run start    # Start production
npm run lint     # ESLint
npm run prod     # Build + run
```

---

## 🚀 Deployment (Vercel)

1. Push code to GitHub
2. Connect repo to Vercel
3. Add environment variables
4. Deploy instantly 🎉

---

## 🔧 Required Environment Variables

| Variable               | Description             | Required |
| ---------------------- | ----------------------- | -------- |
| `SUPABASE_URL`         | Supabase project URL    | ✅       |
| `SUPABASE_KEY`         | Supabase anon key       | ✅       |
| `NEXTAUTH_URL`         | Base URL                | ✅       |
| `NEXTAUTH_SECRET`      | Token encryption secret | ✅       |
| `GOOGLE_CLIENT_ID`     | OAuth                   | Optional |
| `GOOGLE_CLIENT_SECRET` | OAuth                   | Optional |

---

## 🔮 Future Enhancements

- [ ] Stripe / PayPal payments
- [ ] Reviews & ratings
- [ ] Wishlist for favorite cabins
- [ ] Advanced search + filters
- [ ] Email/SMS notifications
- [ ] Multi-language support
- [ ] PWA offline support

---

## 🐛 Known Issues

- Timezone inconsistencies with date picker
- Very large image galleries need optimization
- Minor styling quirks on Safari

---

## 👨‍💻 Author

**Ishwor Timalsina**

- Portfolio: [https://ishwortimalsina.com.np](https://ishwortimalsina.com.np)
- LinkedIn: [https://linkedin.com/in/ishwor-timalsina](https://linkedin.com/in/ishwor-timalsina)

---

## 🙏 Acknowledgments

- Next.js team
- Supabase
- Vercel
- Open-source community
- Jonas Schmedtmann’s Udemy course for inspiration

---

## 🔗 Related Projects

- 🏨 **The Wild Oasis Admin** — [https://github.com/it-is-it/the-wild-oasis](https://github.com/it-is-it/the-wild-oasis)
- 🛒 **Ecommerce Website** — [https://github.com/it-is-it/Ecommerce](https://github.com/it-is-it/Ecommerce)
- 🌍 **WorldWise Travel App** — [https://github.com/it-is-it/Worldwise](https://github.com/it-is-it/Worldwise)

---
