# Product specification

## Purpose

Quora Answer Matcher helps a writer find existing public Quora questions that their long-form answer can address well.

## Version 1

The user pastes one answer and receives a ranked list of 10–20 public Quora question links. Each result includes:

- Question title and URL
- Match score
- Short explanation of the match
- Coverage warnings or gaps
- Suggested adaptation note

## Required workflow

1. Analyze the answer into themes, claims, audience, and search phrases.
2. Discover candidate public Quora pages through a permitted web-search provider.
3. Remove duplicates and invalid results.
4. Evaluate answer-to-question fit using a structured scoring rubric.
5. Display the ranked results for human review.

## Non-goals

- Automatic posting, commenting, voting, or messaging on Quora
- Storing user answers by default
- Scraping Quora pages or using credentials to bypass access restrictions
- Claiming affiliation with Quora

## Quality bar

A high-scoring result must be a question that the supplied answer substantially answers. Topic similarity alone is insufficient.

## Privacy and safety

API keys stay server-side and are supplied through environment variables. Do not commit secrets, user answers, copied Quora content, or search-provider credentials.
