# Multi-Environment Configuration Analysis

This directory contains configuration files for three different environments that need to be analyzed in parallel.

## Objective

Analyze multiple environment configurations simultaneously to generate comprehensive reports on each environment's setup, data characteristics, and configuration parameters.

## Environment Structure

```
├── working_dir1/          # Development environment
│   ├── config.txt        # Environment configuration
│   ├── data.txt         # Sample data
│   └── src/main.py      # Application script
├── working_dir2/         # Staging environment  
│   ├── config.txt       # Environment configuration
│   ├── data.txt         # Sample data
│   └── src/main.py      # Application script
├── working_dir3/         # Production environment
│   ├── config.txt       # Environment configuration
│   ├── data.txt         # Sample data
│   └── src/main.py      # Application script
└── results/             # Output directory for analysis reports
```

## Task Requirements

Create parallel Task agents to analyze all three environments simultaneously. Each agent should:

1. **Use `cd` command to navigate to assigned environment directory**
2. **Generate environment analysis reports**
3. **Extract configuration parameters**
4. **Analyze data characteristics**
5. **Create summary reports**

## Suggested Approach

Use the Task tool to create 3 agents running in parallel:

- Agent 1: Use `cd working_dir1/` then analyze the development environment
- Agent 2: Use `cd working_dir2/` then analyze the staging environment  
- Agent 3: Use `cd working_dir3/` then analyze the production environment

Each agent should first change directory using the `cd` command to their assigned environment directory, then work independently within that directory to generate detailed analysis reports.

## Expected Deliverables

Each agent should produce:
- Environment working directory analysis
- Configuration parameter extraction
- Data file analysis and statistics
- Summary report with key findings
- All outputs saved to `results/` directory with appropriate naming