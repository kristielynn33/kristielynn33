# AI Engineering Portfolio

## Reliable AI-assisted applications and tested workflows

I build independent portfolio projects that combine AI services with
traditional software engineering, data validation, and testing. My focus
is on applications that are transparent about their limitations,
easier to troubleshoot, and backed by automated checks rather than
unsupported claims.

This portfolio includes two projects:

### Document Knowledge Assistant

[View the repository](https://github.com/kristielynn33/document-knowledge-assistant)

A local Streamlit application for answering questions about invented
document policies. It retrieves source passages using TF-IDF, displays
the passages that will be sent, asks for approval before making an API
request, and validates the structured response against citation rules.

The system does not execute arbitrary SQL, does not invent missing facts,
and does not claim that valid citation identifiers guarantee that an
answer is supported.

Capabilities demonstrated include retrieval, citation tracking,
permission-gated AI requests, structured output validation, local JSON
review storage, and automated Python tests using simulated responses.

### AI-Assisted Sales Data Pipeline

[View the repository](https://github.com/kristielynn33/ai-assisted-sales-pipeline)

A supervised analytics workflow using Python, Gemini, LangGraph, DuckDB,
dbt, and Tableau Public. It validates sales CSVs, loads a local warehouse,
builds and tests dbt models, publishes a monthly reporting CSV, and
supports restricted natural-language questions.

Includes bounded retries, approval-gated header mapping, reconciliation
of regional query results, automated Python and dbt tests, and local
run reports. The pipeline uses invented sample data.

## Skills demonstrated across projects

### AI application engineering

- Gemini API integration.
- Structured output validation using Pydantic models.
- Retrieval-augmented question answering.
- Human-approval gates for AI actions.
- Limited retries and error handling.
- Source citation tracking.

### Software engineering

- Python.
- pytest with simulated AI responses.
- Git and GitHub Actions.
- Streamlit.
- Modular workflow nodes.

### Data and analytics engineering

- SQL and DuckDB.
- dbt models and data-quality checks.
- Metric reconciliation.
- Tableau reporting from verified CSV output.

### Troubleshooting demonstrated

- Diagnosed API service errors and selected working model alternatives.
- Resolved request-schema incompatibilities while keeping strict local
  validation.
- Fixed SSL certificate issues by configuring a trusted certificate
  bundle rather than disabling verification.
- Corrected Windows PATH and Git environment issues.

## Engineering principles

1. Validate AI output before using it.
2. Separate AI suggestions from actions.
3. Give tools only the capabilities needed for their task.
4. Preserve verified output when publication steps fail.
5. Test cancellation and failure paths, not only successful paths.
6. Distinguish software-test results from live AI-quality claims.
7. Document limitations and avoid unsupported business claims.
8. Keep API keys, private data, and local databases out of public
   repositories.

## Project verification

### Document Knowledge Assistant

- 28 automated Python tests.
- Manual review of live AI responses, including one appropriate
  insufficient-evidence response.
- No accuracy percentage is claimed from the reviewed responses.

### Sales Pipeline

- 61 automated Python tests.
- 17 separate dbt data checks.
- GitHub Actions runs the Python test suite.
- A saved Tableau visualization uses the monthly reporting CSV.
- The audio walkthrough uses invented sales data and a synthetic voice.

These verification points describe process checks and manual reviews,
not production performance.

## Portfolio links

- [Document Knowledge Assistant](https://github.com/kristielynn33/document-knowledge-assistant)
- [AI-Assisted Sales Data Pipeline](https://github.com/kristielynn33/ai-assisted-sales-pipeline)
- [All repositories](https://github.com/kristielynn33?tab=repositories)

These are independent portfolio projects using invented data. They do not
represent client engagements, employment experience, or production
systems.
