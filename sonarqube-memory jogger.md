1. ```/opt/sonarqube/bin/sonar.sh -v```: Check the version of SonarQube installed on your system
2. ```systemctl start sonarqube```: Start the SonarQube server
3. ```systemctl stop sonarqube```: Stop the SonarQube server:
4. ```systemctl restart sonarqube```: Restart the SonarQube server
5. ```systemctl status sonarqube```: Check the status of the SonarQube server
6. ```sonar-scanner -Dsonar.projectKey=project_key -Dsonar.sources=. -Dsonar.host.url=http://localhost:9000```: Analyze code with SonarScanner
##### By default SonarQube uses port 9000.
6. ```mvn sonar:sonar```: Maven command used to analyze a project with SonarQube. 


## References

#### SonarQube Documentation - https://docs.sonarqube.org/latest/
#### Sonar As a Service (sonarcloud)  - https://www.sonarsource.com/products/sonarcloud/
