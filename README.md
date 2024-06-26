# Big Data Analysis with Oozie Workflow on Flight Data

## Project Overview
This project demonstrates the use of Apache Oozie to orchestrate a Hadoop workflow for analyzing flight data. The analysis includes mapping and reducing tasks to process flight cancellations, on-schedule performance, and taxi times.

## Repository
This project is hosted on GitHub under the username `jinalthakkar7` in the repository [Big-Data-Analysis-with-Oozie-Workflow-on-Flight-Data](https://github.com/jinalthakkar7/Big-Data-Analysis-with-Oozie-Workflow-on-Flight-Data).

## Contents
- **CancellationsMapper.java**: Mapper class for processing flight cancellations.
- **CancellationsReducer.java**: Reducer class for processing flight cancellations.
- **OnScheduleMapper.java**: Mapper class for processing on-schedule performance of flights.
- **OnScheduleReducer.java**: Reducer class for processing on-schedule performance of flights.
- **TaxiTimeMapper.java**: Mapper class for processing taxi times of flights.
- **TaxiTimeReducer.java**: Reducer class for processing taxi times of flights.
- **Commands.txt**: File containing various commands used in the project.
- **Project Report CS644.pdf**: Detailed project report explaining the methodology, implementation, and results.
- **README.md**: Markdown version of the README file.
- **oozie workflow diagram.vsd**: Visual representation of the Oozie workflow.
- **output.txt**: Sample output of the workflow execution.
- **workflow.xml**: Oozie workflow definition file.

## Getting Started
1. **Set up Hadoop and Oozie**: Ensure you have a Hadoop cluster and Oozie set up and configured.
2. **Upload Data**: Place the flight data in HDFS (Hadoop Distributed File System).
3. **Compile Java Classes**: Compile the Java mapper and reducer classes.
4. **Run Oozie Workflow**:
   - Modify the `workflow.xml` file to match your environment settings.
   - Use the `Commands.txt` file for reference on how to submit the Oozie job.

## Workflow Description
The Oozie workflow is defined in the `workflow.xml` file and orchestrates the following steps:
1. **Flight Cancellations Analysis**: Uses `CancellationsMapper` and `CancellationsReducer`.
2. **On-Schedule Performance Analysis**: Uses `OnScheduleMapper` and `OnScheduleReducer`.
3. **Taxi Time Analysis**: Uses `TaxiTimeMapper` and `TaxiTimeReducer`.

## Results
The results of the workflow execution are stored in the specified HDFS output directories and summarized in the `output.txt` file.

## Project Report
For detailed information about the project, including the data sources, methodology, and results, refer to the `Project Report CS644.pdf`.

## Authors
- Jinal Thakkar

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.
