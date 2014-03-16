# Snippets for Sinon asserts

Includes it's own language config so that the comopletions triggers in files for tests. This syntax is called JavaScript (Test) and inherits from the standard JavaScript syntax.

Either you can manually change the syntax for the file to this syntax to enable the completions, or even better use the sublime package [ApplySyntax](https://sublime.wbond.net/packages/ApplySyntax)

Then in your user setting configure it like this (depending on the filename pattern for your tests, in this example all files end with `Spec.js`)

```json
{
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
