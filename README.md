# Tailwind_Template

### Installing Tailwind

npm install -D tailwindcss

npx tailwindcss init  -- **this is to create the tailwind.config.js, package-lock.json, package.json files**

## create index.css file and place  
@tailwind base;
@tailwind components;
@tailwind utilities;

## fill the tailwind.config.js the content section 
 content: [
    "./Mains/**/*.{html,js}",
    "./Componets/**/*.{html,js}",
  ],

## Create a script in package.json that initiates tailwind in place of 
"npx tailwindcss -i ./Mains/Index.css -o ./Dist/output.css --watch"
## package.json file
 "scripts": {
    "dev": "npx tailwindcss -i ./Mains/Index.css -o ./Dist/output.css --watch"
  }


