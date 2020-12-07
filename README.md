# First Maven Project

Just learning a bit of Maven.

* Transitive dependencies (dependencies of dependencies)
* Transitive dependencies can be removed (beware, though)
* Scopes
    * compile - available for everything.
    * test - compiles only for testing.
    * runtime - only available during runtime. Useful for decoupling implementations (by tagging them with runtime scope) from interfaces.
    * provided - assumes dependency will be provided by the application server.
* Dependency versions can be specified in invertals:
    * <version>[4.1,]</version> - accepts any version from 4.1 and above.
    * <version>[,4.5]</version> - accepts any version from 4.5 and below.
    * <version>[4.1,4.5]</version> - accepts any version between 4.1 and 4.5 (inclusive)
    * <version>[4.1,4.5)</version> - accepts any version between 4.1 (inclusive) and 4.5 (exclusive)

## Commands

* `mvn clean` - deletes *target* folder.
* `mvn compile` - compile main code.
* `mvn test-compile` - compile test code.
* `mvn test` - run tests.
* `mvn install` - builds project and saves it to local Maven repository.
* `mvn package` - same as `install`, but doesn't add it to local repository.