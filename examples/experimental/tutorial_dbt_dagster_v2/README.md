# (Experimental) dbt with software-defined assets tutorial example

This example demonstrates how to integrate dbt with Dagster using dbt's example [jaffle shop project](https://github.com/dbt-labs/jaffle_shop), the [dagster-dbt library](/\_apidocs/libraries/dagster-dbt), and a [DuckDB database](https://duckdb.org/).

In this example, we use the new `dagster-dbt` APIs that require the usage of `dbt-core>=1.4.0`.

---

## Getting started

To install this example and its dependencies, run:

```shell
cd my-dagster-project
pip install -e ".[dev]"
```

Compile the dbt project:

```shell
cd jaffle_shop
dbt compile
```

At this point, you can view the **completed** project in the Dagster UI by running:

```shell
cd ..
dagster dev
```
