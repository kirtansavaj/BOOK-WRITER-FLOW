# Book Writer flow using DeepMind's Gemma 3, CrewAI and BrightData

This project implements an automated book writing system using AI agents.
- [Bright Data](https://brdta.com/dailydoseofds) is used to scrape YouTube videos.
- CrewAI to build the Agentic workflow.
- Google DeepMind's latest Gemma 3 as the LLM.


---
## Setup and installations

**Get BrightData API Key**:
- Go to [Bright Data](https://brdta.com/dailydoseofds) and sign up for an account.
- Select "Proxies & Scraping" and create a new "SERP API"
- Select "Native proxy-based access"
- You will find your username and password there.
- Store it in the .env file of the src/ folder (after renaming .env.example to .env).


```
BRIGHDATA_USERNAME="..."
BRIGHDATA_PASSWORD="..."
```

**Setup Ollama**:
   ```bash
   # setup ollama on linux 
   curl -fsSL https://ollama.com/install.sh | sh
   # pull gemma3 model
   ollama pull gemma3:4b 
   ```


**Install Dependencies**:
   Ensure you have Python 3.11 or later installed.
   ```bash
   pip install ollama crewai crewai-tools
   ```

---

## Run the project

Finally, head over to this folder:
```
cd book_flow/book_writing_flow/src
```

and run the project by running the following command:

```bash
python book_writing_flow/main.py
```

AUTHOR - KIRTAN SAVAJ
(AI/BACKEND DEVELOPER)
