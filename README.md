# Smart App to Help Seniors API

A Django API prototype for age-friendly application scenarios. It provides backend endpoints for image understanding, text and voice interaction, and Q&A flows through cloud-based vision, translation, speech, and language-question-answering capabilities.

## Feature Scope

- Image analysis.
- Text-to-speech.
- Speech-to-text.
- Text-based Q&A.
- Voice-based Q&A.

## Technology Stack

- Django 4.1
- Cloud computer-vision service
- Cloud translation service
- Cloud speech service
- Cloud language Q&A service

## Local Run

1. Create a Python virtual environment.
2. Install dependencies:

    pip install -r requirements.txt

3. Provide your own cloud-service endpoints and credentials through local environment configuration.
4. Apply migrations and start the development server:

    python manage.py migrate
    python manage.py runserver

Endpoint paths are defined by the project root routes, `cv/urls.py`, and `speech/urls.py`.

## Privacy and Production Requirements

Image, voice, and Q&A requests may contain personal or sensitive information. Before deployment, add at least:

- HTTPS, authentication, authorization, and access logging;
- Request-size, file-type, and rate limits;
- Key rotation and security review;
- Consent, data minimization, and deletion policies for uploaded content;
- Error handling and availability plans for cloud-service failures.

This project is an API prototype, not a production age-friendly service or a medical-advice system.

## License

See the repository's LICENSE file.