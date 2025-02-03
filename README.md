# hadoop-playground

A hands-on experimental repository for learning and testing Apache Hadoop ecosystem components. This playground is for practicing MapReduce, HDFS, YARN, and related technologies.

## 🎯 Purpose

This repository serves as a sandbox environment for:
- Experimenting with Hadoop ecosystem components
- Testing MapReduce programs
- Understanding HDFS operations
- Learning YARN resource management
- Practicing with various Hadoop tools
- Quick prototypes and proofs of concept

## 🗂️ Repository Structure

```
hadoop-playground/
├── mapreduce/           # MapReduce examples and exercises
├── hdfs/                # HDFS operations and examples
├── yarn/                # YARN configurations and tests
├── docker/              # Docker setup for Hadoop environment
├── data/                # Sample datasets for testing
├── scripts/             # Utility scripts
└── docs/                # Notes and documentation
```

## 🐘 Components Covered

- **Core Hadoop**
  - HDFS
  - MapReduce
  - YARN

- **Data Processing**
  - MapReduce Jobs
  - File Operations
  - Data Loading
  - Data Export

- **Resource Management**
  - YARN Configuration
  - Resource Allocation
  - Job Scheduling

## 🚀 Getting Started

1. Start Hadoop environment:
```bash
docker-compose up -d
```

2. Verify the setup:
```bash
docker exec -it hadoop-master hdfs dfs -ls /
```

3. Run example MapReduce job:
```bash
./scripts/run-wordcount.sh
```

## 📊 Example Projects

1. **Word Count**
   - Basic MapReduce example
   - Located in `/mapreduce/wordcount/`
   - Demonstrates the MapReduce paradigm

2. **Log Analysis**
   - Parse and analyze log files
   - Located in `/mapreduce/loganalysis/`
   - Shows practical usage of MapReduce

3. **HDFS Operations**
   - Basic file operations
   - Located in `/hdfs/operations/`
   - Common HDFS commands and usage

## 🔧 Setup Options

### Docker Setup
```bash
# Build and start containers
docker-compose up -d

# Stop containers
docker-compose down
```

### Local Setup
```bash
# Start HDFS
start-dfs.sh

# Start YARN
start-yarn.sh
```

## 📝 Learning Resources

- **Official Documentation**
  - [Apache Hadoop](https://hadoop.apache.org/docs/current/)
  - [HDFS Architecture](https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/HdfsDesign.html)
  - [MapReduce Tutorial](https://hadoop.apache.org/docs/current/hadoop-mapreduce-client/hadoop-mapreduce-client-core/MapReduceTutorial.html)

- **Example Code**
  - Check `/examples` directory for annotated code samples
  - Each example includes README with explanation

## 🧪 Testing

1. HDFS Tests:
```bash
./scripts/test-hdfs.sh
```

2. MapReduce Tests:
```bash
./scripts/test-mapreduce.sh
```

## 🔍 Debugging Tips

- Check logs in `/logs` directory
- Use `hadoop fs -ls` to verify HDFS contents
- Monitor YARN Resource Manager UI (localhost:8088)
- Check container logs using `docker logs`

## 🤝 Contributing

Feel free to:
- Add new examples
- Improve documentation
- Share interesting use cases
- Report issues
- Suggest improvements

## 📜 License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*This is an experimental playground. Code here is for learning purposes.*
