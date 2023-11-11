# BloC with Freezed

```dart
import 'package:flutter_bloc/flutter_bloc.dart';
import 'package:freezed_annotation/freezed_annotation.dart';

part '$fileNameWithoutExtension$.freezed.dart';

@freezed
class $NAME$Event with _$$$NAME$Event {
  const $NAME$Event._();
  const factory $NAME$Event.init() = Init$NAME$Event;
}

@freezed
class $NAME$State with _$$$NAME$State {
  const $NAME$State._();
  const factory $NAME$State.loading() = Loading$NAME$State;
}

class $NAME$BLoC extends Bloc<$NAME$Event, $NAME$State> {
  $NAME$BLoC() : super(const $NAME$State.loading()){
    on<$NAME$Event>(
          (event, emitter) => event.map(
        init: (event) => _init(event, emitter),
      ),
    );
  }

  Future<void> _init(Init$NAME$Event event, Emitter<$NAME$State> emitter) async {
    // ...
  }
}

```

## Variables

| Name                     | Expression                 | Default value                                     | Skip if Default |
|--------------------------|----------------------------|---------------------------------------------------|-----------------|
| fileNameWithoutExtension | fileNameWithoutExtension() |                                                   | true            |
| NAME                     |                            | capitalize(camelCase(fileNameWithoutExtension())) |                 |
