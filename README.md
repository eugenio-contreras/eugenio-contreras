![header](https://capsule-render.vercel.app/api?type=waving&color=0:020B1F,50:0B3D91,100:00FF9C&height=120&section=header&animation=twinkling)

# Hi, I'm Eugenio <img src="resources/programmer.gif" width="40" alt="programmer" />

![python](https://img.shields.io/badge/python-0D0221?style=flat-square&logo=python&logoColor=00F0FF)
![java](https://img.shields.io/badge/java-0D0221?style=flat-square&logo=openjdk&logoColor=2979FF)
![scala](https://img.shields.io/badge/scala-0D0221?style=flat-square&logo=scala&logoColor=00FF9C)
![go](https://img.shields.io/badge/go-0D0221?style=flat-square&logo=go&logoColor=00F0FF)
![rust](https://img.shields.io/badge/rust-0D0221?style=flat-square&logo=rust&logoColor=2979FF)

![clickhouse](https://img.shields.io/badge/clickhouse-0D0221?style=flat-square&logo=clickhouse&logoColor=2979FF)
![kafka](https://img.shields.io/badge/kafka-0D0221?style=flat-square&logo=apachekafka&logoColor=00FF9C)
![flink](https://img.shields.io/badge/flink-0D0221?style=flat-square&logo=apacheflink&logoColor=00F0FF)
![dbt](https://img.shields.io/badge/dbt-0D0221?style=flat-square&logo=dbt&logoColor=00FF9C)
![dagster](https://img.shields.io/badge/dagster-0D0221?style=flat-square&logo=dagster&logoColor=2979FF)
![kubernetes](https://img.shields.io/badge/kubernetes-0D0221?style=flat-square&logo=kubernetes&logoColor=00F0FF)
![gcp](https://img.shields.io/badge/gcp-0D0221?style=flat-square&logo=googlecloud&logoColor=00FF9C)

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
      storage       = Seq("ClickHouse", "BigQuery", "Bigtable", "PostgreSQL", "Firestore", "MongoDB"),
      ingestion     = Seq("Apache Kafka", "Pub/Sub", "Airbyte"),
      processing    = Seq("Apache Beam/Dataflow", "Apache Flink", "dbt"),
      orchestration = Seq("Dagster", "Airflow"),
      infra         = Seq("Kubernetes", "Docker", "CI/CD", "Jenkins", "GCP", "AWS", "Azure"),
      tools         = Seq("Neovim", "Ghostty")
    ),
    // Long runs and zero-downtime deployments.
    offDuty = Seq("Running (negative splits only)")
  )

  println(s"${eugenio.name} | ${eugenio.role} | ${eugenio.location}")
}
```

![footer](https://capsule-render.vercel.app/api?type=waving&color=0:00FF9C,50:0B3D91,100:020B1F&height=100&section=footer&reversal=true)