# JsonSerializable

```dart
import 'package:json_annotation/json_annotation.dart';

part '$fileNameWithoutExtension$.g.dart';

@JsonSerializable()
class $NAME$ {
  $NAME$();
  factory $NAME$.fromJson(Map<String, dynamic> json) => _$$$NAME$FromJson(json);
  Map<String, dynamic> toJson() => _$$$NAME$ToJson(this);
}
```

## Variables

| Name                     | Expression                 | Default value                                     | Skip if Default |
|--------------------------|----------------------------|---------------------------------------------------|-----------------|
| fileNameWithoutExtension | fileNameWithoutExtension() |                                                   | true            |
| NAME                     |                            | capitalize(camelCase(fileNameWithoutExtension())) |                 |
