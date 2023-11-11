# Freezed with JsonSerializable

```dart
import 'package:freezed_annotation/freezed_annotation.dart';

part '$fileNameWithoutExtension$.freezed.dart';
part '$fileNameWithoutExtension$.g.dart';

@freezed
class $NAME$ with _$$$NAME$ {
  const $NAME$._();

  const factory $NAME$({
    @JsonKey(name: 'id', required: true, disallowNullValue: true)
    required int id,
    $END$
  }) = _$NAME$;

  factory $NAME$.fromJson(Map<String, dynamic> json) => _$$$NAME$FromJson(json);
}
```

## Variables

| Name                     | Expression                 | Default value                                     | Skip if Default |
|--------------------------|----------------------------|---------------------------------------------------|-----------------|
| fileNameWithoutExtension | fileNameWithoutExtension() |                                                   | true            |
| NAME                     |                            | capitalize(camelCase(fileNameWithoutExtension())) |                 |
