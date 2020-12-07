# First Maven Project

Just learning a bit of Maven.

* Transitive dependencies (dependencies of dependencies)
* Transitive dependencies can be removed (beware, though)

## Commands

* `mvn clean` - deletes *target* folder.
* `mvn compile` - compile main code.
* `mvn test-compile` - compile test code.
* `mvn test` - run tests.
* `mvn install` - builds project and saves it to local Maven repository.
* `mvn package` - same as `install`, but doesn't add it to local repository.