# Emby Merge Versions

## Introduction

The Emby Webhook Automation is a Python script that serves as a webhook listener for the Emby media server. It's designed to automate the merging of movies in your Emby library based on provider IDs received through webhooks.

## Features

- Automatically merge two movies in the Emby library based on matching provider IDs.
- Supports multiple `ProviderIds` for searching movies.
- Logs the merge results, including successful and unsuccessful merges.

## Prerequisites

Before using this script, ensure you have the following:

- Python 3.x installed
- Required Python libraries: Flask, requests
- Docker (optional, for Docker installation)

## Installation

### Traditional Installation

1. Clone the repository.
2. Install the requirements using `pip install -r requirements.txt`.
3. Set up your environment variables.
4. Run the application using `python3 main.py`.

### Docker Installation

If you have Docker and Docker Compose installed, you can use the provided `docker-compose.yml`

1. Set up your environment variables in a `.env` file.
2. Run `docker-compose up`.

## Usage

### Setting up Emby Webhook

1. Go to Emby settings.
2. Choose `Webhook` and add a new webhook.
3. Set the url to (e.g., `http://192.168.1.1:5000/emby-webhook`).
4. Select `libary new media added`.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests for new features, bug fixes, or improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
