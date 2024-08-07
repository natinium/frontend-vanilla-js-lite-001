Sure! Here's a `README.md` file based on your project structure and setup. It includes usage instructions for setting up the project, compiling SCSS, linting JavaScript files, and formatting code with Prettier.

```markdown
# Your Project Title

Welcome to your project! This project is a vanilla frontend setup using HTML, SCSS, and JavaScript without any build tools or bundlers.

## Project Structure

```
project-root/
│
├── index.html
├── styles/
│   ├── main.scss
│   └── _variables.scss
├── scripts/
│   └── main.js
├── package.json
├── .eslintrc.json
├── .prettierrc
├── .prettierignore
└── node_modules/
```

## Setup

### Prerequisites

- Node.js and npm installed on your machine.

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

## Usage

### SCSS Compilation

This project uses Dart Sass to compile SCSS to CSS. You can run the following commands to compile your SCSS files:

- **Development (Watch Mode):**
    ```sh
    npm run sass
    ```

- **Production (Build):**
    ```sh
    npm run sass:build
    ```

### Linting and Formatting

This project uses ESLint and Prettier for linting and formatting JavaScript code.

- **Lint JavaScript files:**
    ```sh
    npm run lint
    ```

- **Fix linting errors:**
    ```sh
    npm run lint:fix
    ```

- **Format code with Prettier:**
    ```sh
    npm run format
    ```

## File Descriptions

- **index.html**: The main HTML file.
- **styles/**: This folder contains all SCSS files.
    - `main.scss`: Main SCSS file where other SCSS partials are imported and main styles are written.
    - `_variables.scss`: Partial SCSS file for variables.
- **scripts/**: This folder contains JavaScript files.
    - `main.js`: Main JavaScript file.
- **package.json**: Contains the project configuration and dependencies.
- **.eslintrc.json**: ESLint configuration file.
- **.prettierrc**: Prettier configuration file.
- **.prettierignore**: Files and directories ignored by Prettier.

## Example Code

### HTML (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Project Title</title>
    <link rel="stylesheet" href="styles/main.css">
</head>
<body>
    <div class="container">
        <header>
            <h1>Welcome to Our Service</h1>
        </header>
        <main>
            <p>Discover amazing features and boost your productivity.</p>
            <button id="getStarted" class="btn btn-primary">Get Started</button>
        </main>
    </div>
    <script src="scripts/main.js"></script>
</body>
</html>
```

### SCSS (`styles/main.scss`)

```scss
@import 'variables';

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: $font-family;
    line-height: 1.6;
    color: $text-color;
    background-color: $bg-color;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
}

.container {
    text-align: center;
    padding: 2rem;
    max-width: 600px;
}

h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    color: $primary-color;
}

p {
    font-size: 1.1rem;
    margin-bottom: 2rem;
}

.btn {
    padding: 0.8rem 1.5rem;
    font-size: 1rem;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: all 0.3s ease;

    &-primary {
        background-color: $button-color;
        color: white;

        &:hover {
            background-color: darken($button-color, 10%);
            transform: translateY(-2px);
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
    }
}
```

### SCSS Variables (`styles/_variables.scss`)

```scss
// Colors
$primary-color: #2c3e50;
$bg-color: #ecf0f1;
$text-color: #333;
$button-color: #3498db;

// Typography
$font-family: 'Arial', sans-serif;

// Breakpoints
$breakpoint-sm: 576px;
$breakpoint-md: 768px;
$breakpoint-lg: 992px;
$breakpoint-xl: 1200px;
```

### JavaScript (`scripts/main.js`)

```js
document.addEventListener('DOMContentLoaded', function() {
    const getStartedBtn = document.getElementById('getStarted');

    getStartedBtn.addEventListener('click', function() {
        alert('Welcome! You\'re all set to get started.');
    });
});
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

Feel free to adjust the contents and sections to better fit your project's specifics.
