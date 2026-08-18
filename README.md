# Quora Answer Matcher

An open-source, AI-assisted tool that finds and ranks public Quora questions that are a strong fit for a long-form answer.

> Status: planning and project setup. The first working version is not yet available.

## What it will do

1. Accept a long-form answer.
2. Identify the answer's main ideas, audience, claims, and search phrases.
3. Discover relevant public Quora question pages through a permitted web-search provider.
4. Rank the questions by how fully the answer addresses them.
5. Explain every recommendation, so the writer can decide whether to use it.

## What it will not do

- Post, comment, vote, or message on Quora automatically
- Bypass platform access controls
- Store API keys or user-submitted answers in the repository
- Claim affiliation with Quora

Every recommendation is for human review. A good result is not merely topically related—it is a question that the supplied answer substantially answers.

## Planned first release

Paste one answer and receive 10–20 ranked question matches, each with:

- Title and link
- Match score
- Reason for the match
- Coverage gaps or warnings
- A suggested adaptation note

The full product requirements are in [docs/PROJECT_SPEC.md](docs/PROJECT_SPEC.md).

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request. Never commit API keys, user answers, or copied third-party content.

## License

This project is licensed under the [Apache License 2.0](LICENSE).
