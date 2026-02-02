# PrjMonitoradorSites (Go)

A simple **CLI website monitor** written in **Go**.  
It checks a list of URLs, prints whether they are online/offline, and saves the results to a local log file.

> Goal: practice Go fundamentals (functions, slices, loops, `time`, HTTP requests, and basic file I/O).

---

## ✨ Features

- Menu-driven CLI (interactive options)
- Checks multiple websites (URL list in code)
- Writes results to `HELLO/log.txt` with timestamp and status (`online: true/false`)
- Built with standard Go libraries (e.g., `net/http`, `time`)

---

## 📁 Project Structure

```text
.
└── HELLO/
    ├── hello.go      # CLI + monitoring logic
    └── log.txt       # Monitoring history (generated/updated)
```

## ✅ Requirements

Go installed (recommended: Go 1.20+)

## 🚀 How to Run

### Clone the repository:

git clone https://github.com/KentoImayoshi/PrjMonitoradorSites.git
cd PrjMonitoradorSites


### Run the program:

cd HELLO
go run hello.go

Tip: If you prefer, you can also try go run . (works if your folder is a Go module / has the right setup).

## 🧾 Log Output

The app writes entries like this in HELLO/log.txt:

10/10/2025 14:32:07 - https://example.com - online: true
10/10/2025 14:32:08 - https://another-example.com - online: false

## 🔧 Customizing the URLs

Open HELLO/hello.go and edit the URL list (slice/array) used by the monitor.
You can add/remove websites and run again.

## 🧯 Troubleshooting

It says a website is offline but it opens in the browser

Some websites block automated requests or require specific headers.

Try another URL or check if the endpoint is accessible without authentication.

Permission error writing log.txt

Make sure you have write permission in the HELLO/ folder.

Try running from a terminal with the correct permissions.


## 📜 License

This project is licensed under the **MIT License**. See `LICENSE`.
