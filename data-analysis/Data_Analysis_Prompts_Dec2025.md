# Data Analysis & Technical Prompt Library
Last Updated: December 2025

## SQL Query Generation

### CDW Data Extraction Template
Generate SQL query for VA Corporate Data Warehouse:
- Specify timeframe and patient population
- Include relevant clinical/administrative data elements
- Apply appropriate filters and exclusions
- Use proper table joins
- Include data quality checks

### Performance Metrics Query
Create query to calculate operational metrics:
- Encounter volume by clinic/provider
- Wait times and access measures
- No-show rates and patterns
- Productivity indicators
- Trend analysis over time

### Quality Measure Calculation
Generate SQL for quality measure reporting:
- Numerator and denominator definitions
- Exclusion criteria application
- Risk adjustment factors
- Stratification requirements
- Benchmark comparisons

## Excel/Power BI

### Pivot Table Design
Create Excel pivot table structure for:
- Multi-dimensional data analysis
- Calculated fields and measures
- Conditional formatting rules
- Slicer configuration
- Dashboard layout

### Power BI DAX Formula
Generate DAX measures for:
- Complex calculations
- Time intelligence functions
- Conditional aggregations
- KPI indicators
- Comparative analysis

### Data Visualization Selection
Recommend appropriate chart types for:
- Trend analysis over time
- Comparison across categories
- Distribution analysis
- Relationship identification
- Part-to-whole representation

## Statistical Analysis

### Descriptive Statistics Summary
Calculate and interpret basic statistics:
- Measures of central tendency
- Measures of variability
- Distribution assessment
- Outlier identification
- Confidence intervals

### Hypothesis Testing Framework
Design statistical test for:
- Research question formulation
- Appropriate test selection
- Sample size calculation
- Assumption verification
- Result interpretation

## Automation & Workflow

### Process Automation Design
Design automation solution for:
- Repetitive task identification
- Workflow mapping
- Tool selection (Excel macros, Power Automate, etc.)
- Error handling
- Testing and validation

### Report Template Creation
Generate automated report structure:
- Data source connection
- Refresh schedule
- Formatting standards
- Distribution list
- Version control

## System Integration

### Data Integration Planning
Plan integration between systems:
- Data mapping and transformation
- Validation rules
- Error handling procedures
- Testing strategy
- Maintenance plan

---

## Custom Instructions for Data Analysis Space

```
You are supporting advanced data analysis and technical work for VA 
healthcare operations and research.

When handling data analysis prompts:
1. Generate executable code with clear documentation
2. Follow VA data security and privacy requirements
3. Use VA-standard data sources (CDW, VSSC) when applicable
4. Include data validation and quality checks
5. Explain statistical methods and assumptions
6. Provide interpretation suitable for non-technical stakeholders

For SQL queries:
- Use proper VA CDW table structures and naming conventions
- Optimize for performance with large datasets
- Include comments explaining complex logic
- Handle NULL values and edge cases

For visualizations:
- Follow data visualization best practices
- Consider colorblind-friendly palettes
- Include clear titles, labels, and legends
- Make charts actionable for decision-making

For statistical analysis:
- Verify assumptions before applying tests
- Report effect sizes, not just p-values
- Consider clinical significance vs statistical significance
```