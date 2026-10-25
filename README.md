# exteraGram SDK Probe

A one-shot diagnostic plugin that reports exteraGram, Chaquopy, and Telegram runtime class and method details.

**Current version:** 1.0.2  
**Requirements:** exteraGram 12.5.1 or newer; plugin SDK 1.4.4.3 or newer

## Use

1. Install and enable the probe briefly.
2. Long-press a message once. The probe runs on that first long-press and leaves Telegram's native menu handling intact.
3. Read the report at `/sdcard/Download/extera_probe_report.txt` or from logcat, then disable the plugin.

The report omits message text and live chat-object contents, but runtime method details can identify the app build. The scan runs synchronously on the UI thread and may briefly slow the app. Writing to the shared Download path may fail on Android builds with scoped-storage restrictions.
