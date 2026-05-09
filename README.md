#🛢️ Plantova: Automating the Oil & Gas EPC 3D Modeling Supply Chain
"If you want to contribute to automating the entire 3D modeling supply chain for Oil & Gas and Heavy Industrial EPC, come join this project!"

Welcome to Plantova! We are building an open-source, end-to-end pipeline designed to automate the creation, conversion, and intelligence-tagging of 3D engineering models for the Oil & Gas EPC sector.

Our goal is to transform thousands of hours of manual piping routing, structural steel drafting, and point-cloud tracing into a streamlined, programmatic workflow, accelerating the delivery of Digital Twins and As-Built models.

Whether you are an ML Engineer, a BIM Coordinator, a Piping Designer, or a Point Cloud specialist, there is a place for you here.

#🚀 The Vision
In the EPC industry, creating and updating 3D plant models—especially for brownfield projects—is extremely labor-intensive. Plantova aims to build a unified framework that ingests raw site data (Laser Scan Point Clouds, 2D P&IDs, Isometrics) and autonomously extracts, models, and metadata-tags industrial components (pipes, valves, structural steel, equipment) to output intelligent, plant-ready formats (IFC, AVEVA E3D macros, SP3D-compatible data).

#🧩 The Supply Chain Architecture (Where We Need You!)
Our pipeline is modularized to handle the complexities of industrial multi-discipline engineering. We are looking for contributors across these domains:

##1. 📡 Data Ingestion & Scan-to-BIM
What it does: Processes massive LiDAR point clouds (terabytes of data) and 2D engineering drawings (P&IDs, General Arrangements). Cleans, downsamples, and registers scans.

Looking for: Point Cloud specialists, Computer Vision researchers, PyTorch/PointNet++ engineers.

##2. ⚙️ Semantic Segmentation & Feature Extraction
What it does: Uses AI to identify and isolate specific industrial components from point clouds or 2D diagrams. Automatically recognizes pipe routing, flanges, elbows, valves, and standard structural profiles (I-beams, H-columns).

Looking for: AI/ML Engineers, Computational Geometry experts, 3D Object Detection specialists.

##3. 🏗️ Automated 3D Modeling & Routing
What it does: Converts segmented point cloud data into primitive, solid 3D geometry. Automates orthographic pipe routing, clash avoidance, and auto-generates structural framing based on engineering rules.

Looking for: Computational geometry developers, CAD API experts, Piping/Structural Engineers with programming backgrounds.

##4. 🏷️ Metadata Attribution & P&ID Reconciliation
What it does: "Intelligizes" the 3D geometry. Matches modeled components to equipment lists and P&IDs, automatically assigning line numbers, pipe specs, material grades, and tags.

Looking for: Data Engineers, Graph Database developers, EPC Document Control specialists.

##5. 📦 Clash Detection & Industry Export
What it does: Runs automated hard and soft clash detection across disciplines (Piping vs. Electrical vs. Civil). Exports intelligent models into industry-standard open formats (IFC) or proprietary macros for AVEVA E3D, Hexagon Smart3D, and Navisworks.

Looking for: Software Engineers, BIM/VDC Managers, Interoperability (IFC/BIM) specialists.

##🛠️ Tech Stack
Core Logic: Python, C++

Point Cloud Processing: PDAL, Open3D, CloudCompare, PCL (Point Cloud Library)

AI/ML: PyTorch, PointNet++, YOLO (for 2D P&ID extraction)

Geometry & CAD: OpenCASCADE, IfcOpenShell, FreeCAD API

Data Integration: Neo4j (for P&ID to 3D topology mapping), SQL

Target Outputs: IFC 4.0, DWG, NWD, AVEVA PML (Programmable Macro Language)

🤝 How to Contribute
We welcome contributors of all skill levels, especially those blending software engineering with industrial domain knowledge!

Star the repo and join our [Discord / Slack / Discussions] to introduce yourself!

Check out our CONTRIBUTING.md guide for our engineering standards.

Look at the Issues Tab. We have labeled issues specifically for newcomers:

🟢 good first issue - Great for getting familiar with the codebase.

🔵 help wanted - Core extraction and modeling features.

🟡 domain expertise - Requires knowledge of piping specs, ASME standards, or plant design software.

Fork the repository, create your feature branch, and submit a Pull Request.

Quick Start (Local Development)
Bash
# Clone the repository
git clone https://github.com/illuminankit/Plantova.git

# Navigate into the project
cd Plantova

# Install dependencies
pip install -r requirements.txt

# Run the point-cloud to pipe-cylinder test
python main.py --extract-pipes --input ./sample_data/pump_station_scan.las
🗺️ Roadmap
[ ] Phase 1: Point cloud ingestion, cleaning, and basic cylinder/plane extraction.

[ ] Phase 2: AI-driven recognition of standard piping components (flanges, valves, tees).

[ ] Phase 3: 2D P&ID optical character recognition (OCR) and topology mapping.

[ ] Phase 4: Linking 3D components to P&ID metadata and exporting intelligent IFC files.

📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

Let's build the future of automated plant design and industrial digital twins together! 🏭✨
