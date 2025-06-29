> [!WARNING]
> QtWebkit has been [deprecated](https://wiki.qt.io/New_Features_in_Qt_5.6) in favour of [QtWebengine](https://doc.qt.io/qt-6/qtwebengine-index.html)
> by upstream since 2016 and certain versions might be affected by a huge number of security issues.
> 
> This baseapp should not be used for new submissions at Flathub and any existing or potential
> users are advised to [port to QtWebengine](https://doc.qt.io/qt-6/qtwebenginewidgets-qtwebkitportingguide.html) and
> use the [corresponding baseapp](https://github.com/flathub/io.qt.qtwebengine.BaseApp).

### Source

This baseapp uses the [movableink/webkit](https://github.com/movableink/webkit) fork of QtWebkit.

### Usage

```yaml
app-id: com.example.foo
sdk: org.kde.Sdk
runtime: org.kde.Platform
runtime-version: 5.15-24.08
base: io.qt.qtwebkit.BaseApp
base-version: 5.15-24.08

[...]

cleanup-commands:
  - /app/cleanup-BaseApp.sh
```

### Available branches

|Baseapp branch     |Base branch   |QtWebkit version                                                          |
|-------------------|--------------|--------------------------------------------------------------------------|
|`branch/5.15-24.08`|5.15-24.08    |5.212  ([3cfcdc](https://github.com/movableink/webkit/commit/3cfcdc))     |
