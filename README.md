# AIDA64‑Preview

[![C++](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)](https://isocpp.org)

<p align="center">
  <img width="2227" height="828" alt="Снимок экрана 2025-08-09 225906" src="https://github.com/user-attachments/assets/d8a1efdd-042b-4f6c-b881-e87ea09308dc" />
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
  <img width="2126" height="1291" alt="Снимок экрана 2025-08-09 225942" src="https://github.com/user-attachments/assets/355d8c0c-8f5b-4eb8-97a9-93951969cfb2" width="45%"/>
  <img width="2091" height="1275" alt="Снимок экрана 2025-08-09 230020" src="https://github.com/user-attachments/assets/d44d49bf-2bd9-4487-af13-b12e720df507" width="45%"/>
  <img width="2108" height="1252" alt="Снимок экрана 2025-08-09 230044" src="https://github.com/user-attachments/assets/ecfe8016-0141-4f43-96f8-7c4d057063cc" width="45%"/>
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
* Add tests and gather user feedback

## Contribution & Code Style

* Submit pull requests via GitHub: use feature branches and clear commit messages
* Preferred style: modern C++ (C++17/20), follow C++/WinRT idioms
* Unit tests for core logic and manual UI validation are encouraged
