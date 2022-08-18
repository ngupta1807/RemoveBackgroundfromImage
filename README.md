# Background Remover

This is an android library for removing background from the image.You have to give the bitmap of the image to this library and the library will return the bitmap with the removed background.

## Gradle
Add it in your root build.gradle at the end of repositories:

```groovy
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```

Add the dependency

```groovy
dependencies {
	 implementation 'com.github.GhayasAhmad:auto-background-remover:1.0.1'
}
```

## Code:
```kotlin
BackgroundRemover.bitmapForProcessing(bitmap, object: OnBackgroundChangeListener{
	override fun onSuccess(bitmap: Bitmap) {
		//do what ever you want to do with this bitmap
	}

	override fun onFailed(exception: Exception) {
		//exception
	}
})

```

# 👨 Made By

`Nisha Gupta`