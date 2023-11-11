# Freezed

```dart
import 'package:freezed_annotation/freezed_annotation.dart';
import 'package:flutter/foundation.dart';

part '$fileNameWithoutExtension$.freezed.dart';

@freezed
class $NAME$ with _$$$NAME$ {
  const factory $NAME$(int value) = Data$NAME$;
  const factory $NAME$.loading() = Loading$NAME$;
  const factory $NAME$.error([String? message]) = Error$NAME$;
}
```

## Variables

| Name                     | Expression                 | Default value                                     | Skip if Default |
|--------------------------|----------------------------|---------------------------------------------------|-----------------|
| fileNameWithoutExtension | fileNameWithoutExtension() |                                                   | true            |
| NAME                     |                            | capitalize(camelCase(fileNameWithoutExtension())) |                 |
