This is a pure Dart HTML5 parser.
It's a port of [html5lib](https://github.com/html5lib/html5lib-python) from 
Python. 

# Notice
**This is a fork of `html` that supports more selectors and fixes some bugs.**

**This module was created because the `html` project handles the pull request very slowly.**

# Usage

Parsing HTML is easy!

```dart
import 'package:html_plus/parser.dart' show parse;
import 'package:html_plus/dom.dart';

main() {
  var document = parse(
      '<body>Hello world! <a href="www.html5rocks.com">HTML5 rocks!');
  print(document.outerHtml);
}
```

You can pass a String or list of bytes to `parse`.
There's also `parseFragment` for parsing a document fragment, and `HtmlParser`
if you want more low level control.

[html5parse]: http://dev.w3.org/html5/spec/parsing.html
