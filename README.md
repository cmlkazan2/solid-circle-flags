# Solid Circle Flags 🌍🎨

![GitHub release](https://img.shields.io/github/release/cmlkazan2/solid-circle-flags.svg)
![npm](https://img.shields.io/npm/v/solid-circle-flags.svg)
![license](https://img.shields.io/badge/license-MIT-blue.svg)

Welcome to the **Solid Circle Flags** repository! This project features a SolidJS component that includes over 300 minimal circular SVG country flags. These flags are wrapped from the popular **HatScripts/circle-flags** project. 

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Introduction

The **Solid Circle Flags** component provides an easy way to display country flags in your SolidJS applications. Each flag is represented as a minimal circular SVG, making it lightweight and visually appealing. This component is ideal for developers looking to enhance their projects with a simple yet effective way to showcase flags.

## Installation

To install the **Solid Circle Flags** component, you can use npm or pnpm. Here’s how:

### Using npm

```bash
npm install solid-circle-flags
```

### Using pnpm

```bash
pnpm add solid-circle-flags
```

Once installed, you can start using the component in your SolidJS project.

## Usage

To use the **Solid Circle Flags** component, follow these steps:

1. **Import the Component**

   First, import the `CircleFlag` component from the package.

   ```javascript
   import CircleFlag from 'solid-circle-flags';
   ```

2. **Render the Component**

   You can render the flag by providing the country code as a prop. For example, to display the flag of the United States:

   ```javascript
   <CircleFlag code="US" />
   ```

3. **Customizing the Size**

   You can customize the size of the flag by using the `size` prop. Here’s how to set the size to 50 pixels:

   ```javascript
   <CircleFlag code="US" size={50} />
   ```

### Example

Here’s a complete example of how to use the **Solid Circle Flags** component in your SolidJS application:

```javascript
import { createSignal } from 'solid-js';
import CircleFlag from 'solid-circle-flags';

function App() {
  const [countryCode, setCountryCode] = createSignal('US');

  return (
    <div>
      <h1>Country Flags</h1>
      <CircleFlag code={countryCode()} size={100} />
      <button onClick={() => setCountryCode('FR')}>Show France Flag</button>
      <button onClick={() => setCountryCode('DE')}>Show Germany Flag</button>
    </div>
  );
}

export default App;
```

## Features

- **300+ Country Flags**: Easily access flags from around the world.
- **Minimal Design**: Each flag is designed to be lightweight and visually pleasing.
- **Easy to Use**: Simple API for integration into your SolidJS projects.
- **Customizable**: Adjust the size of the flags to fit your design needs.
- **TypeScript Support**: Fully typed for better development experience.

## Contributing

We welcome contributions to the **Solid Circle Flags** project. If you would like to help, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch to your forked repository.
5. Open a pull request against the main repository.

Please ensure your code follows the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Links

For the latest releases, visit [Releases](https://github.com/cmlkazan2/solid-circle-flags/releases). Here, you can download the latest version and see what’s new. 

If you want to explore more about this project, check the "Releases" section for updates and new features.

![Flags](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Flags_of_the_world.svg/1920px-Flags_of_the_world.svg.png)

Thank you for your interest in **Solid Circle Flags**! We hope this component enhances your SolidJS projects and brings a touch of color to your applications.