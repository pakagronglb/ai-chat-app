# AI Chat Application

![AI Chat Application](public/chatgpt.gif)

A modern AI chat application built with Next.js, featuring real-time conversations with an AI assistant.

## 🚀 Features

- Real-time AI chat interface
- Message history persistence using Prisma and PostgreSQL
- Modern and responsive UI
- Environment variable configuration
- API rate limiting
- Type-safe database operations

## 🛠️ Tech Stack

- **Frontend**: Next.js 14, React, TypeScript
- **Backend**: Next.js API routes
- **Database**: PostgreSQL
- **ORM**: Prisma
- **Styling**: Tailwind CSS
- **Type Safety**: TypeScript

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v18 or higher)
- npm or yarn
- PostgreSQL

## ⚙️ Environment Setup

1. Clone the repository:
```bash
git clone https://github.com/pakagronglb/ai-chat-app.git
cd ai-chat-app
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Create a `.env` file in the root directory with the following variables:
```env
DATABASE_URL="postgresql://username:password@localhost:5432/dbname"
AI_API_KEY="your-ai-api-key"
```

4. Set up the database:
```bash
npx prisma generate
npx prisma db push
```

## 🚀 Development

Run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the application.

## 📁 Project Structure

```
├── app/
│   ├── api/
│   │   └── route.ts         # API endpoints
│   ├── components/          # React components
│   ├── db.ts               # Database configuration
│   └── page.tsx            # Main page
├── prisma/
│   └── schema.prisma       # Database schema
├── public/                 # Static assets
└── types/                  # TypeScript type definitions
```

## 🔧 Configuration

### Database Configuration
The application uses Prisma with PostgreSQL. The database schema is defined in `prisma/schema.prisma`.

### API Configuration
API routes are configured in `app/api/route.ts` with appropriate rate limiting and error handling.

## 📝 API Documentation

### Chat Endpoint
- **POST** `/api/chat`
  - Request body: `{ message: string }`
  - Response: `{ response: string, timestamp: Date }`

## 🚀 Deployment

The application can be deployed using Vercel:

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Configure environment variables in Vercel dashboard
4. Deploy!

For other deployment options, check out the [Next.js deployment documentation](https://nextjs.org/docs/deployment).

## 🧪 Testing

Run the test suite:

```bash
npm test
# or
yarn test
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- Pakagrong Lebel

## 🙏 Acknowledgments

- Next.js team for the amazing framework
- Vercel for the deployment platform
- Jan Marsal - [Tutorial Reference](https://www.youtube.com/watch?v=jf7ocqdhiKc)
- All contributors who help improve the project
