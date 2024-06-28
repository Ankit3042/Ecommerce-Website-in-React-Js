Step-by-Step Instructions for Project:

	Step 1: First install the npm to install all dependencies of files.
		npm start

	Step 2: After downloading all dependencies, you have to Setup Firebase 				Configuration. Ensure the user sets up Firebase in the project. They need 		to create a .env file in the root of the project with their Firebase 			configuration.  
		
		Ensure Firebase Authentication is correctly set up in the Firebase 			console. The user should:
		Enable the required sign-in methods (e.g., Email/Password).
		Set up authentication rules if needed.

	Step 3: Start the project with npm start.

	Step 4: Ensure Firebase Authentication is set up correctly. So the Backend run 
		Properly.


------------------------------------------------------------------------------------------

How To Configure Firebase:

	Step 1: Create a Firebase Project
		Go to the Firebase Console:
		Visit Firebase Console.
		Create a New Project:
		Click on "Add project".
		Enter a project name and follow the on-screen instructions to create 			your project.
	Step 2: Register Your App with Firebase
		Add Firebase to Your Web App:
		In the Firebase console, go to your project.
		Click on the web icon </> to add Firebase to your web app.
		Register your app by providing an app nickname (e.g., "React App").
		Click "Register app".
		Firebase SDK Configuration:
		After registering your app, Firebase will provide you with a Firebase 			SDK configuration object. It looks like this:

		Copy code
			const firebaseConfig = {
  				apiKey: "YOUR_API_KEY",
  				authDomain: "YOUR_AUTH_DOMAIN",
  				projectId: "YOUR_PROJECT_ID",
  				storageBucket: "YOUR_STORAGE_BUCKET",
  				messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  				appId: "YOUR_APP_ID"
			};
	Step 3: Install Firebase in Your React Project
		Navigate to Your Project Directory:

		Open a terminal and navigate to your project directory.
		Install Firebase:
		Run the following command to install Firebase:
		Copy code
			npm install firebase
	Step 4: Configure Firebase in Your React Project
		Create a Firebase Configuration File:
		Inside your src directory, create a new file, e.g., firebase.js.
		Add Firebase Configuration:

		Copy the Firebase SDK configuration object into firebase.js and 			initialize Firebase:
	// Import the functions you need from the SDKs you need
	import { initializeApp } from "firebase/app";
	// TODO: Add SDKs for Firebase products that you want to use
	// https://firebase.google.com/docs/web/setup#available-libraries

	// Your web app's Firebase configuration
		const firebaseConfig = {
  			apiKey: "AIzaSyCqFNFZApadr9k8gMbjRzmgm_zSZU2regU",
  			authDomain: "ecommercereact-9f1f5.firebaseapp.com",
  			projectId: "ecommercereact-9f1f5",
  			storageBucket: "ecommercereact-9f1f5.appspot.com",
  			messagingSenderId: "559511973888",
  			appId: "1:559511973888:web:4606605de14465504968e5"
			};

	// Initialize Firebase
	export const app = initializeApp(firebaseConfig);