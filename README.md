# Build scan quickstart

<img src="http://bit.ly/28Pn68D" align="right" width="280" />

This is an example project that you can use to experience [build scans][gradle.com].

It is a small Java project that has the [build scan plugin][plugin] already applied.

## Create a build scan

Follow these simple steps to create a build scan:

1. Clone this project
2. Read the [Terms of Service][terms-of-service]
3. Uncomment the Terms of Service agreement code in the `build.gradle` file
4. Run `./gradlew build -Dscan`

The build should end with something similar to:

    Publishing build information...
    https://gradle.com/s/ria2s2x5oaazq
    
Follow the green link shown at the end of the build to view your build scan.

Note: If you run a build without the `-Dscan` flag, no build scan will be created and 
no information will be sent.

## Experiment with build scans

Create different kinds of build scans by locally modifying this quickstart project. Here are some ideas:

- Edit `src/main/java/example/Example.java` to introduce compile errors
- Edit `src/test/java/example/ExampleTest.java` to introduce test failures
- Add more dependencies, more plugins, and more projects 

Alternatively, enable one of your own builds to produce build scans by following the [step-by-step instructions][instructions].
 
## Learn more

There's more to build scans. You can create builds scans for all of your builds via an init script.
You can enable automatic publication (i.e. no need for -Dscan).
You can even extend build scans with custom data, and more.

Learn how by consulting the [build scans user manual][manual].
    
## Need help?

Talk to us on the [Gradle forum][gradle-forum].

If you are completely new to the Gradle Build Tool, start [here][gradle-download].

[gradle-download]: https://gradle.org/gradle-download
[plugin]: https://scans.gradle.com/plugin
[gradle.com]: https://www.gradle.com
[terms-of-service]: https://scans.gradle.com/terms-of-service
[instructions]: https://scans.gradle.com/get-started
[gradle-forum]: https://discuss.gradle.org/c/help-discuss/cloud-services
[manual]: https://docs.gradle.com/scans/