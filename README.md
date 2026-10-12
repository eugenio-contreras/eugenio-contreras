# Hi, I'm Eugenio <img src="resources/programmer.gif" width="40" alt="programmer" />

![python](https://img.shields.io/badge/python-3776AB?style=flat-square&logo=python&logoColor=white)
![java](https://img.shields.io/badge/java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![scala](https://img.shields.io/badge/scala-DC322F?style=flat-square&logo=scala&logoColor=white)
![go](https://img.shields.io/badge/go-00ADD8?style=flat-square&logo=go&logoColor=white)
![rust](https://img.shields.io/badge/rust-000000?style=flat-square&logo=rust&logoColor=white)

```scala
case class TechStack(
  languages: Seq[String],
  storage: Seq[String],
  ingestion: Seq[String],
  processing: Seq[String],
  orchestration: Seq[String],
  infra: Seq[String],
  tools: Seq[String]
)

case class Engineer(
  name: String,
  role: String,
  location: String,
  stack: TechStack,
  offDuty: Seq[String]
)

object AboutMe extends App {
  val eugenio = Engineer(
    name = "Eugenio Contreras",
    role = "Senior Data Engineer / Data Platform Architect",
    location = "Düsseldorf, Germany",
    stack = TechStack(
      languages     = Seq("Python", "Java", "Scala", "Go", "Rust", "SQL"),
      storage       = Seq("ClickHouse", "BigQuery", "Bigtable", "PostgreSQL", "Firestore", "SQLite", "LanceDB"),
      ingestion     = Seq("Apache Kafka", "Pub/Sub", "Airbyte"),
      processing    = Seq("Apache Beam/Dataflow", "Apache Flink", "dbt"),
      orchestration = Seq("Dagster", "Airflow"),
      infra         = Seq("Kubernetes", "Docker", "CI/CD", "GCP", "AWS", "Azure"),
      tools         = Seq("Neovim", "Ghostty")
    ),
    // Long runs and zero-downtime deployments.
    offDuty = Seq("Running (negative splits only)")
  )

  println(s"${eugenio.name} | ${eugenio.role} | ${eugenio.location}")
}
```