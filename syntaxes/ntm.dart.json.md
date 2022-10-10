

ntm comment (doesn't work)

```
      "begin": "('|\"|'''|\"\"\")\\s?\\/\\/\\s?ntm",
```

Work for some time:

 "begin": "('|\"|'''|\"\"\")",


Dart comment (doesn't work)

```
    {
      "begin": "\\/\\*ntm\\*\\/\\s?('|\"|'''|\"\"\")",
      "contentName": "meta.embedded.block.ntm",
      "end": "('''|\"\"\"|'[^']|\"[^\"])",
      "patterns": [
        {
          "include": "source.ntm"
        }
      ]
    }
```


All comments (works for few seconds)
```
    {
      "begin": "('''|\"\"\"|'|\")",
      "contentName": "meta.embedded.block.ntm",
      "end": "('''|\"\"\"|'|\")",
      "patterns": [
        {
          "include": "source.ntm"
        }
      ]
    }
```
