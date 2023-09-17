# Astro-Github-Card Component

The Astro-Github-Card component is a reusable component built with Astro that displays information about a GitHub repository in a visually appealing card format. It fetches repository details using the GitHub API and displays them in a user-friendly manner.

<p align="center">
  <img width="65%" height="65%" src="https://github.com/Kons-5/Astro-Github-Cards/blob/main/public/example.png">
</p>

## Running the Example

To run the example and see the Astro-Github-Card component in action, follow these steps:

### 1. Install Dependencies

Before you can run the example, make sure you have Node.js and npm (Node Package Manager) installed on your computer.
Once Node.js and npm are installed, open your terminal or command prompt and navigate to the project directory containing the `package.json` file.

```bash
npm install
```
This command will download and install the required packages, including Axios for making HTTP requests and any other project-specific dependencies.
After the dependencies are successfully installed, you can start the development server. Run the following command:

```bash
npm run dev
```
This command will start the Astro development server and compile your project. It will also open a local development environment, usually at http://localhost:3000, in your web browser.
## Features

- Displays the repository name, description, and primary programming language.
- Shows the number of stars and forks for the repository.
- Provides a link to the GitHub repository.

## Usage

To use the Astro-Github-Card component in your Astro project, follow these steps:

1. Copy the `Card.astro` and `CardList.astro` files to your project directory.

2. Import the `CardList` component in your Astro page where you want to display GitHub repository cards.

   ```astro
   import CardList from "../path-to-CardList.astro";

3. Define an array of GitHub repository URLs that you want to display using the Card component. Replace the URLs in the array with your own repository URLs.

```astro
const repoUrls = [
  "https://github.com/your-username/your-repo-1",
  "https://github.com/your-username/your-repo-2",
  // Add more repository URLs as needed
];
```
4. Render the CardList component in the designated page.
```astro

<CardList/>
```
5. Start your Astro development server to see the GitHub repository cards in action.

## Customization
You can customize the appearance of the GitHub repository cards by modifying the CSS styles in the Card.astro file. Feel free to adjust colors, fonts, margins, and other styles to match your project's design.

## Laguage Colors
The component fetches language colors from the following repository using Axios:
- [ozh/github-colors](https://github.com/ozh/github-colors)

## Dependencies
- [Axios](https://axios-http.com/): Used for making HTTP requests to fetch repository language colors.
- [Font Awesome](https://fontawesome.com/): Used for icons (make sure to include the Font Awesome kit script).
