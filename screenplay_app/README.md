# Screenplay Writer App

A professional screenplay writing application with Google authentication and project management.

## Features

- ✨ **AI-Powered Writing**: Continue your screenplay with AI assistance (OpenAI GPT-3.5)
- 💾 **Auto-Save**: Projects automatically save as you type
- 🎨 **Light/Dark Mode**: Toggle between light and dark themes
- 📱 **Responsive Design**: Works on all devices
- 🎬 **Professional Formatting**: Industry-standard screenplay formatting
- 👥 **Character Tracking**: Automatically tracks characters and scenes
- ⌨️ **Smart Type Menu**: Press Enter to choose element type (like Final Draft)
- 🔐 **Google Sign-In**: Secure authentication with Google account

## Getting Started

### Quick Start

1. Open `index.html` in your web browser
2. Click "Continue without signing in (demo mode)" for instant access
3. Or sign in with your Google account for full functionality

### File Structure

- `index.html` - Sign-in page with Google OAuth
- `projects.html` - Projects dashboard showing all your screenplays
- `editor.html` - The screenplay editor with all writing tools

## How to Use

### Creating a Project

1. After signing in, click "New Project" on the projects dashboard
2. Enter a project name and click "Create"
3. You'll be taken to the editor automatically

### Writing Your Screenplay

#### Formatting Tools

- **Scene** - Dropdown with INT. (Interior) or EXT. (Exterior) options
- **Transition** - Dropdown with 13 standard transitions (CUT TO:, FADE IN:, etc.)
- **Character** - Adds character name with proper indentation
- **Parenthetical** - Adds parenthetical direction for dialogue
- **AI Continue** - Generate screenplay content with AI
- **Save** - Download screenplay as .txt file

#### SmartType Menu

Press **Enter** on a blank line to show the SmartType menu:
- Scene Heading
- Action
- Character
- Dialogue
- Parenthetical
- Transition

Use arrow keys to select, Enter/Tab to apply, Escape to cancel.

#### Auto-Indent

After typing a character name in ALL CAPS, pressing Enter will automatically indent for dialogue.

#### Keyboard Shortcuts

- **Cmd/Ctrl + S** - Save screenplay as .txt file

### Project Management

- **Open** - Open a project to continue writing
- **Duplicate** - Create a copy of a project
- **Delete** - Remove a project (with confirmation)

Projects show:
- Creation date
- Last modified date
- Word count

### AI Continue Feature

1. Click "✨ AI Continue" button
2. Enter a prompt for what should happen next
3. AI will generate screenplay content in proper format

**Note**: You'll need an OpenAI API key for AI features. Get one at https://platform.openai.com/api-keys

## Google Sign-In Setup

To enable Google Sign-In:

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select existing one
3. Enable Google Identity Services API
4. Create OAuth 2.0 credentials
5. Add authorized JavaScript origins (your domain)
6. Copy the Client ID
7. In `index.html`, replace `YOUR_GOOGLE_CLIENT_ID` with your actual Client ID (line 164)

## Technology Stack

- **Frontend**: HTML, CSS, JavaScript (Vanilla JS)
- **Authentication**: Google Identity Services
- **Storage**: localStorage (client-side)
- **AI**: OpenAI GPT-3.5 Turbo API
- **Design**: Custom CSS with light/dark mode support

## Browser Compatibility

Works on all modern browsers:
- Chrome/Edge (recommended)
- Firefox
- Safari

## Data Storage

Projects are stored in browser localStorage:
- No backend server required
- Data persists across sessions
- Stored locally on your device
- Export your work as .txt files for backup

## Formatting Standards

Based on **The Black List** screenplay formatting:
- Scene headings: `INT./EXT. LOCATION - DAY/NIGHT`
- Character names: ALL CAPS, centered (24 spaces indent)
- Dialogue: 10 spaces indent
- Parentheticals: 20 spaces indent, in (parentheses)
- Transitions: Right-aligned (48 spaces)
- Present tense only
- No camera directions

## Tips

1. **Save Regularly**: While auto-save is active, use Cmd/Ctrl+S to download backups
2. **Use Demo Mode**: Try it out without Google sign-in
3. **Dark Mode**: Toggle with 🌓 button in top right
4. **SmartType**: Use Enter key for quick formatting
5. **AI Prompts**: Be specific for better AI-generated content

## Support

For issues or questions, check the sidebar for:
- **SCENES** - Click to jump to any scene
- **CHARACTERS** - See all characters in your screenplay
- **Refresh** - Update the lists manually

## License

Part of the script_buddy_v2 project.
