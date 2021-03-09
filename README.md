# Example - Plugin Flutter PushLink

<p align="center">
  <img src="https://pushlink.com/javax.faces.resource/images/site/logo-verde.png.xhtml?ln=pushlink" height='130' />
  </br>
  </br>
</p>

## <a href="https://github.com/diogo-bruno/flutter-push-link">`Flutter - PushLink`</a>

---

<p align="center">
<br>
ScreenShot Example Application
<br>
<br>
<img src="https://user-images.githubusercontent.com/11491923/110528491-f8d5bf80-80f6-11eb-838d-10f5f19f5f1d.png" width="350" />
</p>

---

## `Test project`

```sh
git clone https://github.com/diogo-bruno/flutter-push-link-example.git
cd flutter-push-link-example
flutter pub get
flutter pub run flutter_push_link:prepare
flutter run -d 'DeviceName or Id' -t lib/main.dart
```

## `Usage code example`

```dart
import 'package:flutter_push_link/flutter_push_link.dart';

...

String deviceId = await FlutterPushLink.deviceId().catchError(onError);

bool started = await FlutterPushLink.startPushLink(DotEnv.env['PUSH_LINK_API_KEY'], deviceId).catchError(onError);

```

<a target="_blank" href="https://github.com/diogo-bruno/flutter-push-link-example/blob/master/lib/main.dart">Open file Application: <b>main.dart</b></a>

---
