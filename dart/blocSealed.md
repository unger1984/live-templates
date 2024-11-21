# BloC with Freezed

```dart
import 'package:flutter_bloc/flutter_bloc.dart';

sealed class $NAME$Event {
  const $NAME$Event();
  const factory $NAME$Event.init() = _Init$NAME$Event;
}
final class _Init$NAME$Event extends $NAME$Event{
  const _Init$NAME$Event();
}

sealed class $NAME$State {
  const $NAME$State();
  const factory $NAME$State.loading() = Loading$NAME$State;
}
final class Loading$NAME$State extends $NAME$State{
  const Loading$NAME$State();
}

class $NAME$BLoC extends Bloc<$NAME$Event, $NAME$State> {
  $NAME$BLoC() : super(const $NAME$State.loading()){
    on<$NAME$Event>(
          (event, emitter) => switch(event){
          _Init$NAME$Event() => _init(event, emitter),
          },
    );
  }

  Future<void> _init(_Init$NAME$Event event, Emitter<$NAME$State> emitter) async {
    // ...
  }
}

```

## Variables

| Name                     | Expression                 | Default value                                     | Skip if Default |
|--------------------------|----------------------------|---------------------------------------------------|-----------------|
| NAME                     |                            | capitalize(camelCase(fileNameWithoutExtension())) |                 |
