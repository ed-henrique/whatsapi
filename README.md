# WhatsAPI

Containerized API to send messages through Whatsapp.

## Goals

1. To create an easily self-hostable Whatsapp API;
2. To prioritize developer experience;

## Tech Stack

- Go (API)
- Docker (Container Engine)
- Puppeteer and JavaScript (Whatsapp Interaction)

## Features

- [ ] Connect
- [ ] Disconnect
- [ ] Send Message

## Roadmap

- Connect to Whatsapp
  - Access [Whatsapp Web](https://web.whatsapp.com)
  - Read QR Code
  - Print QR Code on screen, so that the user can read it (idk if there is a better way to connect yet)
  - Keep the browser instance running, maintaining the connection
- Disconnect from Whatsapp
  - If connected
    - Click on the three dots icon
    - Click `Disconnect`
    - Wait for the request to go through
  - If not connected
    - Do nothing
- Send Message
  - If connected
    - Click on the search bar
    - Search for the contact number
    - If there are results
      - Click on the user
      - Click on the message field
      - Type the message
      - Press `ENTER`
      - Wait for single check or double check icons
      - Repeat for all contacts
    - If there are no results
      - Throw error
  - If not connected
    - Throw error
