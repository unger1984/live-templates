# StatefulWidget

```dart
import 'package:flutter/material.dart';

@immutable
class $NAME$ extends StatefulWidget {
  const $NAME$({super.key});

  @override
  State<$NAME$> createState() => _$NAME$State();
}

class _$NAME$State extends State<$NAME$> {
  @override
  Widget build(BuildContext context) {
    return Container();$END$
  }
}
```

## Variables

| Name   | Expression | Default value |
|--------|------------|---------------|
| NAME   |            |capitalize(camelCase(fileNameWithoutExtension()))|
