# How To Publish A New Release

## 1. Checkout Git Repo

```bash
git clone https://github.com/saalfeldlab/maven.git
```

## 2. Configure Source pom.xml

In your source root pom.xml, configure the maven distribution URL to point to the local directory where you cloned the git repo.

```xml
    <deploy.path>/Users/trautmane/projects/git/maven</deploy.path>

    <build>
        <pluginManagement>
            <plugins>
                <plugin>
                    <artifactId>maven-deploy-plugin</artifactId>
                    <version>2.8.2</version>
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

Run in the directory with the artifact you want to publish:
```bash
cd <path to cloned maven repo>/deploy
```

## 4. Update README 

```bash
cd <path to cloned maven repo>
vim README.md

# add information about new release to README
```

## 5. Commit Changes to GitHub 

```bash
cd <path to cloned maven repo>
git add .
git commit -m "add release x.y.z for project foo"
git push
```
