<a name="readme-top"></a>
<br />

<p align="center">
  <img src="https://ik.imagekit.io/haio54fgp/kwikchat-assets/logo.png" alt="KwikChat" width="400"/>
</p>

<h3 align="center">
  <strong>KwikChat – Real-Time Messaging Made Simple</strong>
</h3>

<p align="center">
  KwikChat is a modern real-time chat application built with Next.js, Pusher, Prisma, and PostgreSQL. Designed for speed, scalability, and a polished user experience, it's perfect for teams, communities, or anyone who needs a reliable messaging tool.
</p>

<p align="center">
  <a href="https://kwikchat.vercel.app">Live Demo</a> |
  <a href="https://github.com/nilotpaldhar/kwikchat">Documentation</a> |
  <a href="https://github.com/nilotpaldhar/kwikchat/issues">Request Feature</a>
</p>

<p align="center">
  <a href="http://commitizen.github.io/cz-cli/">
    <img alt="Commitizen friendly" src="https://img.shields.io/badge/commitizen-friendly-brightgreen.svg?style=for-the-badge" />
  </a>
  <a href="https://github.com/nilotpaldhar/kwikchat/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/nilotpaldhar/kwikchat.svg?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/nilotpaldhar/kwikchat/pulls">
    <img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge" />
  </a>
  <a href="https://linkedin.com/in/nilotpaldhar">
    <img alt="Connect on LinkedIn" src="https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=16B" />
  </a>
</p>

<p align="center">
  <img src="https://ik.imagekit.io/haio54fgp/kwikchat-assets/app-overview.png?updatedAt=1744297521447" alt="App Screenshot" />
</p>

## 📽️ Demo Video

Watch the quick demo of KwikChat in action:

