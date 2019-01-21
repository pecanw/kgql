RELEASING
===

You need `secret.properties` in the project root directory:

```
BINTRAY_USER=
BINTRAY_API_KEY=
#
gradle.publish.key=
gradle.publish.secret=
```

1. Change the version in `gradle.properties` to a non-SNAPSHOT version
2. Update `CHANGELOG.md`
3. Update `README.md` with the new version
4. `git commit -am "Prepare for release vX.Y.Z."` (where X.Y.Z is the new version)
5. `sh ./release.sh`
6. Visit [bintrary.com](https://bintray.com/yshrsmz/kgql) and promote the artifact.
7. Visit [Gradle Plugin Portal](https://plugins.gradle.org/) and promote the plugin.
8. `git tag -a vX.Y.Z -m "Version vX.Y.Z"` (where X.Y.Z is the new version)

