1. Install uv package manager for Python -> [uv-package-manager](https://github.com/astral-sh/uv)
2. Setup python project:
		a. uv init
		b. uv venv
3. Create requirements.txt file with required packages:
		- langchain
		- langchain_community
		- langchain-openai
		- langchain-groq
		- python-dotenv
		- langchain-google-genai
4. Install packages using uv: 
		a. uv add -r requirements.txt
5. Add .env file with following variables:
		a. OPENAI_API_KEY
		b. GROQ_API_KEY
		c. GOOGLE_API_KEY
6. Install ipykernel -> `uv add ipykernel`.