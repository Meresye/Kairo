# https://kairo.meresye.xyz/

# KAIRO DDoS

A high-performance desktop stress-testing and HTTP benchmarking tool built with **WPF and C#**, featuring a sleek, modern, and responsive user interface designed for authorized infrastructure load testing.

## Preview

![KAIRO Preview](https://i.yourimageshare.com/eiBXtZ0GMQ.gif)

## Features

- **Modern WPF UI**: Sleek, hardware-accelerated desktop interface built with C# and XAML.
- **Live Attack Dashboard**: Real-time monitoring of total requests, RPS (Requests Per Second), successful/failed counters, and progress indicators.
- **High-Performance Async Engine**: Multithreaded and asynchronous HTTP request engine optimized for maximum throughput without UI freezes.
- **Proxy Support**: Flexible configuration options (`ip:port` or `user:pass@ip:port`) for distributed testing loads.
- **Config Management**: Automatic handling of user settings and consent verification.
- **Graceful Termination**: Instantaneous stop controls to safely halt tests at any time.

## Requirements

- **OS**: Windows 10 / 11 (64-bit)
- **Runtime**: .NET 8.0 Runtime (or newer)
- **Hardware**: Multi-core processor recommended for high concurrency tests

## Installation & Setup

1. Download the latest release package or clone the repository.
2. Ensure you have the [.NET Desktop Runtime](https://dotnet.microsoft.com/download/dotnet) installed on your system.
3. Open `Kairo.exe` to launch the application.

## Usage

1. **Target Configuration**: Input the target domain or IP address in the designated field.
2. **Proxy Setup**: (Optional) Load a `proxy.txt` file or input proxy details directly into the configuration panel.
3. **Power & Duration**: Configure your concurrency levels and test duration.
4. **Execute**: Launch the stress test and monitor real-time telemetry on the dashboard. Use the stop button at any time to abort the test cleanly.

## Project Layout

```text
Kairo.exe            Main application executable
Kairo.deps.json      Runtime dependency manifests
proxy.txt            Optional proxy list (auto-detected if present)
settings.json        User preferences and configuration storage
```

## Notes

- SSL verification behavior can be configured within the application settings to accommodate self-signed endpoints.
- No telemetry or diagnostic data is transmitted outside of the explicitly defined target environment.

---

## Legal Notice

This tool is intended **strictly for educational purposes, security research, and authorized stress tests** on infrastructure you own or have **explicit written permission** to test. Running it against systems without prior authorization is illegal and may result in criminal prosecution. The authors assume no liability for misuse — **you are solely responsible for how you use this software.**
