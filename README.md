# flutter_multi_select_items
https://pub.dev/packages/flutter_multi_select_items

This is a custom fork of the original package `flutter_multi_select` to address the deprecation and removal of `bodyText1` from `TextTheme`.

## Changes Made

### Fixed Issue: Deprecated `bodyText1`

The Flutter framework has deprecated `bodyText1` in favor of `bodyLarge`. As a result, any reference to `bodyText1` has been updated to ensure compatibility with the latest version of Flutter.

**Original:**

```dart
Text(
  'Example Text',
  style: Theme.of(context).textTheme.bodyText1,
)
```

**Updated:**

```dart
Text(
  'Example Text',
  style: Theme.of(context).textTheme.bodyLarge,
)
```

## How to Use This Fork

To use this fixed version of the package in your Flutter project, add the following to your `pubspec.yaml` file:

```yaml
dependencies:
  package_name:
    git:
      url: https://github.com/larakreisz/flutter_multi_select.git
      ref: master
```
