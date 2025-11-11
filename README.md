# rag_medical_ai
**Prerequisites:**

- Python 3.9+
- A Google Gemini API Key

**Step 1: Setup Environment**
Clone this repository and navigate into it. Then, create and activate a virtual environment:

```
python3 -m venv venv
source venv/bin/activate

```

**Step 2: Install All Dependencies**
Install all required packages in one command using the `requirements.txt` file:

```
pip install -r requirements.txt

```

**Step 3: Add API Key**
Create a file named `.env` in the project root. Add your Google API key to it:

```
GOOGLE_API_KEY=YOUR_API_KEY_HERE

```

**Step 4: (Optional) Create Initial Database**
If you have a folder of PDFs you want to pre-load, place them in the `./documents` folder. Then, run the `ingest_advanced.py` script *once*:

```
python ingest_advanced.py

```

*(You can also skip this and build your database live via the app's uploader.)*

**Step 5: Run the Advanced App**
Launch the Streamlit application:

```
streamlit run app_advanced.py

```

Your browser will open to `http://localhost:8501`. You can now chat with your documents and upload new ones via the sidebar.
