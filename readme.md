setup
1. Initialize npm project
    npm init
Press Enter multiple times to skip the custom configuration.

2. Install Tailwind CSS CLI
    npm install tailwindcss @tailwindcss/cli

3. Create Project Structure
Create the following folder structure because we using GitHub:
    /docs
      └── input.css

4. Configure Tailwind
In docs/input.css, add the following line:
    @import "tailwindcss";

5. Create Your HTML File
Create your HTML file in the /docs folder or root directory.

6. Compile Tailwind CSS
To compile your CSS, run:
    npx @tailwindcss/cli -i ./docs/input.css -o ./docs/output.css --watch
This will continuously rebuild your CSS as you make changes.

7. Add Script to package.json (Optional but Recommended)
Instead of typing the long command every time, update your package.json:

"scripts": {
  "dev": "npx @tailwindcss/cli -i ./docs/input.css -o ./docs/output.css --watch"
}

Now you can just run: "npm run dev"