# FinkiRasporedi

A unified platform for managing, processing, and visualizing academic schedules, built for the needs of FINKI (Faculty of Computer Science and Engineering). This project leverages multiple technologies to provide backend, frontend, data processing, and infrastructure automation.

## 📄 Documentation

- [Project Documentation (Google Doc)](https://docs.google.com/document/d/17Awdmi8-Q2PrmQs-Ad9VzF8es_htYnCphQrrHB2ceFc/edit?usp=sharing)
- [Kubernetes Infrastructure Repository](https://github.com/nnikolovskiii/kubernetes)

## 🎬 Demo

[![Demo Video](https://img.youtube.com/vi/piJBrjdLod8/1.jpg)](https://youtu.be/piJBrjdLod8)

## 🚀 Features

- Data loading and transformation for academic schedules
- Backend services for schedule management (likely .NET Core)
- Interactive frontend (Flutter app)
- Containerized deployment with Docker Compose
- Infrastructure as code with Kubernetes and AWS scripts
- Sample data and UML diagrams for architecture/reference

## 🗂️ Project Structure

```
.
├── DataLoader/                # Scripts and tools for importing/processing schedule data
├── dotnet/                    # Backend API and microservices (likely .NET Core)
├── flutter/                   # Flutter mobile app for user interaction
├── aws-infra/                 # AWS Infrastructure as Code (IaC) scripts/configs
├── mysql-init/                # MySQL initialization scripts
├── docker-compose.yml         # Main Docker Compose file (full stack)
├── docker-compose-backend.yaml
├── docker-compose-ngrok.yaml
├── Calendar_data_loader.ipynb # Jupyter notebook for data manipulation
├── output_file.csv            # Example output data
├── use_case_uml_diagram.png   # UML diagram (use case)
├── Idea.gif, Innovation.mp4   # Visuals and presentations
└── ...
```

## 🛠️ Technologies Used

- **.NET Core**: Backend services (located in `/dotnet`)
- **Flutter**: Cross-platform frontend app (`/flutter`)
- **Python**: Data processing (e.g., notebooks, scripts)
- **Docker & Docker Compose**: Containerization and orchestration
- **Kubernetes**: Production-grade infrastructure (see [kubernetes repo](https://github.com/nnikolovskiii/kubernetes))
- **AWS**: Cloud infrastructure (`/aws-infra`)
- **MySQL**: Relational database

## ⚡ Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/nnikolovskiii/FinkiRasporedi.git
   cd FinkiRasporedi
   ```

2. **Run with Docker Compose (all services)**
   ```bash
   docker-compose up --build
   ```
   - For backend only: `docker-compose -f docker-compose-backend.yaml up`
   - For ngrok tunneling: `docker-compose -f docker-compose-ngrok.yaml up`

3. **Data Loading**
   - Use scripts in `DataLoader/` or the Jupyter notebook (`Calendar_data_loader.ipynb`) for initial data setup.

4. **Flutter Frontend**
   - See [`flutter/README.md`](flutter/README.md) for instructions on running the Flutter app.

5. **Database Initialization**
   - MySQL initialization scripts are located in `/mysql-init`.

## 📦 Deployment

- For Kubernetes deployment, refer to the [kubernetes repo](https://github.com/nnikolovskiii/kubernetes).
- AWS scripts are in `/aws-infra`.

## 📷 Visuals & Diagrams

- ![UML Diagram](use_case_uml_diagram.png)
- ![Idea Gif](Idea.gif)
- [Demo Video](https://youtu.be/piJBrjdLod8)
- Innovation presentation: `Innovation.mp4`

## 🤝 Contributing

Contributions, issues and feature requests are welcome! Please open an issue first to discuss what you would like to change.

## 📜 License

Specify your license here (MIT, Apache 2.0, etc.).

---

> _This README was generated with the help of GitHub Copilot. For more details, see the project documentation or contact the repository owner._
