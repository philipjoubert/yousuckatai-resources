# yousuckatai-resources

Hosting a Simple Website or Web App on Vercel

This guide will walk you through taking a website or web app designed in V0.dev, Bolt.new, or similar AI design tools and deploying it live for free on Vercel. Using this approach, you can quickly create and host a website or web app without any upfront costs.

Steps to Deploy Your Site

Step 1: Build Your Site in V0.dev / Bolt.new

	1.	Use V0.dev or Bolt.new to design your website.
	2.	Export or save your project as a .tsx file compatible with Next.js.

Step 2: Local Machine Setup

To run Next.js locally, set up your development environment. Instructions differ for macOS and Windows:

macOS

	1.	Install Homebrew (if not already installed):

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"


	2.	Install Node.js:

brew install node



Windows

	1.	Install Node.js:
	•	Download the installer from Node.js and follow the setup steps.
	2.	Optional: Install Windows Subsystem for Linux (WSL) for a smoother development experience:
	•	Open PowerShell as Administrator and run:

wsl --install


	•	Then install your preferred Linux distribution from the Microsoft Store.

	3.	Install Git (if not already installed):
	•	Download from Git for Windows and follow the installation steps.

Step 3: Set Up a New Next.js Project

	1.	Create a new Next.js app:

npx create-next-app@14


	2.	Open the project in Cursor or your preferred editor.
	3.	Install ShadCN components:
	•	Initialize ShadCN in your project:

npx shadcn init


	•	Install individual components as needed. For example, to add a Button component:

npx shadcn add button


	4.	Run the development server to ensure everything is working:

npm run dev

	Note: If any component installation issues arise with ShadCN, refer to the ShadCN documentation for specific setup instructions.

	5.	Copy over your code from the exported .tsx file to integrate it into the project structure.

Step 4: Set Up GitHub for Version Control

	1.	Create a new GitHub repository by navigating to GitHub and selecting New Repository.
	2.	Link your local Next.js project to the new GitHub repository. After creating the repository, GitHub will provide setup instructions. Use the following commands to set the remote origin and push your project:

git init
git add .
git commit -m "Initial commit"
git remote add origin <YOUR_REPOSITORY_URL>
git push -u origin main

Replace <YOUR_REPOSITORY_URL> with the URL from GitHub, which appears after creating the new repository.

Step 5: Deploy to Vercel

	1.	Create a new project on Vercel:
	•	Go to Vercel and select New Project.
	•	Link it to your GitHub repository and follow the prompts to deploy.
	2.	Your site is live! 🎉 Visit your Vercel dashboard to view the deployment status.

Optional: Set Up a Custom Domain

	1.	In Vercel, navigate to the Domains tab and add your custom domain.
	2.	Follow Vercel’s instructions to update your DNS settings.

This setup should guide you from design to deployment with minimal fuss. Enjoy your newly live website or web app!
