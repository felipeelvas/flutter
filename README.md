# flutter
Introdução ao desenvolvomento do Flutter
Flutter is an open-source UI software development toolkit created by Google. It is used to develop applications for Android, iOS, Linux, Mac, Windows, Google Fuchsia, and the web from a single codebase.

Here’s a simple example to get you started with Flutter. This example demonstrates how to create a basic Flutter app that displays a centered "Hello, World!" text.

### Step-by-Step Guide:

1. **Install Flutter**:
   - Follow the instructions on the official Flutter [Get Started](https://flutter.dev/docs/get-started/install) page to install Flutter on your machine.

2. **Set Up an Editor**:
   - You can use any text editor, but Visual Studio Code is highly recommended because it has excellent Flutter support. Install the Flutter and Dart plugins for Visual Studio Code.

3. **Create a New Project**:
   - Open a terminal and run the following command to create a new Flutter project:
     ```sh
     flutter create hello_world
     ```
   - Navigate into the project directory:
     ```sh
     cd hello_world
     ```

4. **Edit `main.dart`**:
   - Open the `lib/main.dart` file and replace its content with the following code:
     ```dart
     import 'package:flutter/material.dart';

     void main() {
       runApp(MyApp());
     }

     class MyApp extends StatelessWidget {
       @override
       Widget build(BuildContext context) {
         return MaterialApp(
           home: Scaffold(
             appBar: AppBar(
               title: Text('Hello World App'),
             ),
             body: Center(
               child: Text('Hello, World!'),
             ),
           ),
         );
       }
     }
     ```

5. **Run the App**:
   - Ensure a device emulator is running or connect a physical device.
   - Run the app using the following command:
     ```sh
     flutter run
     ```

### Explanation:

- **Importing Flutter Package**: 
  ```dart
  import 'package:flutter/material.dart';
  ```
  This line imports the Flutter material package which contains pre-designed widgets and tools.

- **Main Function**: 
  ```dart
  void main() {
    runApp(MyApp());
  }
  ```
  The main function is the entry point of the app. It calls the runApp function with our custom widget, MyApp.

- **MyApp Widget**: 
  ```dart
  class MyApp extends StatelessWidget {
    @override
    Widget build(BuildContext context) {
      return MaterialApp(
        home: Scaffold(
          appBar: AppBar(
            title: Text('Hello World App'),
          ),
          body: Center(
            child: Text('Hello, World!'),
          ),
        ),
      );
    }
  }
  ```
  MyApp is a stateless widget. It returns a MaterialApp which sets up the basic structure of the app. Inside it, Scaffold provides the app structure with an AppBar and a body. The body contains a Center widget that centers its child widget, which in this case is a Text widget displaying "Hello, World!".

This simple example should help you get started with Flutter. You can expand upon this by exploring more widgets and Flutter features. For more detailed information and tutorials, you can visit the [official Flutter documentation](https://flutter.dev/docs).
