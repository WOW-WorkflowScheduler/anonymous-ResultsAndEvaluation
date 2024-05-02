# Results

The results are followed as follows:

```
result
├── <Network Speed>(-Number of Nodes)
│   ├── <Workflow>
│   │   ├── <Method>-<DFS>
│   │   │   ├── <Repetition>(-failure)
│   │   │   │   ├── (copytasks.csv)
│   │   │   │   ├── dag.html
│   │   │   │   ├── dataOnNode.csv
│   │   │   │   ├── dataOnSharedFS.csv
│   │   │   │   ├── launch
│   │   │   │   |   ├── .nextflow.log
│   │   │   │   ├── nextflow.config
│   │   │   │   ├── report.html
│   │   │   │   ├── scheduler.log
│   │   │   │   ├── timeline.html
│   │   │   │   └── trace.csv
...
<year>-<month>-<data>--<time>.log
...
```
- If no number of nodes is defined, 8 nodes were used.
- `copytasks.csv` only exists for our WOW approach (here this method is called la)
- Unsuccessful runs are marked with a failure and timestamp.
- `<year>-<month>-<data>--<time>.log` are the logs of our management script orchestrating the experiments.

# Evaluation

- `evaluation.ipynb` Script to read the results and create plots and summary tables from the data.
- `evaluation` a folder with different tables
- `plots` visualizing the data