# AI Exam Prep Website

AI-powered exam preparation platform built with Next.js, Prisma, and PostgreSQL.

## Features

- **Dual Authentication System**: NextAuth.js for admins, custom JWT for students
- **Dynamic Exam Generation**: AI-powered question selection and exam creation
- **Real-time Analytics**: Performance tracking and detailed result analysis
- **Mobile Responsive**: Optimized for all devices
- **Payment Integration**: Razorpay integration for subscriptions
- **Question Management**: Support for text and image-based questions

## Tech Stack

- **Frontend**: Next.js 14, React 18, TypeScript
- **Styling**: Tailwind CSS, Radix UI components
- **Backend**: Next.js API routes, Prisma ORM
- **Database**: PostgreSQL
- **Authentication**: NextAuth.js + Custom JWT
- **Payment**: Razorpay
- **Charts**: Chart.js, Plotly.js, Recharts

## Getting Started

### Prerequisites

- Node.js 18+ 
- PostgreSQL database
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Vuday3336/ai-exam-prep-website.git
cd ai-exam-prep-website
```

2. Navigate to the app directory:
```bash
cd app
```

3. Install dependencies:
```bash
npm install --legacy-peer-deps
```

4. Set up environment variables:
Create a `.env` file in the `app` directory with:
```bash
DATABASE_URL="your-postgresql-connection-string"
NEXTAUTH_URL="http://localhost:3000"
NEXTAUTH_SECRET="your-secret-key"
ABACUSAI_API_KEY="your-abacus-ai-key"
```

5. Generate Prisma client:
```bash
npx prisma generate
```

6. Run database migrations (if needed):
```bash
npx prisma db push
```

7. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:3000`

## Demo Accounts

### Admin Account
- **Email**: john@doe.com
- **Password**: johndoe123
- **Access**: Admin dashboard, question management, user management

### Student Account
- **Email**: student@demo.com
- **Password**: johndoe123
- **Access**: Student dashboard, exam taking, results viewing

## Project Structure

```
app/
├── app/                 # Next.js app directory
├── components/          # React components
├── lib/                # Utility functions and configurations
├── prisma/             # Database schema and migrations
├── public/             # Static assets
├── scripts/            # Database scripts and utilities
└── types/              # TypeScript type definitions
```

## Key Features

### Authentication System
- **Dual System**: NextAuth.js for admins, custom JWT for students
- **Device Management**: Track and manage user devices
- **Session Security**: HTTP-only cookies, CSRF protection

### Exam System
- **Dynamic Generation**: AI-powered question selection
- **Multiple Subjects**: Physics, Chemistry, Mathematics, Biology
- **Difficulty Levels**: Easy, Medium, Hard questions
- **Real-time Timer**: Automatic submission on timeout

### Analytics & Reporting
- **Performance Tracking**: Detailed score analysis
- **Subject-wise Results**: Individual subject performance
- **Progress Charts**: Visual progress representation
- **Export Options**: PDF and image export capabilities

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License.
