# Cubit with Freezed

```dart
import 'package:flutter_bloc/flutter_bloc.dart';
import 'package:freezed_annotation/freezed_annotation.dart';

part '$fileNameWithoutExtension$.freezed.dart';

@freezed
class $NAME$State with _$$$NAME$State {
  const $NAME$State._();
  const factory $NAME$State.loading() = Loading$NAME$State;
}

class $NAME$ extends Cubit<$NAME$State> {
  $NAME$() : super(const Loading$NAME$State());
}
```

## Variables

| Name                     | Expression                 | Default value                                     | Skip if Default |
|--------------------------|----------------------------|---------------------------------------------------|-----------------|
| fileNameWithoutExtension | fileNameWithoutExtension() |                                                   | true            |
| NAME                     |                            | capitalize(camelCase(fileNameWithoutExtension())) |                 |
