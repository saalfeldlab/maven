# How To Publish A New Release

## 1. Checkout Git Repo

```bash
git clone https://github.com/saalfeldlab/maven.git
```

## 2. Configure Source pom.xml

In your source root pom.xml, configure the maven distribution URL to point to the local directory where you cloned the git repo.

> NOTE: In the example below, the git repo was cloned under **/Users/trautmane/git**, 
>       so the `deploy.path` property is passed as **/Users/trautmane/git/maven**

```xml
    <build>
        <pluginManagement>
            <plugins>
                <plugin>
                    <artifactId>maven-deploy-plugin</artifactId>
                    <version>2.8.1</version>
                    <configuration>
                        <altDeploymentRepository>internal.repo::default::file://${deploy.path}</altDeploymentRepository>
                    </configuration>
                </plugin>
            </plugins>
        </pluginManagement>
    </build>

    <distributionManagement>
        <repository>
            <id>local-maven-repo</id>
            <name>Local Maven Repository</name>
            <url>file://${deploy.path}</url>
        </repository>
    </distributionManagement>

```

## 3. Deploy Source Artifacts Locally

```bash
mvn -Ddeploy.path=/Users/trautmane/git/maven clean deploy
```

## 4. Update README 

```bash
cd /Users/trautmane/git/maven
vim README.md

# add information about new release to README
```

## 5. Commit Changes to GitHub 

```bash
cd /Users/trautmane/git/maven
git add .
git commit -m "add release x.y.z for project foo"
git push
```
