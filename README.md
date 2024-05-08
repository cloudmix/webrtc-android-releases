# webrtc-android-releases

Android WebRTC library releases

### Usage

Add the `webrtc-android-releases` maven repository to the `settings.gradle.kts` file:

```kotlin
dependencyResolutionManagement {
	repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
		repositories {
		google()
		mavenCentral()
		maven {
			name = "webrtc"
			url = uri("https://maven.pkg.github.com/cloudmix/webrtc-android-releases")
			credentials {
				username = "my_github_username"
				password = "ghp_xxxxxxxxxxxxxxxxxxxxxxx"
			}
		}
	}
}
```

Add the package to dependencies in `/app/build.gradle.kts`

```kotlin
dependencies {
    ...
    implementation("io.cmix:webrtc:124.0.0")
}
```
