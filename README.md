# Deliveroo-clone
Deliveroo Clone with REACT NATIVE! (Navigation, Implement Redux, Tailwind CSS &amp; Sanity.io, AWS Amplify, React Native Heroicons, )

Installing Expo CLI

npm install --global expo-cli
Initializing the project

npx create-expo-app deliveroo-clone
cd deliveroo-clone
Install dependencies

Setup Tailwind CSS


npm install tailwindcss-react-native
npm install --save-dev tailwindcss
Tailwindcss requires a tailwind.config.js file with the content section configured to include the paths to all of your components and any other source files that contain Tailwind class names.

// tailwind.config.js
module.exports = {
  content: [
    "./screens/**/*.{js,ts,jsx,tsx}",
    "./pages/**/*.{js,ts,jsx,tsx}",
    "./components/**/*.{js,ts,jsx,tsx}",
  ],
  // ...
};
Add TailwindProvider at the top level of your application. The TailwindProvider creates the context for reactive styles and the atomic style objects.

import { TailwindProvider } from "tailwindcss-react-native";

function MyAppsProviders({ children }) {
  return <TailwindProvider>{children}</TailwindProvider>;
}
Configure your babel.config.js
// babel.config.js
module.exports = {
  plugins: ["tailwindcss-react-native/babel"],
};
Install dependencies

🔶 Dependency Info

🏃 Run Locally


Clone the project

  git clone https://github.com/SashenJayathilaka/Deliveroo-Clone.git
change directory

  cd Deliveroo-Clone
Install dependencies

  npx expo install
Start the server

  npx expo start
Creating a Build
Optimize the assets for speed - npx expo-optimize (formerly expo optimize)
Bundle the project for production - npx expo export:web (expo build:web in the legacy Expo CLI).
Creates a production ready static bundle in the web-build/ directory. Don't edit this folder directly.
If you make any changes to your project, you'll need to re-build for production.
For more help use npx expo export:web --help
More Info
🚩 Deployment
To deploy this project run

Expo Publish


publish your project

expo publish
