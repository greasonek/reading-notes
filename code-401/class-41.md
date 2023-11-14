# Class 41 Reading Notes

## Getting Started with React Native

1. Name three Core Components of React Native and describe what they do.

- < View > = a container that supports layout with flexbox, style and some touch handling as well as accessibility controls
- < ScrollView > = a generic scrolling container that contains multiple components and views
- < TextInput > = allows users to enter text

2. What problem does React Native solve (why call it native)?

- It's called native because the apps are not purely web-based or built with web technologies but use native components of the platforms. It therefore solves cross platform development because the apps can be run on both Android and iOS platforms reducing the need for separate codebases.

3. What are the building blocks of a React Native app? How does that compare to a React app?

- Building blocks include components, JSX, state and props. React has similar building blocks, however native allows for platform specific code and modules to interact with native APIs and react does not allow for direct access to native APIs.

## Expo

1. What solution does expo provide?

- Simplifies the set up process for React Native projects and comes with development env that allows to run and test apps directly on the device.

2. Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the _MANAGED_ workflow.

3. What is the difference between React Native and Expo?

- Expo provides a simplified workflow for quick development while React Native has more flexibility and more control over native code.

## Expo Snack

1. Checkout this tool. What does snack allow you to do?

- Allows you to protoype an app and view it in a web browser.

## Ejecting

1. What does “eject” mean within the context of Expo?

- Eject means leaving the standard Expo dev env and moving to a bare workflow where you have access and cotrol over the project, or to ExpoKit.

2. When should you not eject?

- When in the early stages of development with rapid prototyping, when building a simple app that uses built in native modules without much customization, when you want reduced maintenance.

3. Why might you choose to eject?

- When the project requires more customization, when you want more dependency control, when you want full access and control over the building process.
