![plon](https://raw.githubusercontent.com/jsumnersmith/poetic-line-object-notation/master/plon.png 'plon Logo')
#### A protocol for annotating poetic lines as JSON-like data.

## Precis
The goal of this protocol is to define how poetic lines might be represented as JSON-like data structures. This protocol is speculative and therefore will attempt to use examples as much as possible.

## Simple Example
Take a short example such as Ezra Pound's "In a Station of the Metro." As simple text, it reads as follows:
```text
The apparition of these faces in the crowd;
Petals on a wet, black bough.
```
In `plon`, the previous poem would be represented by the following data structure:
```json
[
  {
    "text": "The apparition of these faces in the crowd;",
    "lineNumber": 1,
    "meta": {
      "author": "Ezra Pound",
      "title": "In a Station of the Metro",
      "language": "English"
    },
    "layout": {
      "indentation": 0,
      "alignment": "left",
    },
  },
  {
    "text": "Petals on a wet, black bough.",
    "lineNumber": 2,
    "meta": {
      "author": "Ezra Pound",
      "title": "In a Station of the Metro",
      "language" "English"
    },
    "layout": {
      "indentation": 0,
      "alignment": "left",
    }
  }
]
```
