# maestro-tests
A collection of end-to-end automated UI test flows for mobile applications :
	•	Includes YAML-based flows targeting key user journeys, form validation, and regression checks.
	•	Optimized for maintainability and clarity, using robust selectors (testID/resource-id) and environment variables for reusability.
	•	Designed to run on Android and iOS emulators or real devices via CI or local development.

 Maestro Studio Setup Guide
 1. Prerequisites
	 •	Install Android Studio (for Android) and/or Xcode (for iOS) and set up your emulators/simulators.
	 •	Set your environment variables (e.g., `ANDROID_HOME` for Android devices).
 2. Install or Update Maestro (includes Studio)
   -> Open your terminal and run:
     curl -Ls "https://get.maestro.mobile.dev" | bash

   	•	If using Homebrew, you can upgrade with: brew upgrade maestro
 3. Add Maestro to PATH
     Add Maestro to your PATH if it’s not already:
     export PATH="$PATH:$HOME/.maestro/bin"
 Add this command to your shell profile file (like `.zshrc` or `.bashrc`).

 4. Verify Installation
   Check the version to confirm installation: maestro -v

 5. Launch Maestro Studio
   Start Maestro Studio from your terminal: maestro studio

 6. Run Tests
   You can now run your exported test: maestro test your_flow.yaml

