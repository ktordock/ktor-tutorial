# 建立新 route

建立新 route 的方法很簡單，跟前面建立 Hello world 的方式一樣

我們嘗試看看多加一個 `/test` 的 

```kotlin
get("/test") {
    call.respondText("Hello Test")
}
```
