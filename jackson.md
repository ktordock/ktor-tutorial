# 建立 json response（用 jackson 套件）

## 安裝

在 `build.gradle` 檔案的 `dependencies` 區塊內加上

`implementation "io.ktor:ktor-jackson:$ktor_version"`

## 撰寫

```kotlin
import io.ktor.features.*
import io.ktor.jackson.*
```

然後我們在 `fun Application.module(testing: Boolean = false)` 裡面加上

```kotlin
    install(ContentNegotiation) {
        jackson {
            // Configure Jackson's ObjectMapper here
        }
    }
```

最後我們撰寫一個新的路徑

```kotlin
get("/ok") {
    call.respond(mapOf("OK" to true))
}
```

然後連線 `http://127.0.0.1:8080/ok` 就可以看到一個 Json 格式的回傳，我們這個階段就完成了 
