# Hosting a Simple Website or Web App on Vercel

This guide will walk you through taking a website or web app designed in **V0.dev**, **Bolt.new**, or similar AI design tools and deploying it live for free on **Vercel**. Using this approach, you can quickly create and host a website or web app without any upfront costs. If you get stuck somewhere, just ask ChatGPT or Claude 👾

---

## Steps to Deploy Your Site

### Step 1: Build Your Site in V0.dev / Bolt.new

Use your favorite AI tools like [V0.dev](https://v0.dev/), [Bolt.new](https://bolt.new/) or [Magic Patterns](https://www.magicpatterns.com/) to prototype your website.

---

### Step 2: Local Machine Setup

To run Next.js locally, you need to do a once-off set up of your development environment. 

Exact instructions differ for **macOS** and **Windows**, so ask your favourite LLM how to install [Node.js](https://nodejs.org/)

---

### Step 3: Set Up a New Next.js Project

1. Create a new Next.js app:

```
npx create-next-app@14
```

2. Open the project in any text editor or IDE. I recommend [Cursor](https://www.cursor.com/)
3. Install ShadCN components:

Initialize ShadCN in your project:
```
npx shadcn init
```

Install individual components as needed. For example, to add a Button component:

```
npx shadcn add button
```

Run the development server to ensure everything is working:

```
npm run dev
```

Note: If any component installation issues arise with ShadCN, refer to the ShadCN documentation for specific setup instructions.

Copy over your code from the exported .tsx file to integrate it into the project structure.

---

### Step 4: Set Up GitHub for Version Control

1.	Create a new GitHub repository by navigating to GitHub and selecting New Repository.
2.	Link your local Next.js project to the new GitHub repository. After creating the repository, GitHub will provide setup instructions. Use the following commands to set the remote origin and push your project:

```
git init
git add .
git commit -m "Initial commit"
git remote add origin <YOUR_REPOSITORY_URL>
git push -u origin main
```

Replace <YOUR_REPOSITORY_URL> with the URL from GitHub, which appears after creating the new repository.

---

### Step 5: Deploy to Vercel

1.	Create a new project on Vercel:
	* Go to Vercel and select New Project.
 	* Link it to your GitHub repository and follow the prompts to deploy.
2.	Your site is live! 🎉 

---

### Optional: Set Up a Custom Domain

1. In Vercel, navigate to the Domains tab and add your custom domain.
2. Follow Vercel’s instructions to update your DNS settings.

Enjoy your newly live website or web app!

