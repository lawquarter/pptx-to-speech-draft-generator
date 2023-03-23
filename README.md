# PowerPoint to Draft Speech Converter

This application uses Streamlit, OpenAI, and python-pptx to convert a PowerPoint file into a draft speech. It leverages the power of GPT-4 to generate a captivating speech based on the contents of the uploaded PowerPoint file.

## Requirements
To install the required packages, run: 
```pip install requirements.txt```

## Usage

1. Set the OpenAI API key as an environment variable:

- On Linux or macOS:
```
export OPENAI_API_KEY="your-api-key"
```

- On Windows:
```
setx OPENAI_API_KEY "your-api-key"
```

2. Run the Streamlit app:
```
streamlit run app.py
```

3. Open the provided URL in your browser to use the application.
4. Upload a PowerPoint file with less than 4000 words, and the application will generate a draft speech based on the contents of the file.

## Functions

- get_gpt4_response(system_prompt, user_prompt): Returns a GPT-4-generated response based on the given system and user prompts.
- extract_pptx_text(pptx_file): Extracts text from the provided PowerPoint file.

## Application Interface

The application has a simple interface:

1. A title and brief description of the app.
2. A warning about the maximum word count for the uploaded PowerPoint file.
3. A file uploader to select and upload a PowerPoint file.
4. Output that you can copy
