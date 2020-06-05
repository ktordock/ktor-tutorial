# Hello World

```kotlin
import io.ktor.routing.*
```

再來，我們撰寫第一個路由

```kotlin
fun Application.module(testing: Boolean = false) {
    routing {
        get("/") {
            call.respondText("Hello World")
        }
    }
}
```

## 運作

```
$ gradle run
```

運作後如果看到 ` Application - Responding at http://0.0.0.0:8080` 

這時候透過瀏覽器連線 http://127.0.0.1:8080/ 就可以看到 `Hello World` 囉！
