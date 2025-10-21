# AIDA64‑Preview

[![C++](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)](https://isocpp.org)

<p align="center">
  <img width="2227" height="828" alt="476306562-d8a1efdd-042b-4f6c-b881-e87ea09308dc" src="https://github.com/user-attachments/assets/392c9d9b-730d-49e8-89f9-1770976d8ba9" />
</p>

AIDA64 is an early prototype system monitoring application implemented with **C++/WinRT** and **WinUI 3**. It provides real‑time access to key system metrics (CPU, memory, disk, network, display) and is designed for extensibility via plugins.

**Status:** Early alpha (prototype).

## Key Features

* Real‑time monitoring: CPU, GPU, memory, disk, network
* Light and dark themes, accent color support
* Modular architecture with plugin support
* WMI‑based data provider for system information
* Optional integrated AI assistant for diagnostics (experimental)

## ScreensShots

<p align="center">
  <img width="2091" height="1275" alt="476306579-d44d49bf-2bd9-4487-af13-b12e720df507" src="https://github.com/user-attachments/assets/81c9b377-d604-4758-9b4c-638347955502" />
  <img width="2126" height="1291" alt="476306571-355d8c0c-8f5b-4eb8-97a9-93951969cfb2" src="https://github.com/user-attachments/assets/bfd52f50-48e8-404c-9bb0-0b2e99684306" />
  <img width="2108" height="1252" alt="476306583-ecfe8016-0141-4f43-96f8-7c4d057063cc" src="https://github.com/user-attachments/assets/04605465-2f26-4c23-b70b-89b824945623" />
</p>


Note: The application is intended to run from Visual Studio. Some data collection relies on WMI and may require elevated permissions.

## Architecture (brief)

* **UI (WinUI 3):** application pages (CPU, Memory, Display, AI Assistant, Settings)
* **Core:** data collection and aggregation (WMI abstraction)
* **Plugins:** extend functionality via external modules/DLLs
* **Assistant:** chat assistant subsystem (may require network access)

## Application Pages

* **CPU:** per‑core usage, frequencies, sensor temperatures
* **Memory:** RAM usage, swap activity, available memory
* **Display:** resolution, refresh rate, color profile
* **AI Assistant:** diagnostics and guidance (experimental)
* **Settings:** themes, thresholds, update channels

## Roadmap

* Complete core monitoring modules (CPU/GPU/Memory)
* Document plugin API and extension points
* Improve data accuracy and UI performance
