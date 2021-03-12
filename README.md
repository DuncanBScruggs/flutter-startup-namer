# startup_namer

Simple app that generates proposed names for a startup company. The user can select and unselect names, saving the best ones. The code lazily generates 10 names at a time. As the user scrolls, more names are generated. There is no limit to how far a user can scroll.

## Accomplished in [Part 1](https://flutter.dev/docs/get-started/codelab)

- Created a Flutter app from the ground up.
- Written Dart code.
- Leveraged an external, third-party library.
- Used hot reload for a faster development cycle.
- Implemented a stateful widget.
- Created a lazily loaded, infinite scrolling list.

## Accomplished in [part 2](https://codelabs.developers.google.com/codelabs/first-flutter-app-pt2#0)

- Writing Dart code
- Using hot reload for a faster development cycle
- Implementing a stateful widget, adding interactivity to your app
- Creating a route and adding logic for moving between the home route and the new route
- Learning about changing the look of your app's UI using themes

## Notes

1. The itemBuilder callback is called once per suggested word pairing, and places each suggestion into a ListTile row. For even rows, the function adds a ListTile row for the word pairing. For odd rows, the function adds a Divider widget to visually separate the entries. Note that the divider might be difficult to see on smaller devices.

2. Add a one-pixel-high divider widget before each row in the ListView.

3. The expression i ~/ 2 divides i by 2 and returns an integer result. For example: 1, 2, 3, 4, 5 becomes 0, 1, 1, 2, 2. This calculates the actual number of word pairings in the ListView, minus the divider widgets.

4. If you’ve reached the end of the available word pairings, then generate 10 more and add them to the suggestions list.