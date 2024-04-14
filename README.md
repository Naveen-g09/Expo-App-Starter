# Expo App Starter

Welcome to Expo App Starter, a template repository designed to kickstart your app building journey with Expo! This repository comes fully equipped with all the prerequisites configured for seamless development. From Tailwind CSS integration to CI/CD pipelines, EAS build setup, GitHub actions, commit checks, pre-commit checks, type checking, and Expo router - everything you need is right here.

## Prerequisites

Before getting started, ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [Yarn](https://yarnpkg.com/)
- [EAS (Preferred)](https://docs.expo.dev/build/introduction/)
- [Expo account](https://expo.dev/)

## Getting Started

To work with this starter template, follow these basic steps:

1. **Fork** this repository to your own GitHub account.
2. **Clone** the forked repository locally to your development environment.
3. **Navigate** into the cloned repository directory.
4. Run `yarn` to install all necessary dependencies. (Note: Yarn is also used for installation in GitHub actions. If you prefer using npm, update the configurations in `.github\workflows\preview.yml` and `.github\workflows\update.yml`).
5. Start your application by running `yarn start`. This will launch your application, and you can access it through the Expo Go app.

## Features

- **Tailwind CSS Integration**: Tailwind CSS is pre-configured for effortless styling.
- **CI/CD Pipelines**: Continuous Integration and Continuous Deployment pipelines are set up for streamlined development workflows.
- **EAS Build Setup**: Easily configure and build your Expo projects using Expo Application Services.
- **GitHub Actions**: Automated workflows using GitHub Actions ensure efficient development processes.
- **Commit Checks**: Automated checks are in place to ensure high-quality commits.
- **Pre-commit Checks**: Validate all files to ensure they adhere to ESLint and type safety standards.
- **Type Safety Check and Format**: Run commands like `yarn format` to format files and `yarn pre-commit` to check file integrity.

## Setting Up Expo GitHub Actions

To set up Expo GitHub Actions in the terminal, follow these steps:

1. Create an Expo account and install EAS CLI on your computer:
   ```
   npm install -g eas-cli
   eas login
   eas init
   ```

   Follow the prompts, using your Expo account, and overwrite the key when prompted.

2. Generate a personal access token:
   - Navigate to [Expo settings](https://expo.dev/settings/access-tokens).
   - Click "Create token" to generate a new personal access token.
   - Copy the token generated.

3. Add the access token as a secret in your GitHub repository:
   - Navigate to `https://github.com/your-username/your-repo-name/settings/secrets/actions`, replacing "your-username" and "your-repo-name" with your project's info.
   - Under "Repository secrets," click "New repository secret."
   - Create a secret with the name `EXPO_TOKEN`, and paste the copied access token as the value.

These steps will set up GitHub Actions for your Expo project.

## Personalizing the App

To personalize the app:

- **Single Theme**: Change `userInterfaceStyle` in `app.json` from automatic to light or dark.
- **Replace Icon**: Replace `icon.png` with your image to get your own logo for the app. Note that it's the icon for iOS and adaptive icon for Android.

Hope this is useful and speeds up your journey, happy coding!

## Contributing

We welcome contributions from the community! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

