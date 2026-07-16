# SmartAppToHelpSeniorsAPI

An educational API and AI-assistance project built around Azure AI services to help older adults interact with digital services.

## Project focus

The project explores accessible interaction patterns and AI-backed services, including speech and language capabilities exposed through a web API.

## Architecture

- API layer: request validation, authentication boundaries, and response formatting
- AI integration layer: Azure service clients and prompt/request orchestration
- application layer: user-facing assistance workflows
- configuration layer: environment variables for service endpoints and keys

## Local development

Create an isolated Python environment, install the repository dependencies, and configure Azure service credentials through environment variables. Never commit keys or real user data.

~~~bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
pip install -r requirements.txt
~~~

Run the web service using the entry point documented in the source tree, then inspect the API schema before integrating a client.

## Accessibility and safety

Use readable error messages, conservative defaults, and human review for AI-generated responses. Do not treat generated content as medical, legal, or financial advice.

## License

See the repository license file for redistribution terms.