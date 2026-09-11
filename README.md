# Uptime Kuma Documentation Project

An independent technical documentation project for [Uptime Kuma](https://github.com/louislam/uptime-kuma), an open-source, self-hosted monitoring tool.

This project documents a practical beginner workflow for installing Uptime Kuma, monitoring an HTTP endpoint, interpreting monitoring results, configuring Telegram alerts, and creating a status page.

The documentation was developed through hands-on product testing with Uptime Kuma running locally in Docker.

> [!NOTE]
> This is an independent portfolio project and is not official Uptime Kuma documentation.

## Documentation

### Getting started

- [Install Uptime Kuma with Docker Compose](docs/install-uptime-kuma.md)

### Monitoring

- [Create Your First HTTP Monitor](docs/create-http-monitor.md)
- [Understand Monitor Status and Results](docs/monitor-status-and-results.md)

### Notifications

- [Configure Telegram Notifications](docs/configure-telegram-notifications.md)

### Status pages

- [Create a Status Page](docs/create-status-page.md)

## Documentation journey

The documentation follows a beginner workflow from installation to communicating service availability:

```text
Install Uptime Kuma
        ↓
Create an HTTP monitor
        ↓
Understand monitoring results
        ↓
Configure Telegram notifications
        ↓
Create a status page
```

## What I tested

The procedures and examples were developed against a local Uptime Kuma installation rather than from product documentation alone.

Testing included:

- Installing Uptime Kuma with Docker Compose.
- Configuring SQLite during initial setup.
- Creating and running an HTTP monitor.
- Triggering a controlled DNS resolution failure.
- Observing Down and recovery states.
- Pausing and resuming a monitor.
- Configuring Telegram as a notification provider.
- Receiving test, Down, repeated Down, and recovery notifications.
- Creating a status page and publishing monitor information.

The controlled failure test uses the reserved `.example` domain rather than depending on a real website being unavailable.

## Tested environment

| Component | Environment |
| --- | --- |
| Uptime Kuma | 2.x |
| Operating system | Windows 11 |
| Container platform | Docker Desktop |
| Container configuration | Docker Compose |
| Terminal | PowerShell |
| Database | SQLite |
| Notification provider | Telegram |

## Documentation approach

This project focuses on task-oriented documentation for users who are new to Uptime Kuma.

The documentation is designed to:

- Give each guide a clear user outcome.
- Provide tested procedures and expected results.
- Separate procedural instructions from conceptual explanations.
- Explain errors in the context in which they occur.
- Use screenshots when they help readers navigate or verify the interface.
- Distinguish observed product behavior from assumptions.
- Protect sensitive information such as passwords and API tokens.

## Docs-as-Code workflow

Documentation changes are managed through Git and GitHub using a pull-request workflow.

GitHub Actions automatically checks documentation changes for:

- Markdown quality and consistency.
- Broken links.

Security checks also help detect accidentally committed secrets.

This workflow provides automated quality checks before documentation changes are merged into `main`.

## Repository structure

```text
uptime-kuma-docs/
├── .github/
│   └── workflows/
│       └── docs-quality.yml
├── docs/
│   ├── install-uptime-kuma.md
│   ├── create-http-monitor.md
│   ├── monitor-status-and-results.md
│   ├── configure-telegram-notifications.md
│   └── create-status-page.md
├── images/
├── .gitignore
├── .markdownlint.json
└── README.md
```

## Skills demonstrated

This project demonstrates practical experience with:

- Technical writing
- User and procedural documentation
- Information architecture
- Product investigation and testing
- Markdown
- Git and GitHub
- Docs-as-Code
- Pull requests and documentation review
- GitHub Actions
- Markdown linting
- Automated link checking
- Docker and Docker Compose
- Technical troubleshooting

## Disclaimer

This project is an independent documentation sample created for learning and portfolio purposes.

Uptime Kuma is an open-source project maintained by its respective contributors. Refer to the [official Uptime Kuma repository](https://github.com/louislam/uptime-kuma) for official documentation, releases, and product information.
