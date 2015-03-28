# nebula-dependency-lock-top-level-issue
Minimal project showing an issue with nebula-dependency-lock

Run `./gradlew generateGlobalLock` to see the plugin explode:

```
:generateGlobalLock FAILED

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':generateGlobalLock'.
> Could not resolve all dependencies for configuration 'detachedConfiguration1'.
   > Module version test-gradle:inner:unspecified, configuration 'default' declares a dependency on configuration 'default' which is not declared in the module descriptor for :test-gradle:unspecified

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output.

BUILD FAILED

Total time: 0.703 secs
```
