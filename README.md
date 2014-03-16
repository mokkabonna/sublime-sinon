# Snippets for Sinon asserts

Includes it's own language config so that the comopletions triggers in files for tests. This syntax is called JavaScript (BDD test) and inherits from the standard JavaScript syntax.

Either you can manually change the syntax for the file to this syntax to enable the completions, or even better use the sublime package [ApplySyntax](https://sublime.wbond.net/packages/ApplySyntax)

Then in your user setting configure it like this (depending on the filename pattern for your tests, in this example all files end with `Spec.js`)

```json
{
    // If you want exceptions reraised so you can see them in the console, change this to true.
    "reraise_exceptions": false,

    // If you want to have a syntax applied when new files are created, set new_file_syntax to the name of the syntax to use.
    // The format is exactly the same as "name" in the rules below. For example, if you want to have a new file use
    // JavaScript syntax, set new_file_syntax to 'JavaScript'.
    "new_file_syntax": false,

    // Put your custom syntax rules here:
    "syntaxes": [
        {
            "name": "Sinon/JavaScript (Test)",
            "rules": [
                {"file_name": ".+Spec.js$"}
            ]
        }
    ]
}
```
