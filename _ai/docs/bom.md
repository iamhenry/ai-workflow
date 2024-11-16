# Bill of Materials (BOM)
This BOM provides a roadmap for the core functionality and technical foundation needed for your macOS voice-to-text app MVP.

---

### 1. Components
#### Core Features
- Voice-to-Text Transcription:
  - Speech recognition for transcribing audio to text.
- Clipboard Integration:
  - Copying transcribed text to the clipboard.
- Text Field Injection:
  - Automatic insertion of transcribed text into the active app's text input field.
- Recording Visual Feedback:
  - Animated "pill" to indicate active recording.
- Keyboard Shortcuts:
  - Trigger transcription and cancel recording via hotkeys.
- Model Management:
  - Download, switch, and delete Whisper models (small, medium, large).

#### Supporting Features
- Settings Interface:
  - Manage and configure models and app behavior.
- Privacy Options:
  - Local processing using Whisper models for enhanced privacy.

---

### 2. Technical Stack
#### Frontend
- Language: Swift (for native macOS app development).
- Framework: SwiftUI (for UI design).

#### Backend/Logic
- Speech-to-Text Model: OpenAI’s Whisper/Whisper Turbo.
- Audio Processing: AVFoundation (Apple framework for audio recording and processing).
- Model Integration: WhisperKit for embedding and using Whisper models locally.

#### Utilities
- Clipboard Management: NSPasteboard (native macOS clipboard API).
- Text Injection: Accessibility APIs (e.g., AXUIElement for targeting text input fields).
- Keyboard Shortcuts: Combine framework or global keyboard hook using Carbon or AppKit.

---

### 3. Dependencies
#### Core Libraries
- WhisperKit: To load and utilize Whisper models.
- AVFoundation: For recording audio and handling microphone input.
- Accessibility APIs: For text injection into other applications.

#### Third-party Dependencies
- Swift Package Manager (SPM): For dependency management.
- Whisper Models (Small, Medium, Large): Downloadable via a settings interface.

---

### 4. Functional Requirements
#### MVP Core Functionalities
1. Voice Recording:
   - Record user audio via the computer's microphone.
   - Show a recording indicator (animated pill).
2. Speech-to-Text:
   - Use a selected Whisper model to transcribe the recorded audio to text.
3. Clipboard Handling:
   - Allow users to copy transcribed text to the clipboard.
4. Text Injection:
   - Insert transcribed text into the currently active text input field.
5. Keyboard Shortcuts:
   - Start/stop recording and cancel via configurable shortcuts.
6. Model Management:
   - Download, delete, and switch between Whisper models in the app settings.

#### Secondary Features
1. Settings Panel:
   - Manage Whisper model configurations and app behavior.
2. Local Processing:
   - Ensure models run locally for privacy.
3. Recording Cancellation:
   - Abort active recording with a keyboard shortcut.

---

