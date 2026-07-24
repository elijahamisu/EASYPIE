EASYPIE

Deployment: Vercel Database: Supabase License: MIT

EASYPIE is a premium, mobile-first investment platform specifically designed for
the Nigerian market. It offers a streamlined, high-trust environment for users
to invest Nigerian Naira (₦) and earn automated daily returns.

🚀 Features

  - Premium UI/UX: Fully responsive, mobile-first design with a fintech-grade
    aesthetic.
  - Automated Earnings: Daily investment growth credited automatically every day
    at 12:00 AM (Africa/Lagos).
  - Secure Authentication: Robust user management via Supabase Auth (Register,
    Login, Password Recovery).
  - Kuda Bank Integration: Dedicated deposit workflow optimized for Kuda Bank
    transfers.
  - Real-time Dashboard: Track investments, wallet balances, and transaction
    history instantly.
  - Admin Oversight: Comprehensive admin panel for managing users, verifying
    deposits, and monitoring system health.
  - KYC & Security: Integrated KYC verification process and Row Level Security
    (RLS) for data protection.

🛠 Technology Stack

  - Frontend: HTML5, CSS3 (Modern Flexbox/Grid), Vanilla JavaScript (ES6+).
  - Backend-as-a-Service: Supabase (Database, Auth, Storage).
  - Serverless Logic: Vercel Serverless Functions (Node.js 20.x).
  - Hosting: Vercel.
  - Database Logic: PostgreSQL with Row Level Security (RLS).

📁 Project Structure

EASYPIE/
├── admin/          # Administrative dashboard and management pages
├── api/            # Vercel Serverless Functions (Backend logic)
├── assets/         # Global styles, scripts, images, and fonts
├── components/     # Reusable UI fragments (Navbar, Footer, Modals)
├── database/       # SQL migrations, RLS policies, and DB functions
├── public/         # Static assets (Favicon, Manifest, Robots)
├── supabase/       # Supabase configuration and storage rules
└── *.html          # User-facing application pages

⚙️ Installation

1.  Clone the repository:

    git clone https://github.com/your-username/easypie.git
    cd easypie

2.  Install dependencies:

    npm install

3.  Environment Setup:

      - Copy .env.example to .env.
      - Fill in your SUPABASE_URL, SUPABASE_ANON_KEY, and
        SUPABASE_SERVICE_ROLE_KEY.
      - Configure the Kuda Bank account details and CRON_SECRET.

4.  Local Development:

    npm run dev

🔐 Supabase Setup

To ensure the platform functions correctly, execute the SQL scripts in the
database/ folder within your Supabase SQL Editor in the following order:

1.  schema.sql: Creates tables for wallets, investments, and transactions.
2.  functions.sql: Sets up the logic for daily interest calculation.
3.  policies.sql: Enables Row Level Security (RLS) to protect user data.
4.  seed.sql: (Optional) Populates the platform with initial investment plans.

💰 Investment & Earnings

  - Currency: All transactions are processed in Nigerian Naira (₦).
  - Timezone: System logic operates strictly on Africa/Lagos.
  - Daily Accruals: The system uses a Vercel Cron Job (calling /api/cron.js) to
    trigger daily earnings exactly at 12:00 AM Lagos time.
  - Deposits: Currently exclusively supports Kuda Bank transfers for streamlined
    reconciliation.

🚀 Deployment

This project is optimized for Vercel.

1.  Push your code to a GitHub repository.
2.  Connect the repository to Vercel.
3.  Add your Environment Variables in the Vercel Dashboard.
4.  Vercel will automatically detect the Serverless Functions in the api/
    directory.

🛡 Security

  - Row Level Security (RLS): Users can only read/write their own financial
    data.
  - Service Role Protection: Sensitive operations (like adding earnings) are
    restricted to server-side execution via the SUPABASE_SERVICE_ROLE_KEY.
  - Input Validation: All frontend and backend inputs are sanitized and
    validated.

📄 License

This project is licensed under the MIT License - see the LICENSE file for
details.

📞 Support

For technical support or inquiries, please contact the EASYPIE development team
or visit the Support page within the application.
