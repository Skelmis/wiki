+++
date = '2025-08-17'
title = ''
+++
Libraries that make Python unittest's better

{{< toc >}}

## Pytest

The goat. Swap out the built in testing library for this at your next sprint.

Link: <https://docs.pytest.org/en/stable/>

### pytest-asyncio

Lets pytest run `async def` tests. Must-have for async testing.

Example `pytest.ini` file:
```text
[pytest]
asyncio_mode = auto
asyncio_default_fixture_loop_scope = session
```

Link: <https://pypi.org/project/pytest-asyncio/>

## Freezegun

A must-have for anything that tests datetime objects. lets you automatically mock out dates and ensure every test runs with a fixed datetime.

Link: <https://github.com/spulec/freezegun>

## Faker

Faker is a Python package that generates fake data for you. Whether you need to bootstrap your database, create good-looking XML documents, fill-in your persistence to stress test it, or anonymize data taken from a production service, Faker is for you.

Link: <https://github.com/joke2k/faker>