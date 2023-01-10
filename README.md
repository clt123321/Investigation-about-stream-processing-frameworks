# Investigation-about-stream-processing-frameworks
EPCC MSc Project
## Project information
### Project title
- Investigation about stream processing frameworks
### Student's Name
- **Cheng Litao**
- [s2169894@ed.ac.uk](s2169894@ed.ac.uk)
### EPCC Suprvisor's information
- **ROUBICKOVA Anna**
- [a.roubickova@epcc.ed.ac.uk](a.roubickova@epcc.ed.ac.uk)
- **Edinburgh Parallel Computing Centre**

## Project Abstract

Big data processing can extract insight and value from massive data. The characteristics of rapid generation and low-value density of big data pose challenges to data processing methods. An ideal data processing system should have both high throughput and low response time . Streaming and batch processing are two common ways of processing big data. In some systems requiring fast response, stream processing has advantages over batch processing. Stream and micro-batch processing can be implemented for infinitely generated unbounded data streams. Stream processing frameworks can help to quickly develop unbounded data processing applications, such as Spark, Flink, and Strom. Stream processing frameworks can be used for business analytics, IoT and social media analytics. Due to the widespread use of stream processing, we really wanted to know the deployment details and applicable scenarios of different stream processing frameworks. To explore performance under different data pressures, we need to measure performance using stream processing benchmarking tools.


In this project, we summarize the stream processing architecture and deployment methods. Design ideas for four different open source stream processing benchmarks are discussed, and their strengths and weaknesses are evaluated. We propose a comprehensive metric for judging whether a stream processing application is stable. We explore Spark, Flink throughput, latency, and scalability on a local virtual machine cluster using four workloads from HiBench. The results show that, under the experimental conditions, compared with Spark and Flink, Spark's Maximum Stable Throughput(MST) dominates, while Flink's response time is significantly faster. When the data pressure is close to critical, Spark's MST is about twice that of Flink, and Flink's latency is less than 0.1 times that of Spark. Flink is better at stateful operations, especially window operations. Then the CPU-intensive applications are more scalable than IO-intensive applications. Finally, some performance tuning operations are also verified to be effective. Overall, Flink is more convenient to develop and has an absolute advantage in latency performance. Therefore, when throughput is not the main requirement, it is recommended to use Flink to develop stream processing applications. What is more, stream processing applications on HPC clusters are also a possible future exploration direction.
