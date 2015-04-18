# Dialog.dart

Modern alert, confirm and prompt dialog implementation

## Description

This package replaces default alert and confirm dialogs from Dart's Window class and adds missing prompt dialog. Default system dialogs called by that prompts are superseded by modern modal design.

## Usage

Usage is almost the same as set in the Dart's Window class and completely the same as described in the WHATWG HTML Standard. For each dialog there is just one file to import only the dialog you really need. There is also one file to import all three dialogs at once if you want to use them all.

```Dart
import "package:dialog/<file>";
```

### dialogs/alert.dart

Replaces default alert dialog.

```Dart
querySelector("#alertButton").onClick.listen((_) {
  alert("Alerted?!");
});
```

![Image of alert](https://raw.githubusercontent.com/dvorapa/dialog-dart/master/alert.png)

### dialogs/confirm.dart

Replaces default confirm dialog.

```Dart
querySelector("#confirmButton").onClick.listen((_) {
  var myConfirm = confirm("Confirmed?!");
  alert(myConfirm.toString());
});
```

![Image of confirm](https://raw.githubusercontent.com/dvorapa/dialog-dart/master/confirm.png)

### dialogs/prompt.dart

Adds missing prompt dialog.

```Dart
querySelector("#promptButton").onClick.listen((_) {
  var myPrompt = prompt("Prompted?!", "Yes!");
  alert(myPrompt.toString());
});
```

![Image of prompt](https://raw.githubusercontent.com/dvorapa/dialog-dart/master/prompt.png)

### dialog.dart

Do you need to use them all at once? Try it by importing dialog.dart file.