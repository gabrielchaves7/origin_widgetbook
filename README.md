# Origin Widgetbook

Origin Widgetbook is the project where you can open, see and play with the components from origin design system. This will help you to visualize and test the components from origin design system.

## Getting Started 🚀

### Flutter

The first thing you need is to setup flutter, please follow the steps:

1. https://docs.flutter.dev/get-started/install
2. https://docs.flutter.dev/get-started/editor

### Running the project
To run the project either use the launch configuration in VSCode/Android Studio or use the following command:

```sh
$ flutter run --target lib/main.dart
```

## Continuous Integration 🤖
On each pull request and push, the CI will automatically publish the updated widgetbook project to https://origin-widgetbook.netlify.app.

---

## How widgetbook integrates with the design system?
Each component at the design system is represented as a use case at the widgetbook, see **lib/widgetbook/usecase**. When you create a new component on the design system, you need to create a new usecase to display it on the widgetbook. This can be done following the steps:

1. Create the new usecase. You can use origin_icon_usecase.dart as example.
2. Run the command:
    ```flutter pub run build_runner build --delete-conflicting-outputs```