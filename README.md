i18n
====

Translate messages emited by the other modules.

## How to Use?

### Configuration

#### v0.2.x

`config.translations` is an object in the following format:

Example:

```JSON
{
  "I am.": "Je suis.",
  "You are.": {
      "fr": "Tu es.",
      "ro": "Tu ești."
  },
  ...
}
```

`config.translates` is an array of miids that emit the `message` event.

#### v0.1.x

##### DEPRECATED IN v0.2.x

`config.translations` is an array of objects in the following format:

Example:

```JSON
  [
      {
          "old": "I am.",
          "new": "Je suis."
      },
      {
          "old": "You are.",
          "new": {
              "fr": "Tu es.",
              "ro": "Tu ești."
          }
      },
      ...
  ]
```

`config.listen` is an array of miids that emit the `message` event.
## Changelog

### dev
 - Update to Events v0.1.3 and Bind v0.1.3
 - Renamed `main.js` into `i18n.js`
 - New format of `config.translations`: object instead of array
 - Renamed `config.listen` into `config.translates` to prevent overwriting of Events configuration (that uses `config.listen`)

### v0.1.1
 - Fixed translating strings.

### v0.1.0
 - Initial release
