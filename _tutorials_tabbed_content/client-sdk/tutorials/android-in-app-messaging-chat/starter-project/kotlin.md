---
title: Kotlin
language: android
menu_weight: 1
---


Clone this [Github project](https://github.com/nexmo-community/client-sdk-android-tutorial-messaging).

In Android Studio go to menu `File -> Open` and select the `kotlin-start` folder from cloned repository (this not a top-level folder).

Open `app/src/main/java/com/vonage/tutorial/messaging/Consts.swift` file and add fill:
 -  `Joe`'s user IDs and JWTs, and conversation ID you've created on the previous steps:

```kotlin
package com.vonage.tutorial.messaging

data class User(
    val name: String,
    val jwt: String
)

object Config {

    const val CONVERSATION_ID: String = "" // TODO: set conversation Id

    val jane = User(
        "Jane",
        "" // TODO: "set Jane's JWT token"
    )
    val joe = User(
        "Joe",
        "" // TODO: set Joe's JWT token"
    )
}

```

Notice that we defined these cons and values to store properties of users. This might feel a bit out of place but makes it easier to use later on.