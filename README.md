# fuzzy_matchoop

(Unfinished)

Built for the purpose of matching live item listings on e-commerce platforms with the appropriate product identification code.

Matches similar strings together using a similarity score based off the Jaccard Index.

Highly scalable for big data.

The project is written in Java and runs on Apache Hadoop.

Note: Use non-distributed methods if data is small (i.e under 5GB)

## Getting Started

### Prerequisites

- Apache Hadoop

- Java

- Python

- Linux

- EBay developer key/token

- Semantics3 developer key/token

### Installing

Apache Hadoop download link:
```
http://hadoop.apache.org/releases.html
```
Eclipse IDE download link:
```
https://www.eclipse.org/downloads/packages/eclipse-ide-java-developers/keplersr1
```
EBay developer sign up:
```
https://developer.ebay.com/signin?return_to=%2Fmy%2Fauth%2F%3Fenv%3Dsandbox%26index%3D0
```
Semantics3 sign up:
```
https://www.semantics3.com/
```

## Map Reduce Phases

### Phases 1 & 2: Word Count and Sort

![bto](https://user-images.githubusercontent.com/35964377/36488749-29ae114a-171c-11e8-8910-ba4080c2e8b2.png)

### Phase 3: PPjoin + Kernel

![oprj](https://user-images.githubusercontent.com/35964377/36488918-8df9a628-171c-11e8-8b06-3b8d92d25bd9.png)

### Phase 4: One Phase Record Join

![pp k](https://user-images.githubusercontent.com/35964377/36488924-93e6af4a-171c-11e8-8266-10fdebe6f9b6.png)

## Results

### Sample Word Count and Sort

![sample_results](https://user-images.githubusercontent.com/35964377/36489192-48b146d8-171d-11e8-9873-1372da5590e1.PNG)

### Scalability Testing vs Python

![graph](https://user-images.githubusercontent.com/35964377/36489196-4a29e34e-171d-11e8-8932-f30317c9b68d.PNG)
- Evidence of greater scalability, however needs testing with larger data

## Authors

- Charles Frankum

## Acknowledgements

Vernica, R., Carey, M. J.,Li, C. (2010). Efficient Parallel Set-Similarity Joins Using MapReduce. Technical report, Department of Computer Science, UC Irvine. http://asterix.ics.uci.edu/pub/sigmod10-p495-vernica-long.pdf
