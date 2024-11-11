Prometheus and Grafana Setup with Custom Exporters

This repository demonstrates the setup of a monitoring solution using Prometheus and Grafana, following this tutorial. The project is extended with additional exporters to collect both system and container metrics.
Features

    Prometheus: Used for scraping and storing metrics.
    Grafana: Provides a user-friendly dashboard to visualize metrics.
    Node Exporter: Collects hardware and OS metrics from the host machine.
    cAdvisor: Monitors Docker containers, providing metrics such as CPU, memory, and network usage.
    Pre-configured Grafana Dashboards: Includes dashboards for both system and container metrics.

Project Structure

    docker-compose.yml: Defines services for Prometheus, Grafana, Node Exporter, and cAdvisor.
    prometheus.yml: Configuration file for Prometheus, including targets for scraping metrics from both Node Exporter and cAdvisor.
    grafana-provisioning/: Contains the pre-configured Grafana dashboards.

How to Run

    Clone this repository:

git clone https://github.com/jovan99djokic/Devolution_project
cd Devolution_project

Start all services with Docker Compose:

    docker-compose up -d

    Access the services:

        Grafana: http://localhost:3000

        Prometheus: http://localhost:9090

        Note: If you encounter issues using Chrome, try accessing Grafana with Firefox.

    Explore the following dashboards in Grafana:
        System Metrics: Visualize hardware and OS performance.
        Container Metrics: Monitor Docker container resource usage.

Additional Notes

    The Node Exporter and cAdvisor run as Docker containers, simplifying the deployment process.
    The Grafana dashboards were sourced from the community and customized for this setup.

Screenshots

(Include screenshots of the Grafana dashboards here for better visualization.)
License

This project is open-source and available under the MIT License.
