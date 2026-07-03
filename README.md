# [`oleander`](https://oleander.dev/) Skills

A collection of [agent skills](https://agentskills.io/home) for building with [oleander](https://oleander.dev/).

## Install via skills

Install from [skills.sh](https://skills.sh/) with:

```bash
npx skills add oleanderhq/skills
```

## Skills

| Skill | Useful for |
| --- | --- |
| [`lake-query`](skills/lake-query/SKILL.md) | Explore your data, compare seasonal revenue, analyze product changes, count new user signups, and answer questions hidden in your data. |
| [`lake-catalog`](skills/lake-catalog/SKILL.md) | Engine-agnostic guidance for working with the oleander lake catalog, including naming conventions, catalog hierarchy, and table reference patterns. |
| [`polars-submit`](skills/polars-submit/SKILL.md) | Run Polars queries or scripts on oleander, locally or distributed, and save results to the lake catalog. |
| [`spark-lake-catalog`](skills/spark-lake-catalog/SKILL.md) | Spark-specific patterns for reading and writing oleander lake catalog tables, including append vs overwrite, avoiding driver writes, and reusable table naming. |
| [`spark-lineage`](skills/spark-lineage/SKILL.md) | oleander-specific Spark guidance for connected OpenLineage, `collect()` pitfalls, and environment variable usage. |
| [`spark-submit`](skills/spark-submit/SKILL.md) | Submitting, monitoring, and configuring Spark jobs on oleander using the CLI and TypeScript SDK. |
| [`spark-best-practices`](skills/spark-best-practices/SKILL.md) | General Apache Spark best practices for scalable, maintainable, and performant DataFrame jobs. |
