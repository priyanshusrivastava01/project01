# Website Builder (Frontend)

This is a frontend-only React application powered by Vite, Tailwind CSS, and Redux. It is designed to be deployed directly and seamlessly on **Vercel**.

## Features
- **Interactive Editor**: Drag-and-drop or prompt-based website builder.
- **Firebase Authentication**: Integrated Google login.
- **Tailwind CSS**: Modern styled components.

## Deploying to Vercel
Since the frontend application is located at the root of this repository, you can deploy it to Vercel without any special subdirectory configuration:

1. Push this repository to GitHub/GitLab/Bitbucket.
2. Go to [Vercel](https://vercel.com) and click **Add New Project**.
3. Import this repository.
4. (Optional) In the **Environment Variables** section, add:
   - `VITE_FIREBASE_API_KEY`: Your Firebase API key.
   - `VITE_SERVER_URL`: The URL of your deployed backend server (if any).
5. Click **Deploy**. Vercel will automatically detect the Vite setup, install dependencies, and publish the site.

## Local Development
To run this project locally:

1. Install dependencies:
   ```bash
   npm install
   ```
2. Set up your environment variables in a `.env` file at the root:
   ```env
   VITE_FIREBASE_API_KEY=your_firebase_api_key_here
   VITE_SERVER_URL=http://localhost:8000
   ```
3. Start the Vite development server:
   ```bash
   npm run dev
   ```