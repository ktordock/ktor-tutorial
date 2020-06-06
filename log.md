# log

Ktor 使用 SLF4J 這個套件處理 log

## 建置

在 `build.gradle` 裡面加上

```
compile("ch.qos.logback:logback-classic:1.2.3")
```

程式上面加上

```kotlin
import java.util.logging.*
```

## 參考資料
https://ktor.io/servers/logging.html
