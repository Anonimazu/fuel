# fuel-livedata
[![Kotlin](https://img.shields.io/badge/Kotlin-1.3.20-blue.svg)](https://kotlinlang.org)

The `LiveData` extension package for [`Fuel`](../README.md).

## Installation

You can [download](https://bintray.com/kittinunf/maven/Fuel-Android/_latestVersion) and install `fuel-livedata` with `Maven` and `Gradle`. The livedata package has the following dependencies:
* `fuel:fuel:<same-version>`
* Kotlin: 1.3.20
* [AndroidX Livedata](https://developer.android.com/topic/libraries/architecture/livedata.html)

```groovy
compile 'com.github.kittinunf.fuel:fuel:<latest-version>'
compile 'com.github.kittinunf.fuel:fuel-livedata:<latest-version>'
```

## Usage

See `FuelLiveData.kt`

### LiveData Response

* Fuel supports [LiveData](https://developer.android.com/topic/libraries/architecture/livedata.html)
```kotlin
Fuel.get("www.example.com/get")
    .liveDataResponse()
    .observe(this) { /* do something */ }
```
