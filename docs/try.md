## Try Impeller in Flutter

Impeller is available under the `--enable-impeller` flag on iOS, Android, and
macOS Desktop. This flag can be specified to `flutter run`.

If the application needs to be launched with Impeller enabled without using the
Flutter tool, follow the platform specific steps below.

### iOS and macOS Desktop

To your `Info.plist` file, add under the top-level `<dict>` tag:
```xml
  <key>FLTEnableImpeller</key>
  <true/>
```

### Android

To your `AndroidManifest.xml` file, add under the `<application>` tag:
```xml
  <meta-data
    android:name="io.flutter.embedding.android.EnableImpeller"
    android:value="true" />
```
