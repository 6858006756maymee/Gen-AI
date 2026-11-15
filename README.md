# TrendPilot – AI Social Media Trend Predictor

A student prototype of a social media marketing assistant built with Python and Streamlit.

## What it does
- Accepts brand, product, audience, industry, and platform inputs.
- Displays **sample** social media trends with illustrative interest scores.
- Generates a marketing plan, captions, hashtags, and video ideas using Gemini when an API key is configured.
- Provides a clearly labeled template preview without an API key.
- Lets users download recommendations.

**Important:** This prototype does not retrieve live TikTok, Instagram, or YouTube trends. Sample interest scores are fictional and do not demonstrate predictive accuracy. The dashboard is not evidence of real-world audience behavior.

## Run locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Enable Gemini
Get an API key from Google AI Studio. Set an environment variable `GEMINI_API_KEY`, or create a local `.streamlit/secrets.toml` file with:

```toml
GEMINI_API_KEY = "your-key-here"
```

Never commit your API key to GitHub. On Streamlit Community Cloud, configure it in the app's Secrets settings.

## Deploy
1. Upload these files to a GitHub repository (put `app.py` and `requirements.txt` at the repository root, or specify the correct path when deploying).
2. Visit https://share.streamlit.io/ and select **Create app**.
3. Choose your GitHub repository, branch, and main file path (for a `TrendPilot` folder, use `TrendPilot/app.py`).
4. Deploy. Add `GEMINI_API_KEY` in Streamlit app settings if you want live AI generation.

## Suggested demo
Enter **Glow Studio**, **Skincare serum**, **Students and young adults**, choose **Beauty**, and click **Generate my marketing plan**. Explain the difference between the sample dashboard and Gemini-generated content.
