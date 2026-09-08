# Kerkenez Ecosystem

High-performance, platform-native Windows utilities engineered for zero bloat, mechanical sympathy, and absolute local privacy.

---

### Engineering Principles

* **Platform-Native by Design:** Built exclusively for the Windows NT ecosystem using modern C# / .NET. We do not wrap websites in headless browsers or ship 200 MB of webview runtimes for a tray icon.
* **Local-First & Offline:** Your credentials, configurations, and data never touch our servers, or not that we have a server. Sensitive storage uses Windows DPAPI encryption directly on your machine.
* **System Resource Efficiency:** Background daemons idle in kilobytes, not gigabytes. If an asset exists inside a native Windows binary (like `wpdshext.dll`), we use it rather than bundling duplicate bloat.
* **Single-File Portability:** Software is distributed as clean, self-contained executables. Extract, run, and get to work—no complex dependency webs or fragile runtimes required.

---

### The Suite

| Project | Description | Status |
| :--- | :--- | :--- |
| **KerkenezMail** | Native, ultra-lightweight background email notifier and summarizer. | Active |
| **KerkenezCalendar** | Fast, local desktop calendar with sync from mail accounts and agenda planner. | Open Beta |
| **KerkenezNews** | Track the news feeds you want with 0 telemetry, with optional quick summarization. | Open Beta |
| **KerkenezSpeech** | A Local lightweight speech to text system tray tool with diffrent models option and sub mb idle working set goal. | Open Beta |
| **KerkenezVoice** | Lightweight UI and managment board for Kokoro with advanced tooling. | Open Beta |
| **KerkenezTicket** | Local, Single computer ticket management program for solo developers that wants to organize their project tickets. | Planning |
| **KerkenezRazer** | Low-overhead native battery telemetry daemon for Razer wireless gear. | Open Beta |

---

### Contributing Device Telemetry (`KerkenezRazer`)

Want your Razer wireless hardware supported without running Synapse? Help us map the USB HID reports:

1. Capture a clean Wireshark / USBPcap trace filtered on `usb.idVendor == 0x1532` while launching Synapse once to let it query battery levels.
2. Export the capture as a `.pcapng` file.
3. Open an issue with your exact hardware model name, firmware version, and the attached capture.

---

> *"Build for the OS. Don't shape the OS around your app."*
