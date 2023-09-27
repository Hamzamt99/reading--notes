## React Native

**1. Name three Core Components of React Native and describe what they do.**

- **View**: The View component in React Native is similar to the `<div>` element in web development. It is used to structure and layout UI components, similar to a container. It can contain other components and is essential for creating the overall structure of a mobile app's user interface.

- **Text**: The Text component is used to display text in a React Native application. It allows you to style and format text, making it suitable for displaying headings, paragraphs, labels, and any other textual content within your app.

- **Image**: The Image component is used to display images in a React Native app. It can load and display local or remote images and provides options for resizing, caching, and handling image assets efficiently.

**2. What problem does React Native solve (why call it native)?**

React Native solves the problem of building mobile applications for multiple platforms (iOS and Android) using a single codebase. It is called "native" because it allows developers to create mobile apps with a native look and feel, as if they were developed using platform-specific languages like Swift (for iOS) and Java/Kotlin (for Android). React Native achieves this by using a common JavaScript codebase and a bridge that communicates with native modules on each platform. This approach enables developers to write most of the app's logic and UI using JavaScript while still achieving native performance and access to platform-specific features.

**3. What are the building blocks of a React Native app? How does that compare to a React app?**

**React Native App:**

- **Components**: React Native apps use mobile-specific components like View, Text, and Image for UI layout.
- **Navigator**: React Navigation or similar libraries are often used for navigation between screens in mobile apps.
- **StyleSheet**: React Native uses a special StyleSheet object to define styles for components, similar to CSS but with some differences due to platform constraints.
- **Native Modules**: React Native apps can utilize native modules to access device-specific features not available in JavaScript alone.
- **Platform-Specific Code**: Sometimes, platform-specific code or tweaks may be required for fine-tuning the app's behavior on iOS and Android.

**React Web App:**

- **Components**: React web apps use standard HTML elements (e.g., `<div>`, `<span>`) in addition to React components.
- **Router**: React web apps often use libraries like React Router for handling navigation and routing.
- **CSS**: Styling in React web apps is typically done using CSS, CSS-in-JS libraries, or CSS preprocessors.
- **Web APIs**: Web apps can access various browser APIs for features like geolocation, local storage, and more.
- **Platform Independence**: React web apps are platform-independent and run in web browsers, making them compatible with a wide range of devices.

# Expo: Simplifying Mobile App Development

## What solution does Expo provide?

Expo provides a comprehensive solution for developing and building mobile applications, primarily using React Native. It aims to simplify the development process and streamline app creation by offering various tools and services. Some key solutions Expo provides include:

- **Unified Development Environment**: Expo offers a unified development environment that includes a set of developer tools, a managed build service, and a mobile app client for testing your projects during development.

- **Pre-configured Native Modules**: Expo includes a curated set of pre-configured native modules and libraries that allow developers to access device features and services without the need for extensive native code integration.

- **Over-the-Air Updates**: Expo allows you to push updates to your app without going through the app store review process, making it easier to deploy changes and bug fixes.

- **Simplified Project Setup**: Expo eliminates much of the setup and configuration required for a React Native project, allowing developers to focus on writing code.

- **Expo Go**: The Expo Go app allows you to test your Expo projects on real devices quickly, without the need for complicated device setup.

## Expo's Managed Workflow

Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the **Managed** workflow. In the Expo Managed workflow, Expo takes care of many of the complex aspects of mobile app development, such as managing native dependencies, providing a unified development environment, and simplifying the build and deployment process. This allows developers to focus more on writing JavaScript code and less on the intricacies of native app development.

## Difference Between React Native and Expo

### React Native

- **Definition**: React Native is an open-source framework developed by Facebook for building mobile applications using JavaScript and React. It provides a foundation for creating cross-platform mobile apps that have a native look and feel. React Native allows you to write native modules when needed for platform-specific functionality.

### Expo

- **Definition**: Expo is a set of tools and services built on top of React Native to simplify the development process. Expo offers a managed workflow that abstracts many of the complexities of React Native development. It includes a set of pre-configured native modules and a build service. However, it also comes with some limitations, as it restricts you from using certain native modules and libraries that are not included in the Expo SDK.

In summary, Expo and React Native are related technologies, but developers can choose between them based on project requirements and the level of control and customization needed for their mobile apps.

