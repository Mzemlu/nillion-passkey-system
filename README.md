# nillion-passkey-system

# WebAuthn Ed25519 Example

This project demonstrates how to use WebAuthn with Ed25519 key pairs for secure authentication.

## Prerequisites

- Python 3.8+
- Node.js (for frontend development)
- Flask
- SQLAlchemy

## Setup

### Backend

1. Navigate to the `backend` directory:
    ```bash
    cd backend
    ```

2. Install the necessary Python packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Initialize the database:
    ```bash
    python database.py
    ```

4. Run the Flask server:
    ```bash
    python app.py
    ```

### Frontend

1. Open `frontend/index.html` in your browser.

## Usage

- **Register**: Creates a new Ed25519 key pair on the user's device and sends the public key to the server.
- **Authenticate**: Signs a challenge with the private key stored on the user's device and sends it to the server for verification.

## Trusted Parties

In this implementation, the trusted parties are the authenticator (user's device) and the user's browser. The private key never leaves the authenticator and is used only for signing authentication challenges.

## Demo Video

[Insert demo video link here]

## License

This project is licensed under the MIT License.
