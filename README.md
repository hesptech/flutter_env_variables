# Flutter hide variables from git repository.

An Application prototype built with Dart and Flutter.

## Overview

### Features

- Hide information for variables in code that should not be uploaded to git repositories;

### Dependencies

| Package               | Purpose                                                                                                                    |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| flutter_dotenv        | Load configuration at runtime from a .env file which can be used throughout the application.                               |


## Building

You can follow these instructions to build the app and install it onto your device.

### Prerequisites

If you are new to Flutter, please first follow the [Flutter Setup](https://flutter.dev/setup/) guide.

### Downloading and installing the Flutter app

```
git clone https://github.com/hesptech/flutter_env_variables.git
cd flutter_env_variables
flutter run
```

The `flutter run` command both builds and installs the Flutter app to your device or emulator.

### How to configure and set up

Before using/testing the application, you need to have run the inline flutter pub get command in the terminal, to make sure it has installed the flutter_dotenv package.

Apart from the following steps to create the file locally with the content that should not be uploaded to git repositories, all the necessary configuration setup is already done in the app. This includes adding in the pubspec.yaml file the dependencie of the package and the assets file path of the file, plus adding the code to load/initialize in the main.dart file.

Further info on the flutter_dotenv package from pub.dev, are provided at [here](https://pub.dev/packages/flutter_dotenv).

Follow this step by step on how to use the application:

1. Run the following inline command: 
flutter pub get: 
in the terminal, to make sure it has installed the flutter_dotenv package:

2. Create a .env file in the root of your project, which will remain only on the local repository:

2. Add the following content in the .env file you just created:

```
...
FOO=foo
BAR=bar
FOOBAR=$FOO$BAR
ESCAPED_DOLLAR_SIGN='$1000'
# This is a comment
...
```

3. That should be it, now you can run the app:

## terminal online cmd 

```
flutter run
```

support info: olea.oswaldo@gmail.com