# Data Engineering Fundamentals

This repository documents core data engineering concepts that form the foundation of modern analytics and data platforms. It focuses on *design principles*, *system tradeoffs*, and *data modeling strategies* rather than implementation-specific code.

The goal of this repository is to demonstrate conceptual understanding used by data engineers when designing scalable, reliable data systems.

---

## Topics Covered

### OLTP vs OLAP Systems
- Differences between transactional and analytical workloads
- Performance characteristics and schema design considerations
- Why modern architectures separate operational and analytical systems

📄 See: `olap-vs-oltp.md`

---

### Star Schema Data Modeling
- Fact and dimension tables
- Dimensional modeling for analytics
- Tradeoffs between star schemas and normalized schemas

📄 See: `star-schema.md`

---

### Slowly Changing Dimensions (SCD)
- Strategies for managing historical changes in dimension data
- SCD Types 0, 1, 2, and 3
- Common real-world use cases and tradeoffs

📄 See: `scd-types.md`

---

## Why This Matters

Data engineers must understand *how data is structured, stored, and queried* before building pipelines and analytics systems. These concepts guide decisions around:

- Data warehouse design
- Query performance
- Historical data accuracy
- Scalability and maintainability

This repository serves as a conceptual reference that supports more advanced projects involving ETL pipelines, cloud data platforms, and analytics systems.

---

## Author

**Hashim Nahidian**  
Data Engineering | AWS | Python | SQL  
George Mason University – IT (Databases & Programming)
