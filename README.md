# EDGAR

**AI tool for integrating APIs.** 

Try it out now at [superface.ai/edgar](https://superface.ai/edgar)

EDGAR reads and analyzes API docs so you don't have to. Then, based on your plain english input, EDGAR builds the API integration to be used via [Superface OneService](https://github.com/superfaceai/one-service).

This repository is the datasource of APIs for EDGAR.

[→ Add API](#add-api)<br />
[→ Check available APIs](./docs)<br />
[→ Provide feedback](https://github.com/superfaceai/edgar-community/issues/new?template=FEEDBACK.md)

## Add API

You can add an API by **opening a new pull request with the API documentation**. Upon review and merging, EDGAR will index the documentation and once ready, it will become available at [superface.ai/edgar](https://superface.ai/edgar)

### API documentation format

The format for the API documentation is a **plain text**. Markdown is welcome but not required.

When formating the API documentation, it is important to **use the separator**. The documentation consists of various topics, divided by pages or headings. These includes _authentication, rate limiting, general instructions, API operations (often grouped by resources), and others_. When submitting the API docs, use the _the separator_ to split these topisc.

The separator is a sequence of equal signs (`===========`) terminated by a newline. At minimum use 5 _equal_ (`=`) characters to form a separator. The API docs ready for EDGAR might look something like the following:

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

[Check existing APIs](./docs) for more examples.

The entire API documentation is then stored in as a **single text `.txt` file in `docs` directory**.

Opened pull request are usually reviewed in few hours. In the meantime, consider starring this repo so that you don't miss new development.

If you don't want to submit an API docs on your own, feel free to [suggest a new API](https://github.com/superfaceai/edgar-community/issues/new?template=NEW_API.yml) and we will add it for you!





