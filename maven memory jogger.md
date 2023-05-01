1. ```mvn --version```: Displays the installed version of Maven.
2. ```mvn help```: Displays the Maven help documentation.
3. ```mvn clean```: Cleans the project by deleting the target directory.
4. ```mvn package```: Packages the project and creates a .jar or .war file.
5. ```mvn install```: Installs the package in the local repository for use as a dependency in other projects.
6. ```mvn deploy```: Deploys the package to a remote repository for use as a dependency in other projects.
7. ```mvn test```: Runs the unit tests for the project.
8. ```mvn verify```: Runs the integration tests for the project.
9. ```mvn site```: Generates a website for the project, including documentation, metrics, and reports.
10. ```mvn dependency:tree```: Displays the project's dependency tree.
11. ```mvn dependency:analyze```: Analyzes the project's dependencies and reports any potential issues.
12. ```mvn dependency:purge-local-repository```: Deletes all dependencies from the local repository.
13. ```mvn clean package -DskipTests```: Builds the package without running any tests.
14. ```mvn clean install -Dmaven.test.skip=true```: Installs the package without running any tests.
