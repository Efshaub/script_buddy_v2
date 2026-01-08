# AI Screenplay Generator Setup Guide

The aiscreenplay submodule has been configured and improved for easy use.

## Quick Start

1. **Navigate to the aiscreenplay directory:**
   ```bash
   cd aiscreenplay
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set your OpenAI API key:**
   ```bash
   export OPENAI_API_KEY='your-api-key-here'
   ```

   Get your API key from: https://platform.openai.com/api-keys

4. **Run the app:**
   ```bash
   ./run.sh
   ```

   The app will open at http://localhost:8501

## Improvements Made

- ✅ Updated to use environment variables for API key (more secure)
- ✅ Modernized to use OpenAI ChatCompletion API (gpt-3.5-turbo)
- ✅ Added error handling and user-friendly messages
- ✅ Created requirements.txt for easy dependency management
- ✅ Added run.sh script for simplified startup
- ✅ Improved README with clearer instructions

## How to Use

Once the app is running:

1. Fill out the scene template with your screenplay details:
   - Location (e.g., "Coffee shop - interior")
   - Time of day (e.g., "Morning")
   - Characters (e.g., "JOHN, 30s, detective")
   - Objective (what should happen)
   - Conflict (obstacles characters face)
   - Key dialogue
   - Important actions
   - Emotional tone
   - Additional notes

2. Adjust optional parameters:
   - **Temperature**: Controls creativity (0.0-1.0, default 0.7)
   - **P-Value**: Controls diversity (0.0-1.0, default 0.9)

3. Click "Generate Screenplay"

4. Copy the generated screenplay to your preferred screenwriting software

## Note

The improvements are stored locally in the submodule. If you want to keep them permanently, consider forking the original repository to your own GitHub account.
