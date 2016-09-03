Gradle Wrapper Demo
===================

How to generate a `gradlew` file under the project root.

Install `gradle` first:

```
brew install gradle
gradle -v
```

Generate `gradlew` by command:

```
gradle wrapper --gradle-version 2.4
```

Or define a task in `build.gradle`:

```
task wrapper(type: Wrapper) {
   gradleVersion = '2.4' //version required
}
```

Then run:

```
gradle wrapper
```
