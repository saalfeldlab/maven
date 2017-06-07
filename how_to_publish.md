# How To Publish A New Release

## 1. Checkout Git Repo

```bash
git clone https://github.com/saalfeldlab/maven.git
```

## 2. Configure Source pom.xml

In your source root pom.xml, configure the maven distribution URL to point to the local directory where you cloned the git repo.

> NOTE: In the example below, the git repo was cloned under **/Users/trautmane/git**, 
>       so the saalfeld-maven-path property is defined as **/Users/trautmane/git/maven**

```xml
    <properties>
        <saalfeld-maven-path>/Users/trautmane/git/maven</saalfeld-maven-path>
    </properties>

    <build>
        <pluginManagement>
            <plugins>
                <plugin>
                    <artifactId>maven-deploy-plugin</artifactId>
                    <version>2.8.1</version>
                    <configuration>
                        <altDeploymentRepository>internal.repo::default::file://${saalfeld-maven-path}</altDeploymentRepository>
                    </configuration>
                </plugin>
            </plugins>
        </pluginManagement>
    </build>

    <distributionManagement>
        <repository>
            <id>local-saalfeld-maven-repo</id>
            <name>Local Saalfeld Repo</name>
            <url>file://${saalfeld-maven-path}</url>
        </repository>
    </distributionManagement>

```

## 3. Deploy Source Artifacts Locally

```bash
mvn clean deploy
```

## 4. Update README 

```bash
cd ${saalfeld-maven-path}
vi README.md

# add information about new release to README
```

## 5. Commit Changes to GitHub 

```bash
cd ${saalfeld-maven-path}
git add .
git commit -m "add release x.y.z for project foo"
git push
```
