angular_oauthio_wrapper.dart
============================

An AngularDart wrapper around OAuth.io's oauth.js library


Bind your config in your module:

```dart
class YourModule extends Module {
  YourModule() {
    String publicKey = 'YOUR_PUBLIC_KEY';
    bind(OauthioConfig, toValue: new OmniauthOauthioConfig(publicKey, 'localhost', 3000, 'users/auth')..secure=false);
  }
}
```
