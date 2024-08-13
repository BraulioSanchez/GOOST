# Grid-Ordering for Outlier Detection in Massive Data Streams

by
Braulio V. S. Vinces, Robson L. F. Cordeiro.

# To Cite
    @ARTICLE{GOOST2024,
      author={Braulio V. Sánchez Vinces, Robson L. F. Cordeiro},
      title={GOOST: Grid-Ordering for Outlier Detection in Massive Data Streams},
      booktitle={2024 Journal of Information and Data Management (JIDM)},
      year={2024}
    }

# Abstract

> Outlier detection is critical in data mining, encompassing the revelation of hidden insights or identification of potentially disruptive anomalies.
While numerous strategies have been proposed for serial-processing outlier detection, the ever-expanding realm of big data applications demands efficient distributed computing solutions.
This paper addresses the challenge of real-time outlier detection in multidimensional data streams with high-frequency arrivals, presenting GOOST.
This novel algorithm employs neighborhood analysis based on grid-based data sorting.
GOOST efficiently detects distance-based outliers, ensuring accurate detection in distributed environments within a competitive and much more stable processing time than concurrent ones.
We perform experiments on $6$ real and synthetic data sets with up to $1.2$M events, with up to $55$ dimensions.
We demonstrate that GOOST outperforms $3$ other methods in terms of quality of results ($30%$ more accurate) within competitive (and $45%$ more stable) processing times for real-time analysis of multidimensional data streams and high event frequency, offering a promising solution for various scientific and commercial domains.

# Main Sections
1. [Directory Tree]
2. [GOOST Usage]
3. [GOOST Competitors]

## Directory Tree

A summary of the file structure can be found in the following directory tree.

```bash
GOOST
├───code
│   ├───goost \\ Java implementation
├───competitors
│   ├───parallel-streaming-outlier-detection
├───datasets \\ All used datasets
├───results \\ Sheet with all the detailed results
```

## GOOST Usage

GOOST and its competitors use a number of open source tools to work properly. The following packages should be installed before starting

#### Related to Java

- jre8+ - Java Runtime Environment version 8 or more.
- maven - Software project management and comprehension tool.

#### Related to Scala

- Scala - <https://scala-lang.org/download/2.11.6.html>

#### Related to Apache Spark

- Apache Spark - <https://archive.apache.org/dist/spark/spark-2.4.5/>

#### Related to Apache Flink

- Apache Flink - <https://archive.apache.org/dist/flink/flink-1.4.0/flink-1.4.0-src.tgz>

### Building GOOST

Run with no options:

```sh
sh code/build.sh
```

## GOOST Competitors

All competitors are publicly available, below are the source code download links:

- Competitors - <https://github.com/tatoliop/parallel-streaming-outlier-detection>

_This software was designed in Unix-like systems, it is not yet fully tested in other OS._
