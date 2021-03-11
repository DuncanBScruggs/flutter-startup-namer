# startup_namer

A new Flutter project. 

Simple app that generates proposed names for a startup company. The user can select and unselect names, saving the best ones. The code lazily generates 10 names at a time. As the user scrolls, more names are generated. There is no limit to how far a user can scroll.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Accomplished in [Part 1](https://flutter.dev/docs/get-started/codelab)

- Created a Flutter app from the ground up.
- Written Dart code.
- Leveraged an external, third-party library.
- Used hot reload for a faster development cycle.
- Implemented a stateful widget.
- Created a lazily loaded, infinite scrolling list.

## [part 2](https://codelabs.developers.google.com/codelabs/first-flutter-app-pt2#0)


## Notes

1. The itemBuilder callback is called once per suggested word pairing, and places each suggestion into a ListTile row. For even rows, the function adds a ListTile row for the word pairing. For odd rows, the function adds a Divider widget to visually separate the entries. Note that the divider might be difficult to see on smaller devices.

2. Add a one-pixel-high divider widget before each row in the ListView.

3. The expression i ~/ 2 divides i by 2 and returns an integer result. For example: 1, 2, 3, 4, 5 becomes 0, 1, 1, 2, 2. This calculates the actual number of word pairings in the ListView, minus the divider widgets.

4. If you’ve reached the end of the available word pairings, then generate 10 more and add them to the suggestions list.