[![Watch the demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

## 📑 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Deployment](#deployment)
- [Contribution](#contribution)
- [Support](#support)
- [License](#license)

## Features ✨

- 🔐 Secure authentication flow
- 🧠 Smart user presence detection
- ⚡ Real-time message updates via Pusher
- 💬 Beautiful, responsive UI with Tailwind & Shadcn
- 📱 Mobile-first design
- 🕒 Message timestamps and delivery status

## Tech Stack 🛠️

- [![Next][next.js]][next-url]
- [![React][react.js]][react-url]
- [![PostgreSQL][postgresql]][postgresql-url]
- [![Prisma][prisma]][prisma-url]
- [![Pusher][pusher]][pusher-url]
- [![Tailwind CSS][tailwind-css]][tailwind-css-url]
- [![ImageKit][imagekit]][imagekit-url]
- [![Shadcn][shadcn]][shadcn-url]
- [![Vercel][vercel]][vercel-url]

## Getting Started 🚀

Follow these steps to set up the project locally.

### Prerequisites

- Node.js (v20+)
- Any code editor (VS Code recommended)

### Step 1: Install Project Dependencies

---

```bash
# 1. Clone the repo
git clone https://github.com/<your_username>/kwikchat.git

# 2. Navigate to the project directory
cd kwikchat

# 3. Install dependencies
npm install

# 4. Setup environment variables
cp .env.sample .env
```

> See [.env.sample](https://github.com/nilotpaldhar/kwikchat/blob/main/.env.sample) for required environment keys.

### Step 2: Configure Prisma & PostgreSQL

---

```bash
# 1. Add your PostgreSQL connection string in .env
DATABASE_URL="postgresql://username:password@localhost:5432/kwikchat"

# 2. Generate the Prisma client
npm run db:generate

# 3. Run database migrations
npm run db:migrate
```

Add real-time functionality to your chat app using Pusher Channels — allowing users to send and receive messages instantly ⚡

1. **Create a Pusher account**  
   Sign up at [pusher.com](https://pusher.com) if you don’t already have one.

2. **Create a new Pusher app**

   - Go to your [Pusher dashboard](https://dashboard.pusher.com/)
   - Click “Create App”
   - Choose an app name, select a cluster (e.g., `ap2`), and set the frontend/backend technology (can be anything)

3. **Get your credentials**  
   From the app settings page, note the following values:

   - `APP ID`
   - `APP KEY`
   - `APP SECRET`
   - `CLUSTER`

4. **Configure environment variables**  
   Open your `.env` file and add the following lines (replace with your actual values):

   ```bash
   PUSHER_APP_ID="<your_pusher_app_id>"
   NEXT_PUBLIC_PUSHER_APP_KEY="<your_pusher_app_key>"
   PUSHER_APP_SECRET="<your_pusher_app_secret>"
   NEXT_PUBLIC_PUSHER_APP_CLUSTER="<your_pusher_app_cluster>"
   ```

### **Step 5: Integrate ImageKit for Media Handling**

---

Enable fast and optimized image uploads and delivery using **ImageKit** — a powerful media management and CDN platform 🚀

1. **Create an ImageKit account**  
   Sign up at [imagekit.io](https://imagekit.io) if you haven't already.

2. **Create a new ImageKit project**

   - After logging in, go to the **Developer Settings** section
   - Locate your **Public Key**, **Private Key**, and **URL Endpoint**

3. **Update your `.env` file**  
   Add the following environment variables using your credentials:
   ```bash
   IMAGE_KIT_PRIVATE_KEY="<your_image_kit_private_key>"
   NEXT_PUBLIC_IMAGE_KIT_PUBLIC_KEY="<your_image_kit_public_key>"
   NEXT_PUBLIC_IMAGE_KIT_URL_ENDPOINT="<your_image_kit_url_endpoint>"
   ```

### **Step 6: Seed the Database**

---

Populate your database with initial test data to help you get up and running quickly.

Run the following command in your project root:

```bash
npm run db:seed
```

## Deployment 🚀

KwikChat is ready to deploy on [Vercel](https://vercel.com). Just connect your GitHub repo and add the required environment variables.

> For more info, refer to the [Next.js deployment docs](https://nextjs.org/docs/deployment).

## Contribution 🤝

KwikChat is open source and contributions are welcome. Check out our [Code of Conduct](https://github.com/nilotpaldhar/test-app/blob/main/.github/community/CODE_OF_CONDUCT.md) and [Issues](https://github.com/nilotpaldhar/kwikchat/issues) page to get started.

## Support 💗

If you found this project helpful:

- ⭐ Star this repo on GitHub
- 💬 Share it with your network
- 📢 Give a shoutout on social media

## License 📄

This project is licensed under the [MIT License](https://github.com/nilotpaldhar/test-app/blob/main/LICENSE).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!--
KwikChat | Real-time messaging app using Next.js, Pusher, Prisma, PostgreSQL, Tailwind CSS, and Shadcn UI.
A modern, full-stack chat app designed to be responsive, scalable, and visually clean.
-->

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[next-url]: https://nextjs.org/
[react.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[react-url]: https://reactjs.org/
[postgresql]: https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white
[postgresql-url]: https://www.postgresql.org
[prisma]: https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white
[prisma-url]: https://www.prisma.io
[pusher]: https://img.shields.io/badge/Pusher-1A96F0?style=for-the-badge&logo=pusher&logoColor=white
[pusher-url]: https://pusher.com
[tailwind-css]: https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white
[tailwind-css-url]: https://tailwindcss.com
[imagekit]: https://img.shields.io/badge/ImageKit.io-0099E5?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDgiIGhlaWdodD0iNDgiIHZpZXdCb3g9IjAgMCAxMDIgMTAyIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxjaXJjbGUgY3g9IjUxIiBjeT0iNTEiIHI9IjUwIiBmaWxsPSIjZmZmIi8+PC9zdmc+&logoColor=white
[imagekit-url]: https://imagekit.io
[shadcn]: https://img.shields.io/badge/Shadcn_UI-111827?style=for-the-badge&logo=none&logoColor=white
[shadcn-url]: https://ui.shadcn.com
[vercel]: https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white
[vercel-url]: https://vercel.com
