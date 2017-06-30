# Saalfeld Lab Releases for Maven Users

This maven repository contains stable releases of Saalfeld Lab software not available in Maven Central.  
Lab members can find information on how to package and publish releases [here](how_to_publish.md).

## How to use
Add this to your pom.xml:

```
<repositories>
    <repository>
        <id>saalfeld-lab-maven-repo</id>
        <url>https://saalfeldlab.github.io/maven</url>
    </repository>
</repositories>
```
Then add dependencies for the specific components you wish to use.

## Renderer Toolkit Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **0.3.0** | 5 Jan 2017 | [https://github.com/saalfeldlab/render/releases/tag/v0.3.0] |
| **1.0.0** | 5 Jun 2017 | [https://github.com/saalfeldlab/render/releases/tag/v1.0.0] |

### Components
```
<dependencies>
    <dependency>
        <!-- Core render models and processing components -->
        <groupId>org.janelia.render</groupId>
        <artifactId>render-app</artifactId>
        <version>${render.version}</version>
    </dependency>
    <dependency>
        <!-- Render web service components -->
        <groupId>org.janelia.render</groupId>
        <artifactId>render-ws</artifactId>
        <version>${render.version}</version>
        <classifier>classes</classifier>
    </dependency>
    <dependency>
        <!-- Java client components that utilize render web services -->
        <groupId>org.janelia.render</groupId>
        <artifactId>render-ws-java-client</artifactId>
        <version>${render.version}</version>
    </dependency>
    <dependency>
        <!-- Spark client components that utilize render web services -->
        <groupId>org.janelia.render</groupId>
        <artifactId>render-ws-spark-client</artifactId>
        <version>${render.version}</version>
    </dependency>
    <dependency>
        <!-- Tools and scripts for translating data between the TrakEM2 and Render models -->
        <groupId>org.janelia.render</groupId>
        <artifactId>trakem2-scripts</artifactId>
        <version>${render.version}</version>
    </dependency>
</dependencies>
```

## N5 Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 21 Jun 2017 | [https://github.com/saalfeldlab/n5/tree/1.0.0] |
| **1.1.0** | 23 Jun 2017 | [https://github.com/saalfeldlab/n5/tree/1.1.0] |
| **1.1.1** | 28 Jun 2017 | [https://github.com/saalfeldlab/n5/tree/1.1.1] |
| **1.1.3** | 28 Jun 2017 | [https://github.com/saalfeldlab/n5/tree/1.1.3] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5</artifactId>
        <version>${n5.version}</version>
    </dependency>
</dependencies>
```

## N5 ImgLib2 Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 21 Jun 2017 | [https://github.com/saalfeldlab/n5-imglib2/tree/1.0.0] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5-imglib2</artifactId>
        <version>${n5-imglib2.version}</version>
    </dependency>
</dependencies>
```
