---
title: "Kotlin"
description: "Learn Kotlin. An exciting modern language for everything"
coverImage: "/kotlin.svg"
category: "Multiplatform"
inDev: False
pubDate: "2025-10-20"
updatedDate: ""
publishDate: "Monday 20th"
---

# Kotlin: Concise. Multiplatform. Fun.

Kotlin is a powerful language that can be used for Android development, backend services, and even scripting.
This week's challenges will help you build core Kotlin skills while having fun!

Before we dive into the challenges, here are some resources to help you get started with Kotlin:
 - [Kotlin Tour](https://kotlinlang.org/docs/kotlin-tour-welcome.html)
 - [Kotlin in 100 Seconds](https://www.youtube.com/watch?v=xT8oP0wy-A0)
 - [Kotlin Docs](https://kotlinlang.org/docs/home.html)

It is highly recommend to be familiar with the basics of Kotlin syntax before attempting the challenges.

There are two categories of challenges:
 - Kotlin Playground Challenges (for those who want to practice in a browser)
 - Kotlin Multiplatform Project Challenge (for those who want to dive into multiplatform development)

## **Kotlin Playground Challenges (No Installation Needed!)**
For those who don’t want to set up IntelliJ, you can solve these challenges in the **Kotlin Playground**: [https://play.kotlinlang.org](https://play.kotlinlang.org)

### Challenge 1: Hello World (50 Points)
Create a function that takes a name as a parameter and returns a greeting. I highly recommend using [string templates](https://kotlinlang.org/docs/strings.html#string-templates).

```kotlin
fun greetUser(name: String) {
    // Your code
}
```

Example:
```kotlin
fun main() {
   greetUser("Will") // Output: Hello, Will! Welcome to Kotlin!
}
```

---

### Challenge 2: When Expression (50 Points)
Write a function to assign a letter grade, given an integer score (out of 100). Try not to write an if-else chain, use Kotlin’s [when expression](https://kotlinlang.org/docs/control-flow.html#when-expressions-and-statements) and [ranges](https://kotlinlang.org/docs/ranges.html#range).

```kotlin
fun assignGrade(score: Int): String {
    return when (score) {
        // Your code here using ranges like `in 90..100`
    }
}

fun main() {
    println("95: ${assignGrade(95)}") // Expected: A
    println("82: ${assignGrade(82)}") // Expected: B
    println("55: ${assignGrade(55)}") // Expected: F
}
```

### Challenge 3: Null Safety (20 Points)
Update your hello world greeting function to take a [nullable](https://kotlinlang.org/docs/null-safety.html#nullable-types-and-non-nullable-types) string instead. If the name is null, use guest. Try not to use an if statement!

```kotlin
fun greetUser(name: String?) {
    // Your code
}
```

Example:
```kotlin
fun main() {
    greetUser("Will") // Output: Hello, Will! Welcome to Kotlin!
    greetUser(null) // Output: Hello, Guest! Welcome to Kotlin!
}
```

---

### 🏃‍♂️ Challenge 4: Extension Function (20 Points)
Add an [extension function](https://kotlinlang.org/docs/extensions.html) to the `String` class that makes the string all uppercase and adds exclamation points.

```kotlin
// Your extension function here. It should start with `fun String.shout(): String`

fun main() {
    val message = "hello kotlin"
    println(message.shout()) // Expected: HELLO KOTLIN!!!
}
```

---

## Challenge: Create a Kotlin Multiplatform Project (100 Points)
### What is Kotlin Multiplatform (KMP)?
Kotlin Multiplatform (KMP) is a powerful feature of Kotlin that allows developers to write shared code once and run it on multiple platforms, such as:

- Android (using Kotlin/JVM)
- iOS (using Swift/Objective-C interop)
- Web (via Kotlin/JS or Kotlin/WASM)
- Desktop (using Kotlin/JVM or Kotlin/Native)

Unlike traditional cross-platform frameworks, KMP does not enforce a single UI toolkit—you can share business logic, networking, and data processing while keeping native UI experiences for each platform.
#### Why is KMP Exciting?

- Single Codebase for Business Logic – Reduce duplication by sharing data models, networking, and logic across platforms.
- Platform-Specific Flexibility – Use expect/actual to implement native features where needed.
- Interoperability – Easily integrate with existing Android, iOS, and web projects.
- Less Boilerplate, More Productivity – Write less redundant code while keeping full platform-native power!

### Your goal is to create a Kotlin Multiplatform (KMP) project that:
- Shares business logic across different platforms.
- Runs on **at least two targets** (e.g., Android & JVM, iOS & Web, etc.).
- Uses Kotlin’s **expect/actual mechanism** for platform-specific implementations.

Have a good idea and want to keep developing? You can submit your project to the official [Kotlin Multiplatform Contest](https://kotlinconf.com/contest/) and win a free trip of KotlinConf!

---

### Steps to Complete the Challenge
1. **Set up a new KMP project**
   - Use [IntelliJ IDEA](https://www.jetbrains.com/idea/download/), [Android Studio](https://developer.android.com/studio), or [Fleet](https://www.jetbrains.com/fleet/).
   - Follow along with the [Kotlin Multiplatform Setup Guide](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html).
   - Create a project with the [Kotlin Multiplatform Wizard](https://kmp.jetbrains.com/).
   - Choose at least **two targets** (e.g., Android + iOS, JVM + Web, etc.).

2. **Implement shared logic**
   - Create a shared module (e.g., `:shared`) with a simple function, such as `fun getPlatformName(): String`.
   - Use `expect` in the shared module and `actual` implementations in platform-specific code.

3. **Run on multiple platforms**
   - Run the project and ensure the shared code executes on **all configured platforms**.

---

---

### **💡 Example: Shared `expect/actual` Code**
#### **Shared Code (commonMain)**
```kotlin
expect fun getPlatformName(): String

fun greet(): String = "Hello from ${getPlatformName()}!"
```

#### **Android Implementation (androidMain)**
```kotlin
actual fun getPlatformName(): String = "Android"
```

#### **iOS Implementation (iosMain)**
```kotlin
actual fun getPlatformName(): String = "iOS"
```

---

### **🔗 Resources to Get Started**
- [Kotlin Multiplatform Setup Guide](https://kotlinlang.org/docs/multiplatform.html)
- [Kotlin Multiplatform Wizard](https://kmp.jetbrains.com/)
- [Compose Multiplatform (Jetpack Compose UI)](https://www.jetbrains.com/lp/compose-multiplatform/)

---

This challenge is **open-ended**, so feel free to explore different platforms and experiment! Let me know if you want specific tweaks or more advanced goals.

### **🔗 How to Submit**
1. For Kotlin Playground challenges, submit a link to your solution.
2. For the multiplatform project, share your project repository or a screenshot/video.

Submission Form: [Submit Here](https://forms.gle/g3TbxaU2r4sCy84XA)
