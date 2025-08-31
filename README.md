# Prismic + Next.js Minimal Starter

Want to quickly get started building your own project with [Prismic][prismic] and [Next.js][nextjs]? This project includes basic configurations and nothing else. The project includes one Rich Text slice, a homepage, and a dynamic page.

- **Demo**: [Open live demo][live-demo]
- **Learn more about Prismic and Next.js**: [Prismic Next.js Documentation][prismic-docs]

&nbsp;

![Website screenshot](https://user-images.githubusercontent.com/31219208/228821412-fdde92b2-c13c-4287-b799-611fa96a5fd6.png)

&nbsp;

## 🚀 Quick Start

To start a new project using this starter:

1. Visit <https://prismic.io/dashboard>.
2. Create a new Prismic repository by selecting **Next.js**.
3. Select the **Minimal starter**.
4. Fill out your repository details and continue with the steps given in Prismic.

When you're ready to start your project, run the following command:

```sh
npm run dev
```


# 🌟 Fizzi Demo

Welcome to **Fizzi Demo** — a modern web application designed with scalability, performance, and clean UI in mind.  
The project is live at 👉 **[fizzi-demo.vercel.app](https://fizzi-demo.vercel.app/)**  

---

## 🌐 Live Demo
🚀 Check out the live app here:  
👉 **[https://fizzi-demo.vercel.app/](https://fizzi-demo.vercel.app/)**  

---

## ✨ Features
- ⚡ **Fast & Responsive** – Optimized for performance across all devices.  
- 🎨 **Modern UI** – Styled with **Tailwind CSS** for a clean, elegant interface.  
- 📱 **Mobile-First** – Works seamlessly on desktop, tablet, and mobile.  
- 🔄 **CMS Powered** – Content managed via **Prismic + Slice Machine**.  
- 🛠️ **Developer Friendly** – TypeScript, ESLint, Prettier, PostCSS included.  
- ☁️ **Deployed on Vercel** – Continuous deployment for every update.  

---

## 🛠️ Tech Stack
- **Framework:** [Next.js](https://nextjs.org/) + [React](https://react.dev/)  
- **CMS:** [Prismic](https://prismic.io/) with Slice Machine  
- **Styling:** [Tailwind CSS](https://tailwindcss.com/)  
- **Language:** TypeScript  
- **Linting & Formatting:** ESLint + Prettier  
- **Deployment:** [Vercel](https://vercel.com/)  

---

## 📂 Folder Structure

The project structure is modular and follows best practices:



## How to use your project

To edit the content of this project, go to [prismic.io/dashboard](https://prismic.io/dashboard), click on the repository for this website, and start editing.

### Create a page

To create a page, click on the green pencil icon, then select **Page**.

Pages are made of Slices. You can add and rearrange Slices to your pages.

Your new page will be accessible by its URL, but it won't appear on the website automatically. To let users discover it, add it to the navigation.

### Preview documents

If you chose this starter when you created a new repository from the Prismic Dashboard, then your repository is preconfigured with previews on localhost. To change the preview configuration or add previews to your production or staging environments, see [Preview Drafts in Next.js](https://prismic.io/docs/technologies/preview-content-nextjs) in the Prismic documentation.

### Customize this website

This website is preconfigured with Prismic. It has three Prismic packages installed:

- `@prismicio/client` provides helpers for fetching content from Prismic
- `@prismicio/react` provides React components for rendering content from Prismic
- `@prismicio/next` provides a wrapper component to configure Prismic previews

These packages are already integrated and employed in this app. Take a look at the code to see how they're used.

### Edit the code

There are two steps to rendering content from Prismic in your Next.js project:

1. Fetch content from the Prismic API using `@prismicio/client`.
2. Template the content using components from `@prismicio/react`.

Here are some of the files in your project that you can edit:

- `prismicio.ts` - This file includes configuration for `@prismicio/client` and exports useful API helpers.
- `app/layout.tsx` - This is your layout component, which includes configuration for `@prismicio/react` and `@prismicio/next`.
- `app/page.tsx` - This is the app homepage. It queries and renders a page document with the UID (unique identifier) "home" from the Prismic API.
- `app/[uid]/page.tsx` - This is the page component, which queries and renders a page document from your Prismic repository based on the UID.
- `slices/*/index.tsx` - Each Slice in your project has an index.tsx file that renders the Slice component. Edit this file to customize your Slices.

These are important files that you should leave as-is:

- `app/api/exit-preview/route.ts` - Do not edit or delete this file. This is the API endpoint to close a Prismic preview session.
- `app/api/preview/route.ts` - Do not edit or delete this file. This is the API endpoint to launch a Prismic preview session.
- `app/slice-simulator/page.tsx` - Do not edit or delete this file. This file simulates your Slice components in development.
- `slices/` - This directory contains Slice components, which are generated programmatically by Slice Machine. To customize a Slice template, you can edit the Slice's index.tsx file. To add Slices, delete Slices, or edit Slice models, use Slice Machine (more info below).

Learn more about how to edit your components with [Fetch Data in Next.js](https://prismic.io/docs/technologies/fetch-data-nextjs) and [Template Content in Next.js](https://prismic.io/docs/technologies/template-content-nextjs).

Learn more about how to use [TypeScript with Prismic](https://prismic.io/docs/typescript-nextjs).

### Deploy to the web

To put your project online, see [Deploy your Next.js App](https://prismic.io/docs/technologies/deploy-nextjs).

### Edit content models with Slice Machine

This project includes an application called Slice Machine, which generates models for your Custom Types and Slices. Slice Machine stores the models locally in your codebase, so you can save and version them. It also syncs your models to Prismic. To learn how to use Slice Machine, read [Model Content in Next.js](https://prismic.io/docs/technologies/model-content-nextjs).

If you change or add to your Custom Types, you'll need to update your route handling to match. To learn how to do that, read [Define Paths in Next.js](https://prismic.io/docs/technologies/define-paths-nextjs).

## Documentation

For the official Prismic documentation, see [Prismic's guide for Next.js][prismic-docs] or the [technical references for the installed Prismic packages](https://prismic.io/docs/technologies/technical-references).

## License

```
Copyright 2013-2022 Prismic <contact@prismic.io> (https://prismic.io)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

[prismic]: https://prismic.io/
[prismic-docs]: https://prismic.io/docs/technologies/nextjs
[prismic-sign-up]: https://prismic.io/dashboard/signup
[nextjs]: https://nextjs.org/
[live-demo]: https://nextjs-starter-prismic-minimal.vercel.app/


fizzi/
│
├── customtypes/                # Prismic Custom Types configurations
│
├── page/                       # Page level components or static pages
│
├── public/                     # Publicly accessible assets (images, fonts, etc.)
│
├── src/                        # Main source code
│   ├── components/             # Reusable UI components
│   ├── pages/                  # Application routes (Next.js pages)
│   ├── styles/                 # Global & modular styles
│   └── utils/                  # Helper functions & utilities
│
├── .gitignore                  # Git ignore rules
├── .prettierignore              # Prettier ignore rules
├── .prettierrc                  # Prettier configuration
├── LICENSE                      # Apache-2.0 license
├── README.md                    # Project documentation
├── eslint.config.mjs            # ESLint configuration
├── next.config.ts               # Next.js configuration
├── package-lock.json            # Auto-generated dependency lock file
├── package.json                 # Project dependencies & scripts
├── postcss.config.js            # PostCSS configuration
├── prismicio-types.d.ts         # Generated Prismic types
├── slicemachine.config.json     # Slice Machine configuration
├── tailwind.config.js           # Tailwind CSS configuration
└── tsconfig.json                # TypeScript configuration



---

## 📸 Screenshots

![Website screenshot](hero.png)

### 🏠 Homepage
![Homepage](images/homepage.png)

### 📱 Mobile View
![Mobile View](images/mobile.png)

### 📂 Folder View
![Folder Structure](images/folder-structure.png)

---

## 🚀 Getting Started

Follow these steps to run locally:

```bash
# Clone the repository
git clone https://github.com/your-username/fizzi.git
cd fizzi

# Install dependencies
npm install
# or
yarn install

# Start the development server
npm run dev
# or
yarn dev

# Open in browser
http://localhost:3000

📦 Deployment

The app is hosted on Vercel.
Each push to the main branch triggers an automatic deployment.

Live Deployment 👉 fizzi-demo.vercel.app

🤝 Contributing

Contributions are welcome!

Fork the repo

Create your feature branch: git checkout -b feature/new-feature

Commit changes: git commit -m 'Add new feature'

Push to branch: git push origin feature/new-feature

Open a Pull Request 🎉

📜 License

This project is licensed under the Apache-2.0 License.
See the LICENSE
 file for details.

👨‍💻 Author

Developed with ❤️ by Ashit



---

⚡ Suggestion: If you send me a couple of **screenshots of your app**, I can add them into the README properly with captions and placeholders already replaced.  

Do you want me to also design a **badges section** (like build status, license, framework logos) at the top for a more professional GitHub look?

