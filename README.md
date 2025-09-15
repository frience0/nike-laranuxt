# 🛒 Nuxt + Laravel E-commerce

A modern **E-commerce application** built with **Nuxt 3** (frontend) and **Laravel** (backend API).  
This project combines the power of Nuxt for SSR/SPA user experience and Laravel for secure backend services, authentication, and database management.

---

## 🚀 Tech Stack

### Frontend (Nuxt 3)

- [Nuxt 3](https://nuxt.com/) with SSR/SPA support
- [TailwindCSS](https://tailwindcss.com/) + Typography
- [Pinia](https://pinia.vuejs.org/) (state management)
- [Prisma](https://www.prisma.io/) with Nuxt integration
- [Stripe](https://stripe.com/) via `@unlok-co/nuxt-stripe`
- [Vue Router](https://router.vuejs.org/)
- [Vuelidate](https://vuelidate-next.netlify.app/) for form validation
- [Chart.js](https://www.chartjs.org/) for analytics
- [SweetAlert2](https://sweetalert2.github.io/) and [Vue Toast Notification](https://vue-toastification.maronato.dev/) for UI feedback
- [Vue3 OTP Input](https://www.npmjs.com/package/vue3-otp-input) for OTP verification
- [Zod](https://zod.dev/) for schema validation

### Backend (Laravel)

- REST API built with **Laravel 11**
- **MySQL / PostgreSQL** database (via Prisma ORM client)
- **Authentication & JWT**
- **Multer** for file uploads
- **Bcrypt** for password hashing
- **Nodemailer** (via Nuxt integration) for email notifications

---

## 📂 Project Structure

---

## ⚙️ Setup & Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/nuxt-laravel-ecommerce.git
cd nuxt-laravel-ecommerce


cd nuxt-app
npm install
npm run dev


cd laravel-api
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve


NUXT_STRIPE_KEY=your_stripe_public_key
NUXT_BACKEND_URL=http://localhost:8000/api
NUXT_JWT_SECRET=your_jwt_secret




DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=ecommerce
DB_USERNAME=root
DB_PASSWORD=

JWT_SECRET=your_jwt_secret
MAIL_MAILER=smtp
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME=your_username
MAIL_PASSWORD=your_password

```

```
npm run dev        # Start development server
npm run build      # Build for production
npm run generate   # Generate static site
npm run preview    # Preview production build
npm start          # Start production server
```
