# EDGAR

**EDGAR is an AI-powered assistant for integrating APIs.**

At heart, EDGAR differs from other AI agents by leveraging existing API docs to create your integration. This means the AI engine first analyzes the human-readable documentation and then builds your use case from that. In other words — **it reads and analyzes the docs so you don't have to**.


**[→ Add your favorite API](#adding-your-api)<br />**
[→ Check requested APIs pipeline](https://github.com/superfaceai/edgar/issues?q=is%3Aissue+is%3Aopen+label%3Aapi-request)<br />
[→ Send us feedback about EDGAR](https://github.com/superfaceai/edgar/issues/new?template=FEEDBACK.md)

---

## Adding your API

We embrace new APIs being added to EDGAR! You can add your API by **opening a new pull request with the API documentation**.

#### Format

The expected format for the API documentation is **plain text**. Markdown is welcome but not required.

The major part of formatting the docs is **using the separator**. The documentation conventionally consists of various topics, usually set apart by separate pages or big headings. They might be _authentication, rate limiting, general rules, API operations (sometimes grouped by resources)_.

It's highly recommended each of these topics (or chunks) is set apart in the docs provided for EDGAR, too. For that, we use _the separator_.

The separator is a long `===========` ended with a newline. Technically 5 _equal_ characters are enough to form a separator. The API docs ready for EDGAR might look something like the following:

```
# Welcome to our docs
(...)
================================
# API Basics
(...)
================================
# Authorizing Requests
(...)
================================
# /todos/:id/items
This endpoint lists all items (...)
================================
(...)
```

Entire documentation for an API provider is then stored in a single `.txt` file in `docs` directory.

Then, open a pull request and wait for one of our reviewers to approve the new API. In the meantime, consider Starring the repo so that you don't miss new development.
