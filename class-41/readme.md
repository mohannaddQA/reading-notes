# Getting Started with React Native

## Core Components of React Native

1. **View**: The `View` component is like the `<div>` element in web development. It is used to structure and group other components and can be styled and customized to create various layouts.

2. **Text**: The `Text` component is used to display text in a React Native app. It can be styled and formatted just like regular text in web development.

3. **Image**: The `Image` component is used to display images. It supports various image formats and allows for resizing and customization.

## Problem Solved by React Native

React Native solves the problem of building mobile apps with a single codebase that can run on both iOS and Android platforms, while providing a native look and feel. It's called "native" because it allows developers to write code in JavaScript, but the resulting app uses native components and performance optimizations.

## Building Blocks of a React Native App

The building blocks of a React Native app include components like `View`, `Text`, and `Image`, as well as navigation components, state management libraries, and third-party modules. Compared to a React app, React Native includes platform-specific components and APIs for mobile development, while React for web focuses on web-specific components and APIs.

---

# Expo

## Solution Provided by Expo

Expo provides a simplified development environment and toolset for building React Native apps. It offers pre-configured templates, easy access to native modules, and a development server, making it easier for developers to get started with mobile app development.

## Expo Workflow

Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the "managed" workflow.

## Difference Between React Native and Expo

React Native is the underlying framework for building mobile apps, while Expo is a set of tools and libraries that simplify the development process. Expo can be seen as a higher-level abstraction that sits on top of React Native. While Expo simplifies development, it may limit access to certain native modules and require "ejecting" for more advanced customization.

---

# Expo Snack

## Expo Snack

Expo Snack is an online tool provided by Expo that allows you to write and run React Native code in your web browser. It's a convenient way to quickly prototype and test React Native components and features without setting up a development environment.

---

# Ejecting

## Ejecting in the Context of Expo

"Ejecting" in the context of Expo refers to the process of transitioning from the Expo managed workflow to the "bare" workflow. When you eject from Expo, you gain more control over your project configuration, but you also take on more responsibility for managing native dependencies and builds.

## When Not to Eject

You should avoid ejecting from Expo if you prefer the simplicity of the managed workflow and do not need advanced customizations or access to specific native modules.

## Reasons to Eject

You might choose to eject from Expo when you require more control over the native code, need to add custom native modules, or want to integrate with third-party libraries that are not supported in the managed workflow.
