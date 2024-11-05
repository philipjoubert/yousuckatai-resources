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

You'll be asked a few questions. I recommend answering them as follows:

* *What is your project named?* the_name_of_your_app
* *Would you like to use TypeScript?* Yes
* *Would you like to use ESLint?* No
* *Would you like to use Tailwind CSS?* Yes
* *Would you like to use `src/` directory?* No
* *Would you like to use App Router? (recommended)* Yes
* *Would you like to customize the default import alias (@/*)?* No

2. Open the project in any text editor or IDE. I recommend [Cursor](https://www.cursor.com/)

3. Run the development server to ensure everything is working:

```
npm run dev
```
By default your website will be available at: [http://localhost:3000](http://localhost:3000)

---

### Step 4: Add your website content

1. Next you'll want to copy the code from your AI coding tool (e.g. v0.dev) to your Next.js app. For a single page website, you're specifically looking to replace the contents of the page.tsx file.

2. Assuming you're running your web server, you'll probably get a bunch of errors due to missing ShadCN components or icons.

3. Install ShadCN components

Initialize ShadCN in your project:
```
npx shadcn init
```

Install individual components as needed. For example:

```
npx shadcn@latest add button
npx shadcn@latest add input
npx shadcn@latest add form
npx shadcn@latest add card
```

### Step 5: Set Up GitHub for Version Control

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

### Step 6: Deploy to Vercel

1.	Create a new project on Vercel:
	* Go to Vercel and select New Project.
 	* Link it to your GitHub repository and follow the prompts to deploy.
2.	Your site is live! 🎉 

---

### Optional: Set Up a Custom Domain

1. In Vercel, navigate to the Domains tab and add your custom domain.
2. Follow Vercel’s instructions to update your DNS settings.

Enjoy your newly live website or web app!

