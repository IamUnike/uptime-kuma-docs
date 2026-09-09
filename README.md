# Uptime Kuma Documentation Project

An independent technical documentation project for [Uptime Kuma](https://github.com/louislam/uptime-kuma), an open-source, self-hosted monitoring tool.

This project documents a practical beginner workflow for installing Uptime Kuma, monitoring an HTTP endpoint, interpreting monitoring results, configuring Telegram alerts, and publishing a status page.

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

## What this project covers

The documentation follows a beginner workflow from installation to basic monitoring:

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

The examples include both successful and failed monitoring scenarios. A deliberately invalid `.example` domain is used to demonstrate DNS failure behavior without depending on a real website being unavailable.

## Tested environment

The documentation was developed and tested using:

- Uptime Kuma 2.x
- Docker Desktop
- Docker Compose
- Windows 11
- PowerShell
- SQLite for the initial Uptime Kuma setup
- Telegram for notification testing

## Repository structure

```text
uptime-kuma-docs/
├── docs/
│   ├── install-uptime-kuma.md
│   ├── create-http-monitor.md
│   ├── understand-monitor-results.md
│   ├── configure-telegram-notifications.md
│   └── create-status-page.md
│
├── images/
│   └── ...
│
└── README.md
```

The `docs` directory contains the documentation set. The `images` directory contains screenshots captured during product testing.

## Testing approach

The procedures and examples in this project were tested against a local Uptime Kuma installation.

Testing included:

- Installing and starting Uptime Kuma with Docker Compose.
- Creating a working HTTP monitor.
- Triggering a controlled DNS resolution failure.
- Observing Down and recovery states.
- Configuring a Telegram bot as a notification provider.
- Receiving test, Down, repeated Down, and recovery notifications.
- Pausing and resuming a monitor.
- Creating a status page and adding a monitor to it.

Sensitive information such as administrator passwords and Telegram bot tokens is excluded from the repository.

## Documentation approach

The project focuses on task-oriented documentation for users who are new to Uptime Kuma.

The documentation aims to:

- Give readers a clear outcome for each guide.
- Provide tested commands and procedures.
- Explain expected results after important steps.
- Distinguish product observations from assumptions.
- Use screenshots only when they help readers navigate or verify the interface.
- Explain errors in the context in which they occur.
- Keep security-sensitive information out of examples and screenshots.

## Disclaimer

This project is an independent documentation sample created for learning and portfolio purposes.

Uptime Kuma is an open-source project maintained by its respective contributors. For official product information, releases, and documentation, refer to the [Uptime Kuma GitHub repository](https://github.com/louislam/uptime-kuma) and its official documentation.
