# RestAPI for Creating QR Codes

## Features

- **QR Code Generation:** Generate QR codes from URLs with customizable colors and sizes.
- **Authentication:** OAuth2 based authentication (username: `admin`, password: `secret`).
- **Static File Serving:** Generated QR codes are stored in a designated directory and served via Nginx.
- **RESTful Endpoints:** Endpoints to create, list, and delete QR code images.
- **Dockerized Deployment:** Run the entire application (FastAPI and Nginx) via Docker Compose.

# Install
1. Clone
2. Make virtual environment:  python3 -m venv venv
3. Activate virtual environment: source venv/bin/activate
4. Install requirements: pip install -r requirements.txt
5. run: mkdir qr_codes to create a qr codes directory to save in.
6. Note: make sure docker is started
7. run pytest locally to check that it works locally
8. Start the app with docker compose up --build
9. Goto http://localhost/docs to view openapi spec documentation
10. Click "authorize" input username: admin password: secret
11. Test making,  retrieving, and deleting QR codes on the spec page.