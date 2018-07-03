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
| **1.2.0** | 25 Aug 2017 | [https://github.com/saalfeldlab/n5/tree/1.2.0] |
| **1.3.0** | 18 Dec 2017 | [https://github.com/saalfeldlab/n5/tree/1.3.0] |
| **1.4.0** | 20 Dec 2017 | [https://github.com/saalfeldlab/n5/tree/1.4.0] |
| **1.5.0** | 16 Jan 2018 | [https://github.com/saalfeldlab/n5/tree/1.5.0] |
| **2.0.0** | 17 Jan 2018 | [https://github.com/saalfeldlab/n5/tree/2.0.0] |
| **2.0.1** | 02 Feb 2018 | [https://github.com/saalfeldlab/n5/tree/2.0.1] |
| **2.0.2** | 12 Mar 2018 | [https://github.com/saalfeldlab/n5/tree/2.0.2] |

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

## N5 HDF5 Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 17 Jan 2018 | [https://github.com/saalfeldlab/n5-hdf5/tree/1.0.0] |
| **1.0.1** | 02 Feb 2018 | [https://github.com/saalfeldlab/n5-hdf5/tree/1.0.1] |
| **1.0.2** | 12 Mar 2018 | [https://github.com/saalfeldlab/n5-hdf5/tree/1.0.2] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5-hdf5</artifactId>
        <version>${n5-hdf5.version}</version>
    </dependency>
</dependencies>
```

## N5 ImgLib2 Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 21 Jun 2017 | [https://github.com/saalfeldlab/n5-imglib2/tree/1.0.0] |
| **1.1.0** | 18 Dec 2017 | [https://github.com/saalfeldlab/n5-imglib2/tree/1.1.0] |
| **2.0.0** | 17 Jan 2018 | [https://github.com/saalfeldlab/n5-imglib2/tree/2.0.0] |
| **2.1.0** | 13 Mar 2018 | [https://github.com/saalfeldlab/n5-imglib2/tree/2.1.0] |
| **2.1.1** | 14 Mar 2018 | [https://github.com/saalfeldlab/n5-imglib2/tree/2.1.1] |
| **3.0.0** | 11 May 2018 | [https://github.com/saalfeldlab/n5-imglib2/tree/3.0.0] |

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

## N5 Spark Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 17 Sep 2017 | [https://github.com/saalfeldlab/n5-spark/tree/1.0.0] |
| **1.1.0** | 19 Dec 2017 | [https://github.com/saalfeldlab/n5-spark/tree/1.1.0] |
| **2.0.0** | 17 Jan 2018 | [https://github.com/saalfeldlab/n5-spark/tree/2.0.0] |
| **2.1.0** | 13 Mar 2018 | [https://github.com/saalfeldlab/n5-spark/tree/2.1.0] |
| **3.0.0** | 22 Jun 2018 | [https://github.com/saalfeldlab/n5-spark/tree/3.0.0] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5-spark</artifactId>
        <version>${n5-spark.version}</version>
    </dependency>
</dependencies>
```

## N5 AWS S3 Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 19 Dec 2017 | [https://github.com/saalfeldlab/n5-aws-s3/tree/1.0.0] |
| **2.0.0** | 17 Jan 2018 | [https://github.com/saalfeldlab/n5-aws-s3/tree/2.0.0] |
| **2.0.1** | 02 Feb 2018 | [https://github.com/saalfeldlab/n5-aws-s3/tree/2.0.1] |
| **2.0.2** | 14 Mar 2018 | [https://github.com/saalfeldlab/n5-aws-s3/tree/2.0.2] |
| **2.1.0** | 23 Apr 2018 | [https://github.com/saalfeldlab/n5-aws-s3/tree/2.1.0] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5-aws-s3</artifactId>
        <version>${n5-aws-s3.version}</version>
    </dependency>
</dependencies>
```

## N5 Google Cloud Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 19 Dec 2017 | [https://github.com/saalfeldlab/n5-google-cloud/tree/1.0.0] |
| **2.0.0** | 17 Jan 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.0.0] |
| **2.0.1** | 02 Feb 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.0.1] |
| **2.0.2** | 14 Mar 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.0.2] |
| **2.1.0** | 19 Apr 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.1.0] |
| **2.1.1** | 20 Apr 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.1.1] |
| **2.2.0** | 20 Apr 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.2.0] |
| **2.3.0** | 23 Apr 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.3.0] |
| **2.3.1** | 23 Apr 2018 | [https://github.com/saalfeldlab/n5-google-cloud/tree/2.3.1] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5-google-cloud</artifactId>
        <version>${n5-google-cloud.version}</version>
    </dependency>
</dependencies>
```

## N5 Viewer Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **1.0.0** | 30 Jun 2017 | [https://github.com/saalfeldlab/n5-viewer/tree/1.0.0] |
| **1.2.0** | 19 Dec 2017 | [https://github.com/saalfeldlab/n5-viewer/tree/1.2.0] |
| **2.0.0** | 17 Jan 2018 | [https://github.com/saalfeldlab/n5-viewer/tree/2.0.0] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5-viewer_fiji</artifactId>
        <version>${n5-viewer_fiji.version}</version>
    </dependency>
</dependencies>
```

## N5 Label Multisets Releases
| Version | Date | Source |
| ------- | ---- | ------ |
| **0.1.0** | 19 Apr 2018 | [https://github.com/saalfeldlab/n5-label-multisets/tree/0.1.0] |
| **0.2.0** | 30 Apr 2018 | [https://github.com/saalfeldlab/n5-label-multisets/tree/0.2.0] |
| **0.3.0** | 28 Jun 2018 | [https://github.com/saalfeldlab/n5-label-multisets/tree/0.3.0] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>n5-label-multisets</artifactId>
        <version>${n5-label-multisets.version}</version>
    </dependency>
</dependencies>
```

## BigCAT Releases

| Version | Date | Source |
| ------- | ---- | ------ |
| **0.0.1-beta-1** | 1 Sep 2017 | [https://github.com/saalfeldlab/bigcat/tree/0.0.1-beta-1] |
| **0.0.3-beta-1** | 6 Feb 2018 | [https://github.com/saalfeldlab/bigcat/tree/0.0.3-beta-1] |

### Components
```
<dependencies>
    <dependency>
        <groupId>sc.fiji</groupId>
        <artifactId>bigcat</artifactId>
        <version>${bigcat.version}</version>
    </dependency>
</dependencies>
```

## Label Utilities Spark Releases
| Version | Date | Source |
| ------- | ---- | ------ |
| **0.1.0** | 29 Jun 2018 | [https://github.com/saalfeldlab/label-utilities-spark/tree/0.1.0] |
| **0.1.1** | 03 Jul 2018 | [https://github.com/saalfeldlab/label-utilities-spark/tree/0.1.1] |

### Components
```
<dependencies>
    <dependency>
        <groupId>org.janelia.saalfeldlab</groupId>
        <artifactId>label-utilities-spark</artifactId>
        <version>${n5-label-multisets.version}</version>
    </dependency>
</dependencies>
```
