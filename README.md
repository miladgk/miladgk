# Milad Ghaemi, PhD

[![Portfolio](https://img.shields.io/badge/Portfolio-miladgk.github.io-2563eb?style=for-the-badge&logo=googlechrome&logoColor=white)](https://miladgk.github.io/)

**🌐 [Explore Interactive Portfolio & Engineering Workflows](https://miladgk.github.io/)**

**Computational Materials Physics | Data Engineering & Scientific ML | Helsinki, Finland**

[![Portfolio Website](https://img.shields.io/badge/Portfolio_Website-miladgk.github.io-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white)](https://miladgk.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Milad_Ghaemi-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/milad-ghaemikermani/)
[![Google Scholar](https://img.shields.io/badge/Google_Scholar-Publications-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white)](https://scholar.google.com/citations?hl=en&user=dzrQ6WsAAAAJ)

I build reliable data platforms, scientific machine-learning workflows, and computational simulation tools. My work connects industrial analytics, atomistic simulation, finite-element modeling, and reproducible research software.

## Focus Areas

- **Data Engineering:** ingestion, PostgreSQL analytics, dimensional modeling, dbt, Airflow, data quality, and observability
- **Scientific ML:** feature engineering, anomaly detection, forecasting, classification, explainability, and model validation
- **Computational Materials:** ML interatomic potentials, kinetic Monte Carlo, molecular dynamics, electronic structure, and multiscale simulation
- **Computational Mechanics:** finite elements, geometry/mesh processing, solver verification, HPC, and MPI workflows

## Featured Public Projects

### [Industrial Energy SQL Pipeline](https://github.com/miladgk/industrial-energy-sql-pipeline)

[![CI](https://github.com/miladgk/industrial-energy-sql-pipeline/actions/workflows/ci.yml/badge.svg)](https://github.com/miladgk/industrial-energy-sql-pipeline/actions/workflows/ci.yml)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Scale](https://img.shields.io/badge/Scale-6.3M_rows-6f42c1?style=flat-square)
![Idempotency](https://img.shields.io/badge/Loading-Idempotent-2ea44f?style=flat-square)

An end-to-end data engineering platform for industrial energy facilities, combining high-volume ingestion, PostgreSQL analytics, SQL anomaly detection, automated quality checks, and Metabase reporting.

**Highlights:** approximately **6.3 million** five-minute sensor readings; incremental high-watermark ingestion; database-level conflict-safe inserts; normalized PostgreSQL schema; window functions and ranking analytics; pytest checks; Dockerized local setup; Metabase dashboard.

```mermaid
flowchart LR
    A[Synthetic telemetry generator] --> B[CSV data lake]
    B --> C[Incremental ingestion]
    C --> D[(PostgreSQL)]
    D --> E[Quality checks]
    D --> F[SQL analytics]
    F --> G[Anomaly detection]
    F --> H[Facility ranking]
    F --> I[Rolling metrics]
    G --> J[Metabase dashboard]
    H --> J
    I --> J
```

### [Amorphous Phase ML](https://github.com/miladgk/amorphous-phase-ml)

[![CI](https://github.com/miladgk/amorphous-phase-ml/actions/workflows/ci.yml/badge.svg)](https://github.com/miladgk/amorphous-phase-ml/actions/workflows/ci.yml)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LAMMPS](https://img.shields.io/badge/LAMMPS-Scientific_Computing-1f6feb?style=flat-square)
![scikit--learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Descriptors](https://img.shields.io/badge/Features-18_per_atom-6f42c1?style=flat-square)
![Macro F1](https://img.shields.io/badge/Macro_F1-0.854-2ea44f?style=flat-square)

A materials-science machine-learning workflow for identifying polyamorphous phases in metallic glasses from atomistic simulation data.

**Highlights:** LAMMPS trajectory processing; **18 structural descriptors per atom**; group-aware splitting; HistGradientBoosting classification; **0.854 macro F1**; SHAP and permutation importance; calibration; deployment to new datasets.

```mermaid
flowchart LR
    A[LAMMPS trajectories] --> B[Trajectory post-processing]
    B --> C[Per-atom structural descriptors]
    C --> D[Feature validation]
    D --> E[Group-aware split]
    E --> F[Model training]
    F --> G[Evaluation and calibration]
    F --> H[SHAP / permutation importance]
    G --> I[Phase predictions]
    H --> J[Scientific interpretation]
    I --> J
```

### [Aether Climate Engine](https://github.com/miladgk/aether-climate-engine)

[![CI](https://github.com/miladgk/aether-climate-engine/actions/workflows/ci.yml/badge.svg)](https://github.com/miladgk/aether-climate-engine/actions/workflows/ci.yml)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Forecasting](https://img.shields.io/badge/Forecasting-Multi--model-6f42c1?style=flat-square)

A real-time meteorological telemetry platform combining global station ingestion, statistical anomaly detection, forecasting, dimensional modeling, and an interactive field-station dashboard.

**Highlights:** Open-Meteo and AWS S3 ingestion; PostgreSQL raw layer; dbt staging/fact/mart models; Apache Airflow orchestration; linear, SMA, and EMA forecasting; 365-day year-over-year comparisons; pytest mocks; Bandit AST scanning; GitHub Actions CI.

```mermaid
flowchart LR
    A[Open-Meteo / AWS S3] --> B[Telemetry ingestion]
    B --> C[(PostgreSQL raw layer)]
    C --> D[dbt staging models]
    D --> E[Dimensional marts]
    E --> F[Anomaly detection]
    E --> G[Forecasting engine]
    F --> H[Field-station dashboard]
    G --> H
    I[Apache Airflow] --> B
    I --> D
```

## Selected Private & R&D Projects

These projects remain **strictly private**. The summaries below describe architecture and technical contributions without exposing confidential source code, private datasets, credentials, or operational details.

| Project | Area | Architecture / stack | Selected technical signal |
|---|---|---|---|
| **MLIP–KMC Research Review** *(Private)* | Scientific research | LaTeX, Python, structured evidence library | ML interatomic potentials, kMC, verification logs, reproducible review workflow |
| **Airflow Academy** *(Private)* | Data orchestration education | Next.js, FastAPI, Supabase, Docker, Airflow | Browser DAG execution, AST validation, isolated sandboxes, SSE logs |
| **Smileprint** *(Private)* | Compliance data platform | FastAPI, PostgreSQL, React, Docker, Caddy | Audit ledger, compliance insights, ESG calculations, PDF lineage |
| **Verified FEM Workbench** *(Private)* | Computational mechanics | Gmsh, Code_Aster, CalculiX, Docker | Review gates, analytical references, cross-solver verification |
| **Parallel Anatomy FEA** *(Private)* | HPC simulation | Gmsh, DOLFINx, UFL, PETSc, MPI, HDF5 | CAD/anatomy import, parallel cases, XDMF/HDF5 output |
| **Quantum ESPRESSO Advisor** *(Private)* | Electronic structure | Fortran, Python, Docker, Quantum ESPRESSO | Empirical benchmark ledger, input/log advisor, reproducible sweeps |
| **Tessera** *(Private)* | Mobile product engineering | Kotlin, Firebase, Room, Voronoi engine | Geometry gameplay, cloud services, privacy controls, monetization |

<details>
<summary><strong>MLIP–KMC Research Review</strong> · LaTeX · Python · Scientific evidence management</summary>

A private research environment for a review of machine-learning interatomic potentials and kinetic Monte Carlo.

- Structured paper library with one record per paper
- Verification status and append-only verification logs
- Evidence-first policy for quantitative claims
- Citation snowballing and exclusion controls
- Reproducible manuscript builds, figures, references, and scanning utilities
- Research scope covering barrier prediction, MLIP surrogates, kMC, and multiscale materials simulation

</details>

<details>
<summary><strong>Airflow Academy</strong> · Next.js · FastAPI · Supabase · Docker · Apache Airflow</summary>

An interactive browser platform for learning and executing Airflow DAGs. The private implementation includes a curriculum of **48 lessons across 7 chapters**.

```mermaid
flowchart LR
    A[Next.js frontend] --> B[Monaco DAG editor]
    A --> C[Lesson interface]
    A --> D[SSE log console]
    B --> E[FastAPI execution API]
    C --> F[(Supabase / PostgreSQL)]
    E --> G[AST validation]
    G --> H[Concurrency-controlled Docker sandbox]
    H --> I[Airflow 2.8.1 runtime]
    I --> D
```

- Custom AST validators for imports, DAG declarations, operators, dependencies, and context usage
- Ephemeral Docker execution with timeout and concurrency controls
- Synchronous and Server-Sent Events execution endpoints
- OAuth authentication and database/filesystem lesson fallback
- Curriculum authoring system for DAGs, ETL, operators, debugging, and TaskFlow
- Automated backend deployment workflow

</details>

<details>
<summary><strong>Smileprint</strong> · FastAPI · PostgreSQL · React · Docker · Compliance analytics</summary>

A private compliance and sustainability platform for Finnish dental clinics.

```mermaid
flowchart LR
    A[Clinic entry / CSV import] --> B[FastAPI API]
    B --> C[(PostgreSQL)]
    C --> D[Append-only revision ledger]
    C --> E[Compliance insight engine]
    C --> F[ESG calculations]
    E --> G[Alerts and metrics]
    F --> H[PDF sustainability reports]
    B --> I[React / Vite frontend]
    J[Caddy + Docker deployment] --> B
```

- SQLAlchemy, Alembic, PostgreSQL, React, Vite, Tailwind, and Caddy
- Append-only audit history and retained revision records
- Checks for waste routing, duplicate invoices, cost spikes, and volume anomalies
- Data-lineage-aware PDF reporting and ESG workflows
- Automated backend and frontend testing

</details>

<details>
<summary><strong>Verified FEM Workbench</strong> · Gmsh · Code_Aster · CalculiX · Physics-based verification</summary>

A solver-neutral finite-element workbench designed around explicit model review and physics-based verification.

```mermaid
flowchart LR
    A[Text / GUI / YAML model] --> B[Validated solver-neutral spec]
    B --> C[Review and approval gate]
    C --> D[Gmsh second-order mesh]
    D --> E[Code_Aster]
    D --> F[CalculiX]
    E --> G[Result parsing]
    F --> H[Result parsing]
    G --> I[Equilibrium and analytical checks]
    H --> I
    I --> J[Node-by-node comparison]
```

- Verified cantilever, plate-with-hole, and elastoplastic-bar examples
- Global equilibrium and analytical reference checks
- Common mesh and nodal comparison across two solvers
- Optional retrieval-assisted repair of failed solver input

</details>

<details>
<summary><strong>Parallel Anatomy FEA Pipeline</strong> · Gmsh · DOLFINx · PETSc · MPI</summary>

A private computational mechanics pipeline for anatomy/CAD geometry import, robust meshing, parallel simulation, and scientific result export.

```mermaid
flowchart LR
    A[STEP / STL geometry] --> B[Healing and classification]
    B --> C[Gmsh mesh generation]
    C --> D[DOLFINx / UFL model]
    D --> E[MPI parallel simulation]
    E --> F[Stress and displacement fields]
    F --> G[HDF5 / XDMF export]
```

- Geometry healing, volume classification, physical groups, and mesh sizing
- DOLFINx, UFL, PETSc, MPI, NumPy, Pandas, and HDF5
- Resumable parameterized cases and visualization-ready XDMF output

</details>

<details>
<summary><strong>Quantum ESPRESSO Advisor</strong> · Fortran · Python · HPC benchmarking</summary>

A private computational-physics toolkit for reproducible Quantum ESPRESSO performance and correctness analysis.

- Fortran source modifications and native builds
- Docker-based development and benchmark environments
- k-point, hybrid-functional, relaxation, and ensemble experiments
- Empirical benchmark ledger with evidence paths
- CLI analysis of Quantum ESPRESSO inputs and logs
- Recommendations constrained to experimentally supported regimes
- Explicit reporting of unverified cases and limitations

</details>

<details>
<summary><strong>Tessera</strong> · Kotlin · Firebase · Room · Voronoi game engine</summary>

A private Android application combining geometry-based puzzle gameplay, authentication, cloud data, local persistence, analytics controls, and monetization services.

- Kotlin Android application architecture with Voronoi-based gameplay
- Firebase Auth, Firestore, Crashlytics, App Check, Analytics, and Remote Config
- Room persistence for preferences, progress, and puzzle data
- Daily puzzle and competition repositories
- Adapty billing integration and privacy/consent controls
- Downloadable music and media playback components

</details>

## Technical Toolkit

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![Apache Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![LAMMPS](https://img.shields.io/badge/LAMMPS-Scientific_Computing-1f6feb?style=for-the-badge)
![VASP](https://img.shields.io/badge/VASP-Computational_Materials-6f42c1?style=for-the-badge)
![MACE / MLIPs](https://img.shields.io/badge/MACE_%2F_MLIPs-Interatomic_Potentials-6f42c1?style=for-the-badge)
![Kinetic Monte Carlo](https://img.shields.io/badge/Kinetic_Monte_Carlo-kMC-6f42c1?style=for-the-badge)
![HPC / Slurm](https://img.shields.io/badge/HPC_%2F_Slurm-Cluster_Computing-2ea44f?style=for-the-badge)
![MPI](https://img.shields.io/badge/MPI-Parallel_Computing-2ea44f?style=for-the-badge)
![Gmsh](https://img.shields.io/badge/Gmsh-Meshing-2ea44f?style=for-the-badge)
![DOLFINx](https://img.shields.io/badge/DOLFINx-FEM-2ea44f?style=for-the-badge)
![Quantum ESPRESSO](https://img.shields.io/badge/Quantum_ESPRESSO-Electronic_Structure-6f42c1?style=for-the-badge)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

## Engineering Principles

- Make data pipelines observable, repeatable, and idempotent.
- Treat scientific claims as evidence that must be traceable and verifiable.
- Validate simulations against physics, not only software exit codes.
- Prefer explicit limitations over unsupported conclusions.
- Keep private work private while communicating architecture and impact clearly.

## Publications

1. **Crystallization dynamics and interfacial structure during HiPIMS growth of thin Nb films on Cu** — *Materials Today Communications* (2026) · Atomistic MD, HiPIMS thin-film deposition, Nb/Cu superconducting RF interfaces · [Search on Google Scholar](https://scholar.google.com/scholar?q=Crystallization+dynamics+and+interfacial+structure+during+HiPIMS+growth+of+thin+Nb+films+on+Cu) · [Add DOI](https://doi.org/)
2. **Surface orientation effects on Cu blistering under high-fluence H ion irradiation** — *Acta Materialia* (2024) · Hydrogen blistering, ion irradiation, Cu surfaces, atomistic modeling · [Search on Google Scholar](https://scholar.google.com/scholar?q=Surface+orientation+effects+on+Cu+blistering+under+high-fluence+H+ion+irradiation) · [Add DOI](https://doi.org/)
3. **Comparative study of Nb film growth on Cu substrates using DCMS and HiPIMS** — *Surface and Coatings Technology* (2024) · Thin-film growth mechanisms, DCMS vs. HiPIMS, energetic deposition · [Search on Google Scholar](https://scholar.google.com/scholar?q=Comparative+study+of+Nb+film+growth+on+Cu+substrates+using+DCMS+and+HiPIMS) · [Add DOI](https://doi.org/)
4. **Notch-tip brittle-ductile transitions in metallic glasses** — *Extreme Mechanics Letters* (2022) · Metallic glasses, fracture mechanics, brittle-to-ductile transition · [Search on Google Scholar](https://scholar.google.com/scholar?q=Notch-tip+brittle-ductile+transitions+in+metallic+glasses) · [Add DOI](https://doi.org/)
5. **Investigation of grain boundary mechanical failure under strain and stress control** — *ECS Journal of Solid State Science and Technology* (2021) · Grain boundary mechanics, failure analysis, atomistic deformation · [Search on Google Scholar](https://scholar.google.com/scholar?q=Investigation+of+grain+boundary+mechanical+failure+under+strain+and+stress+control) · [Add DOI](https://doi.org/)
6. **Thermodynamic potentials and physical quantities of metallic glasses** — *Journal of Non-Crystalline Solids* (2020) · Amorphous alloys, thermodynamics, disordered systems · [Search on Google Scholar](https://scholar.google.com/scholar?q=Thermodynamic+potentials+and+physical+quantities+of+metallic+glasses) · [Add DOI](https://doi.org/)
7. **Short- and medium-range ordering in Cu-Zr and Ni-Zr metallic glasses** — *Journal of Non-Crystalline Solids* (2018) · Cu-Zr / Ni-Zr metallic glasses, structural ordering, polyamorphism · [Search on Google Scholar](https://scholar.google.com/scholar?q=Short-+and+medium-range+ordering+in+Cu-Zr+and+Ni-Zr+metallic+glasses) · [Add DOI](https://doi.org/)

## Contact

- GitHub: [@miladgk](https://github.com/miladgk)
- Portfolio: [miladgk.github.io](https://miladgk.github.io)
- LinkedIn: [Milad Ghaemi](https://www.linkedin.com/in/milad-ghaemikermani/)
- Google Scholar: [Publications](https://scholar.google.com/citations?hl=en&user=dzrQ6WsAAAAJ)
- Collaboration interests: data engineering, scientific machine learning, computational materials science, and computational mechanics.
