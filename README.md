# AI Engineering Portfolio

## Reliable AI-assisted applications and tested workflows

I build independent portfolio projects that combine AI services with
software engineering, data validation, and human review.

My focus is on creating applications that are transparent about their
sources and limitations, and easier to test and troubleshoot.

## Featured Project 1: Document Knowledge Assistant

**Status: Working portfolio prototype**

[View the Document Knowledge Assistant repository](https://github.com/kristielynn33/document-knowledge-assistant)

A document question-answering prototype built with Python, Gemini,
Streamlit, and scikit-learn. It uses two invented company-policy documents.

```text
Question
   -> Local passage retrieval
   -> Review the passages
   -> Permission to send them to Gemini
   -> Proposed answer or insufficient-evidence response
   -> Display citations for human review
```

### What it demonstrates

- Local TF-IDF passage retrieval.
- A Streamlit browser interface.
- Permission before sending questions and passages to Gemini.
- Structured response and citation-ID validation.
- Source excerpts displayed alongside proposed answers.
- Insufficient-evidence handling for unsupported questions.
- Offline retrieval evaluation and recorded human reviews.
- Automated tests using simulated AI responses.
- GitHub Actions continuous integration.

### Verification checkpoint

- **28 automated Python tests** passed locally.
- The GitHub Actions workflow completed successfully.
- Four sample retrieval questions found their expected passages in the
  top three results.
- Two selected live responses were manually reviewed: one supported
  answer and one appropriate insufficient-evidence response.

### Limitations

These small evaluations do not establish general model accuracy.
A valid citation ID does not by itself prove that the passage supports
the answer. TF-IDF measures word similarity, not confidence.

The project is a local prototype using invented documents—not a
production service or a client deployment.

## Featured Project 2: AI-Assisted Sales Data Pipeline

**Status: Working portfolio MVP**

[View the AI-Assisted Sales Data Pipeline repository](https://github.com/kristielynn33/ai-assisted-sales-pipeline)

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

### AI and data capabilities

- Proposes mappings for unfamiliar CSV headers with human approval.
- Validates sales records before loading and publishing data.
- Builds staging and monthly reporting models in dbt.
- Supports selected natural-language questions through structured plans.
- Executes fixed, parameterized SQL using a read-only connection.
- Reconciles regional query results against the Tableau-ready CSV.

### Reliability and troubleshooting

- Bounded retries for selected temporary API failures.
- Temporary-file verification before publishing CSV output.
- Local run reports and automated tests.
- Diagnosed API availability and request-schema issues.
- Resolved a dependency-download certificate issue without disabling
  certificate verification.
- Corrected Windows Git and PATH configuration issues.

### Verification checkpoint

- **61 automated Python tests** passed locally.
- **17 separate dbt data tests** passed in the reporting build.
- GitHub Actions runs the Python test suite.
- The sample January regional-revenue result reconciled at **$4,650.50**.

The repository includes documentation, a Tableau screenshot, and an
audio walkthrough. It uses invented sales data.

## Skills demonstrated

### AI application engineering

- Gemini API integration
- Retrieval-augmented question answering
- Structured response validation
- Source citations and human review
- Permission gates and restricted tool use
- Evaluation documentation and failure handling

### Software engineering

- Python
- pytest and simulated API responses
- Git and GitHub Actions
- Streamlit
- Modular workflow components

### Data and analytics engineering

- SQL and DuckDB
- dbt models and data-quality checks
- Pydantic data contracts
- Metric reconciliation
- Tableau reporting

## Engineering principles

1. Validate model output before using it.
2. Show users what will be sent to an external AI service.
3. Separate AI suggestions from actions.
4. Give tools only the capabilities needed for their task.
5. Test cancellation and failure paths—not only successful runs.
6. Distinguish software-test results from measured AI-answer quality.
7. Document limitations and avoid unsupported business claims.
8. Keep credentials and confidential data out of public repositories.

## Project links

- [Document Knowledge Assistant](https://github.com/kristielynn33/document-knowledge-assistant)
- [AI-Assisted Sales Data Pipeline](https://github.com/kristielynn33/ai-assisted-sales-pipeline)
- [All GitHub repositories](https://github.com/kristielynn33?tab=repositories)

These are independent portfolio projects. They do not imply client
engagements, employment experience, or production deployments.
