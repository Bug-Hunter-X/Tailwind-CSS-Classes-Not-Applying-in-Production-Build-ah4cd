# Tailwind CSS Production Build Issue

This repository demonstrates a bug where Tailwind CSS classes fail to apply in a production build, despite working correctly during development. The issue arises from a misconfiguration in how Tailwind is integrated into the production build process, which can be resolved by ensuring correct purge configuration and build process for production.

## Setup

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm run build` to build for production. 
5. Open the `dist/index.html` file in your browser. Observe that the Tailwind classes do not work. 

## Bug Description

The bug is that Tailwind CSS classes are not applied to elements in production. The classes are correctly applied during the development process. This is likely due to an issue with how Tailwind is configured and/or how the production build process handles the CSS files.

## Solution

The solution involves properly configuring the `purge` option in your Tailwind CSS configuration to correctly identify and include the necessary CSS classes in your production build.  This ensures that only the used classes are included, preventing unused styles from being removed.