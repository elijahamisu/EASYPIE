EASYPIE

EASYPIE is a premium, mobile-first Nigerian Naira (₦) investment platform built
for high performance, security, and trust. It provides users with a seamless
experience to grow their wealth through structured investment plans, featuring
automated daily earnings and secure wallet management.

🚀 Features

  - Premium Fintech UI: High-end, accessible, and responsive design optimized
    for mobile devices.
  - Secure Authentication: Robust user registration and login system powered by
    Supabase.
  - Investment Management: Browse plans, track active investments, and view
    real-time earning stats.
  - Kuda Bank Integration: Streamlined deposit workflow via dedicated Kuda Bank
    account details.
  - Automated Daily Earnings: Interest is calculated and credited to user
    wallets daily at 12:00 AM (Africa/Lagos).
  - Comprehensive Dashboard: Overview of total balance, active investments, and
    recent activities.
  - Financial History: Detailed logs for deposits, withdrawals, and transaction
    history.
  - KYC & Security: Integrated identity verification and account security
    settings.
  - Admin Suite: Full management interface for users, investments, and platform
    configurations.

🛠 Technology Stack

  - Frontend: HTML5, CSS3 (Modern Flexbox/Grid), Vanilla JavaScript (ES6+).
  - Backend-as-a-Service: Supabase (Auth, Database, Storage, RLS).
  - Serverless Logic: Vercel Serverless Functions (Node.js 20).
  - Hosting: Vercel.
  - Database: PostgreSQL with Row Level Security (RLS).

📂 Project Structure

EASYPIE/
├── admin/          # Administrative dashboard and management pages
├── api/            # Vercel Serverless Functions (Node.js)
├── assets/         # Styles, scripts, images, and fonts
├── components/     # Reusable HTML snippets (Navbar, Sidebar, etc.)
├── database/       # SQL schemas, policies, and seed data
├── public/         # Static assets (Favicons, manifest)
└── supabase/       # Supabase migrations and storage config

⚙️ Installation

1.  Clone the repository:

    git clone https://github.com/your-username/easypie.git
    cd easypie

2.  Install dependencies:

    npm install

3.  Set up environment variables: Copy the .env.example file to .env and fill in
    your Supabase credentials.

    cp .env.example .env

🔑 Environment Variables

Required variables for the project to function:

| Variable                        | Description                                    |
| :------------------------------ | :--------------------------------------------- |
| `NEXT_PUBLIC_SUPABASE_URL`      | Your Supabase Project URL                      |
| `NEXT_PUBLIC_SUPABASE_ANON_KEY` | Supabase anonymous API key                     |
| `SUPABASE_SERVICE_ROLE_KEY`     | Secret key for server-side operations          |
| `CRON_SECRET`                   | Security token for the daily earnings cron job |
| `KUDA_ACCOUNT_NUMBER`           | The platform's Kuda Bank account for deposits  |

💻 Local Development

Run the project locally using the Vercel CLI to support serverless functions:

# Start the local development server
npm run dev

The application will be available at http://localhost:3000.

🚀 Deployment on Vercel

This project is optimized for Vercel.

1.  Push your code to a GitHub repository.
2.  Connect the repository to Vercel.
3.  Add the Environment Variables in the Vercel Dashboard.
4.  Vercel will automatically detect the configuration and deploy.

🗄️ Supabase Setup

1.  Create a new Supabase project.
2.  Run the scripts in database/schema.sql to create the necessary tables.
3.  Apply database/policies.sql to enable Row Level Security (RLS).
4.  Create an avatars bucket in Supabase Storage for user profile pictures.

💰 Kuda Bank Deposit Workflow

1.  User navigates to the Deposit page.
2.  The platform displays the official Kuda Bank account details.
3.  User makes a transfer via their banking app.
4.  User submits the transaction reference/proof on EASYPIE.
5.  Admin reviews and approves the deposit from the Admin Dashboard.

📅 Daily Earnings System

EASYPIE features an automated interest distribution system:

  - Execution Time: Daily at 12:00 AM (Africa/Lagos).
  - Logic: The api/cron.js function calculates interest based on active
    investment plans and updates user balances.
  - Security: The endpoint is protected by a CRON_SECRET header.

🛡️ Security Features

  - Row Level Security (RLS): Users can only read/write their own data.
  - Input Validation: Strict sanitization on both client and server sides.
  - Serverless Logic: Sensitive operations (like earnings calculation) are
    hidden from the frontend.
  - Protected Routes: Unauthorized users are redirected from private pages.

🤝 Contributing

1.  Fork the Project.
2.  Create your Feature Branch (git checkout -b feature/AmazingFeature).
3.  Commit your Changes (git commit -m 'Add some AmazingFeature').
4.  Push to the Branch (git push origin feature/AmazingFeature).
5.  Open a Pull Request.

📄 License

Distributed under the MIT License. See LICENSE for more information.

📞 Support

For support, email support@easypie.com or visit the Support Page within the app.

EASYPIE • Premium Investment Solutions for Nigeria.
