# django-test-runner

Adds support for running Django tests in [Visual Studio Code](https://github.com/microsoft/vscode). Provides shortcuts to run closest method, class, file, app and previous tests. Provides support for Django-Nose in settings.
Draws inspiration from [vscode-django-tests](https://github.com/remik/vscode-django-tests) and [vim-python-test-runner](https://github.com/JarrodCTaylor/vim-python-test-runner).

Default shortcuts:
```
Run Closest Test Method: cmd+d+m        extension.djangoTestRunner.runMethodTests
Run Closest Test Class:  cmd+d+c        extension.djangoTestRunner.runClassTests
Run Current Test File:   cmd+d+f        extension.djangoTestRunner.runFileTests
Run Current App Tests:   cmd+d+a        extension.djangoTestRunner.runAppTests
Run Previous Tests:      cmd+d+p        extension.djangoTestRunner.runPreviousTests
```

## Features

\!\[feature X\]\(images/feature-x.png\)

> Tip: Many popular extensions utilize animations. This is an excellent way to show off your extension! We recommend short, focused animations that are easy to follow.

## Requirements

Requires manage&#46;py to be in the root workspace directory, otherwise add a cd command to the `python.djangoTestRunner.prefixCommand` settings such as "cd ~/Projects/hello-world/src &&"

## Extension Settings

This extension contributes the following settings:

* `python.djangoTestRunner.djangoNose`: if checked will use django-nose syntax for running class/method tests inside a file, defaults to non-nose testing syntax
* `python.djangoTestRunner.flags`: any flags you wish to run such as --nocapture, also useful for specifying different settings if you use a modified manage&#46;py
* `python.djangoTestRunner.prefixCommand`: any command(s) to be directly before the main test command e.g. "cd ~/Projects/hello-world/src &&" to cd into the directory containing your manage&#46;py

## Known Issues

Open a issue/feature request and more at [the github repository](https://github.com/Pachwenko/VSCode-Django-Test-Runner/issues)

## Release Notes

Adds support for running Django Tests a multitude of ways such as by method or class. Supports Django-Nose syntax, test flags, and prefix commands.

### 1.0.0

Initial release of Django Test Runner