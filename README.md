# Real-Time AI Voice Agent - by Khadija HIMRI

## 1. Project Overview

This project is an implementation of a real-time AI voice agent using the **LiveKit Agents framework for Python**. It serves as a robust foundation for building sophisticated AI agents capable of processing live audio streams with minimal latency.

The agent is configured to connect to a LiveKit room, listen to a participant's audio, and can be extended to process and respond to it, demonstrating the core functionality of a real-time media pipeline.

## 2. Key Features

-   **Real-Time Audio Processing**: Built on the LiveKit framework to handle live audio streams efficiently.
-   **Extensible Agent Framework**: Uses `livekit-agents` to create a `Worker` that is easily extendable for more complex tasks like transcription, language model interaction, and text-to-speech.
-   **Cloud-Based Configuration**: Connects securely to a LiveKit Cloud room using API keys for robust and scalable communication.

## 3. Setup and Usage (Windows)

### Prerequisites
- Python 3.9+
- A LiveKit Cloud account to get API keys.

### Installation
1.  Clone this repository.
2.  Navigate into the project directory:
    ```bash
    cd RealTime-AI-Voice-Agent
    ```
3.  Create and activate a Python virtual environment:
    ```bash
    python -m venv .venv
    .venv\Scripts\activate
    ```
4.  Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Agent
1.  Set your LiveKit credentials in the terminal:
    ```bash
    set LIVEKIT_API_KEY=YOUR_API_KEY
    set LIVEKIT_API_SECRET=YOUR_API_SECRET
    set LIVEKIT_URL=YOUR_LIVEKIT_URL
    ```
2.  Launch the agent:
    ```bash
    python -m src.agent
    ```