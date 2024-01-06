# Chat with SQLite Database

## Introduction

This workspace is a Python project that uses the OpenAI API to interact with a SQLite database. It is designed to handle chat-based interactions, where the AI can execute SQL queries based on the user's input and generate reports from the results.

The project is structured in a way that separates the different responsibilities into distinct modules. The `main.py` file is the entry point of the application, where the chat model and the agent executor are set up. The `handlers` directory contains the `ChatModelStartHandler` class, which handles the start of a chat model. The `tools` directory contains utility functions for interacting with the SQLite database (`sql.py`) and for writing HTML reports (`reports.py`).

## Usage Instructions

1. Install the required Python packages. This project uses several packages such as `langchain`, `pyboxen`, and `pydantic`. You can install them using pip:

```sh
pip install langchain pyboxen pydantic
```

2. Run the `main.py` script to start the application:

```sh
python main.py
```

3. The application will start a chat-based interaction. You can input SQL queries in a conversational manner, and the application will execute them against the SQLite database (`db.sqlite`).

4. If you ask for a report, the application will generate an HTML report using the `write_report` function from `reports.py`.

# Limitations

The application is designed to handle simple SQL queries. It does not support complex queries such as joins, subqueries, and aggregations. It also does not support SQL statements such as `CREATE TABLE`, `ALTER TABLE`, and `DROP TABLE`.
