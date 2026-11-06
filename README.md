# AI Engineering Portfolio

### Reliable LLM applications, controlled tool use, and tested workflows

I build and troubleshoot independent projects that combine AI services
with practical software and data engineering.

My focus is making AI-assisted applications easier to validate,
debug, and operate—not simply connecting a prompt to an API.

This portfolio documents my completed work, engineering decisions,
and the capabilities I am developing next.

## Featured project: AI-Assisted Sales Data Pipeline

**Status: Working portfolio MVP**

[View the source code, documentation, Tableau screenshot, and audio walkthrough](https://github.com/kristielynn33/ai-assisted-sales-pipeline)

A supervised analytics workflow built with Python, Gemini, LangGraph,
DuckDB, dbt, and Tableau.

```text
Sales CSV
    -> Cleaning and record validation
    -> DuckDB warehouse
    -> dbt models and data-quality checks
    -> Verified reporting CSV
    -> Tableau
```

### AI capabilities

- Proposes mappings for unfamiliar CSV headers.
- Requires permission before requesting an AI proposal.
- Requires human approval before applying header mappings.
- Converts supported business questions into structured query plans.
- Uses fixed, parameterized SQL instead of executing arbitrary
  model-generated SQL.
- Compares regional query results with the Tableau-ready reporting CSV
  before displaying a verified answer.

### Reliability and safeguards

- Pydantic validation for records and query plans.
- Read-only connections for answering questions.
- Bounded retries for selected temporary API errors.
- Temporary-file verification before publishing CSV output.
- Local run reports.
- Automated tests and GitHub Actions continuous integration.

### Verification checkpoint

- 61 automated Python tests.
- 17 separate dbt data tests.
- GitHub Actions runs the Python tests and dependency checks.
- January sample revenue reconciled at $4,650.50.
- A saved Tableau visualization built from the reporting output.

The test counts describe software and data-quality checks.
They are not a measurement of model accuracy.

### Troubleshooting demonstrated

- Diagnosed unavailable model responses and configured a working option.
- Handled temporary API service errors with limited retries.
- Resolved API request-schema incompatibilities while retaining
  strict local validation.
- Resolved a dependency-download certificate error without disabling
  certificate verification.
- Corrected Windows Git and PATH configuration issues.
- Used error logs and automated tests to verify fixes.

### Current scope

This is an independent portfolio project using invented sales data,
not a client deployment.

AI assistance is limited to approved header mappings and supported
regional-revenue questions. It does not repair arbitrary datasets
or execute unrestricted SQL.

Answer reconciliation checks the local reporting CSV, not the current
state of an online Tableau dashboard.

## Next project: Document Knowledge Assistant

**Status: Planned — not implemented yet**

A document question-answering application designed to answer from
retrieved evidence and cite its sources.

### Planned capabilities

- Ingest a small collection of public or invented documents.
- Split documents into searchable passages.
- Retrieve relevant passages for a question.
- Generate answers grounded in those passages.
- Display source citations.
- Identify questions that the available documents cannot answer.
- Treat retrieved document content as untrusted data.
- Evaluate retrieval and answer quality using a documented question set.

### Planned evaluation

- Retrieval relevance.
- Citation correctness.
- Whether answers are supported by the cited passages.
- Handling of unsupported questions.
- Response latency and API usage.

Results will be published after implementation and measurement.
No accuracy or cost-reduction claims are made in advance.

## Skills demonstrated in completed work

### AI application engineering

- Gemini API integration.
- Structured model outputs.
- Local schema validation.
- Human approval gates.
- Restricted tool execution.
- Error handling and bounded retries.

### Software engineering

- Python.
- Modular tools and workflow nodes.
- pytest.
- Mocked service responses.
- Git and GitHub.
- GitHub Actions.

### Data and analytics engineering

- SQL and DuckDB.
- dbt staging and reporting models.
- Data contracts and quality checks.
- Metric reconciliation.
- Tableau reporting.

## Engineering principles

1. Validate model output before using it.
2. Separate AI suggestions from actions.
3. Give tools only the capabilities they need.
4. Preserve verified output when publication fails.
5. Test cancellation and failure paths, not just successful runs.
6. Distinguish software tests from AI-quality evaluation.
7. Document limitations and avoid unsupported business claims.
8. Keep credentials and confidential data out of public repositories.

## Portfolio links

- [Completed sales-pipeline project](https://github.com/kristielynn33/ai-assisted-sales-pipeline)
- [GitHub repositories](https://github.com/kristielynn33?tab=repositories)

This portfolio presents independent project work. It does not imply
client engagements or employment experience.
