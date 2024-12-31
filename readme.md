# Audio to SRT Transcriber

This Python application transcribes audio files (WAV or MP3) into subtitle files (.SRT) using OpenAI's Whisper model. The generated SRT files can be easily accessed and opened through a simple graphical user interface (GUI).

## Requirements:
- Python 3.x
- `whisper` (for transcription)

## Installation:
1. Download or clone this repository.
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
   
## Usage:
1. Run the script:
    ```bash
    python main.py
    ```

2. Select the audio files (WAV or MP3) using the **Browse** button.

3. Click **Transcribe** to generate SRT files. The results will appear in the list below.

4. Double-click any SRT file in the list to open it with the default text editor.

## Output:
- The transcribed subtitle files are saved in an "output" directory.

## Package to an executable:

```bash
pip install pyinstaller
```

Make sure pyinstaller is in your PATH

```bash
pyinstaller --onefile --noconsole --add-data "<path-to-whisper-package>;whisper/" .\main.py
```

Check pyinstaller docs for more details