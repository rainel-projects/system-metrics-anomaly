# system-metrics-anomaly

![Build Status](https://github.com/rainel-projects/system-metrics-anomaly/workflows/CI/badge.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

ML-based system metrics anomaly detection using IsolationForest and DBSCAN.

## Architecture

Combines IsolationForest for outlier detection with DBSCAN for density-based clustering to identify anomalous system metrics patterns.

## Tech Stack

- **Algorithms**: IsolationForest, DBSCAN
- **ML Library**: scikit-learn
- **Visualization**: matplotlib, seaborn
- **Dataset**: Public metrics dataset

## Quick Start

### Using Docker Compose (Recommended)

```bash
# Clone the repository
git clone https://github.com/rainel-projects/system-metrics-anomaly.git
cd system-metrics-anomaly

# Start services
docker-compose up -d

# View logs
docker-compose logs -f
```

### Run Detector
```bash
python src/detector.py --dataset data/metrics.csv
```

## Project Structure

```
system-metrics-anomaly/
├── src/              # Source code
├── benchmarks/       # Performance benchmarks
├── docs/             # Documentation
├── Dockerfile        # Container image
├── docker-compose.yml
└── .github/workflows/ # CI/CD pipelines
```

## Benchmarks

Run performance benchmarks:

```bash
cd benchmarks
./bench.sh
```

## Contributing

Contributions welcome! Please open an issue or submit a PR.

## License

MIT License - see LICENSE file for details.
