# [`oleander`](https://oleander.dev/) Skills

A collection of [agent skills](https://agentskills.io/home) for building with [oleander](https://oleander.dev/).

[Browse on skills.sh](https://skills.sh/oleanderhq/skills)

## Install

```bash
npx skills add OleanderHQ/skills -g -y
```

## Skills

| Skill | Use when |
| --- | --- |
| [`lake-query`](skills/lake-query/SKILL.md) | Querying lake tables, writing query results to a table, or handling engine routing and billing errors |
| [`lake-catalog`](skills/lake-catalog/SKILL.md) | Naming tables, choosing namespaces, or referencing the lake catalog |
| [`polars-submit`](skills/polars-submit/SKILL.md) | Running Polars via the CLI (query/script, local/distributed, `--save`) |
| [`spark-lake-catalog`](skills/spark-lake-catalog/SKILL.md) | Reading or writing Iceberg tables from Spark jobs |
| [`spark-lineage`](skills/spark-lineage/SKILL.md) | Fixing disconnected OpenLineage or avoiding `collect()` between read and write |
| [`spark-submit`](skills/spark-submit/SKILL.md) | Submitting, monitoring, or automating Spark jobs (MCP, CLI, SDK) |
| [`spark-best-practices`](skills/spark-best-practices/SKILL.md) | Optimizing or reviewing general Spark DataFrame jobs |

### Former skill names

These older skill IDs were renamed. Prefer the current names above:

| Former | Current |
| --- | --- |
| `oleander-spark-lineage` | `spark-lineage` |
| `oleander-spark-submit` | `spark-submit` |
| `oleander-iceberg-catalog` | `lake-catalog` / `spark-lake-catalog` |
