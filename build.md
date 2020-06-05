# 建立 ktor 專案

## 安裝 ktor plugin

透過下列網址安裝 ktor 套件

https://plugins.jetbrains.com/plugin/10823-ktor

## 建立專案

安裝套件之後

使用 IntelliJ IDEA 打開 File > New > Project

在左側的選單選擇「Ktor」，之後一路「Next」

```kotlin
package com.example

import io.ktor.application.*
import io.ktor.response.*
import io.ktor.request.*

fun main(args: Array<String>): Unit = io.ktor.server.netty.EngineMain.main(args)

@Suppress("unused") // Referenced in application.conf
@kotlin.jvm.JvmOverloads
fun Application.module(testing: Boolean = false) {
}


```

看到這個程式碼的話，恭喜你，專案就建立完成了！
