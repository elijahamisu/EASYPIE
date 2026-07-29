# EASYPIE

## Project Overview
**EASYPIE** is a premium Nigerian Naira (NGN) investment platform engineered for security, simplicity, and high performance. Designed with a mobile-first philosophy, the platform provides a luxury dark-themed interface that allows users to grow their wealth through a streamlined investment process. 

The application leverages **Supabase** for real-time database management and authentication, uses **Vite** for optimized frontend performance, and is built for seamless deployment on **Vercel**.

---

## Features

### User Features
*   **Secure Authentication:** Registration and Login systems (No KYC required for ease of use).
*   **Welcome Bonus:** Every new user automatically receives a **₦500 bonus** upon successful registration.
*   **Dynamic Dashboard:** Real-time tracking of wallet balance, active investments, and daily earnings.
*   **Investment Plans:** Browse and subscribe to various investment packages.
*   **Flexible Funding:** Users can invest directly from their wallet balance.
*   **Kuda Bank Deposits:** Exclusive integration with Kuda Bank for simplified deposits.
*   **Automated Earnings:** Daily profits are calculated and credited automatically every day at **12:00 AM (Africa/Lagos)**.
*   **Referral System:** Built-in reward system for inviting new investors.
*   **Transaction History:** Detailed logs for deposits, withdrawals, earnings, and referrals.
*   **Notifications:** Real-time alerts for all account activities.
*   **Community Integration:** Direct access to the official Telegram community.

### Admin Features
*   **Live Statistics:** Comprehensive overview of platform performance.
*   **User Management:** Monitor and manage all registered investors.
*   **Financial Oversight:** Approve/Manage deposits and withdrawals.
*   **System Settings:** Configure platform parameters and investment plans.

---

## Project Structure
The project follows a clean and modular architecture for easy maintenance and deployment:

*   `/` (Root): Main application pages (HTML).
*   `admin/`: Exclusive dashboard and management tools for administrators.
*   `api/`: Client-side logic and Supabase integration scripts.
*   `assets/`: Global styles (CSS), images, and client-side JavaScript.
*   `config/`: Configuration files and environment constant loaders.
*   `public/`: Static assets like icons and manifest files.

---

## Installation

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/easypie.git
    cd easypie
    ```

2.  **Install Dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Setup:**
    *   Copy `.env.example` to a new file named `.env`.
    *   Input your **Supabase URL** and **Anon Key**.
    *   Configure your Kuda Bank details and Telegram link.

4.  **Start Development Server:**
    ```bash
    npm run dev
    ```

5.  **Build for Production:**
    ```bash
    npm run build
    ```

---

## Environment Variables
The following variables are required for the application to function. Ensure they are set in your deployment environment (e.g., Vercel Dashboard):

*   `VITE_SUPABASE_URL`: Your Supabase project endpoint.
*   `VITE_SUPABASE_ANON_KEY`: Your Supabase public API key.
*   `VITE_APP_NAME`: EASYPIE
*   `VITE_WELCOME_BONUS`: 500
*   `VITE_KUDA_ACCOUNT_NUMBER`: Your Kuda account details.
*   `VITE_TELEGRAM_LINK`: Official community link.

---

## Technologies
*   **Frontend:** HTML5, CSS3 (Modern Flexbox/Grid), JavaScript (ES Modules).
*   **Backend & Database:** Supabase (PostgreSQL).
*   **Build Tool:** Vite.
*   **Deployment:** Vercel.

---

## Security
EASYPIE is built with a "Security First" mindset:
*   **No Hardcoded Keys:** All sensitive credentials are managed via Environment Variables.
*   **Secure Queries:** Database interactions are handled through secure Supabase client protocols.
*   **Validation:** Strict input validation on all forms to prevent injection and errors.
*   **Protected Admin Area:** The admin directory is restricted to authorized personnel only.

---

## Deployment
This project is optimized for **Vercel**. 
*   No `vercel.json` is required. 
*   Simply connect your GitHub repository to Vercel, import the environment variables, and deploy.

---

## Support
For technical issues or inquiries, please visit the **Support** page within the application or contact the administrator via the provided admin email.

---
*© 2024 EASYPIE. All Rights Reserved.*
