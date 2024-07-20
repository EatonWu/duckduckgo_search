A fork of https://github.com/kevin-rs/duckduckgo that has the option of returning a Vec<(String, String)> instead of simply printing out the search results using the DuckDuckGoSearch struct and calling
DuckDuckGoSearch.search() function, where (String, String) is (Title_Of_Page, Page_Url)

# 🦆 DuckDuckGo

[![Crates.io](https://img.shields.io/crates/v/duckduckgo.svg)](https://crates.io/crates/duckduckgo)
[![docs](https://docs.rs/duckduckgo/badge.svg)](https://docs.rs/duckduckgo/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

```sh
duckduckgo 0.1.2

▓█████▄  █    ██  ▄████▄   ██ ▄█▀▓█████▄  █    ██  ▄████▄   ██ ▄█▀  ▄████  ▒█████  
▒██▀ ██▌ ██  ▓██▒▒██▀ ▀█   ██▄█▒ ▒██▀ ██▌ ██  ▓██▒▒██▀ ▀█   ██▄█▒  ██▒ ▀█▒▒██▒  ██▒
░██   █▌▓██  ▒██░▒▓█    ▄ ▓███▄░ ░██   █▌▓██  ▒██░▒▓█    ▄ ▓███▄░ ▒██░▄▄▄░▒██░  ██▒
░▓█▄   ▌▓▓█  ░██░▒▓▓▄ ▄██▒▓██ █▄ ░▓█▄   ▌▓▓█  ░██░▒▓▓▄ ▄██▒▓██ █▄ ░▓█  ██▓▒██   ██░
░▒████▓ ▒▒█████▓ ▒ ▓███▀ ░▒██▒ █▄░▒████▓ ▒▒█████▓ ▒ ▓███▀ ░▒██▒ █▄░▒▓███▀▒░ ████▓▒░
 ▒▒▓  ▒ ░▒▓▒ ▒ ▒ ░ ░▒ ▒  ░▒ ▒▒ ▓▒ ▒▒▓  ▒ ░▒▓▒ ▒ ▒ ░ ░▒ ▒  ░▒ ▒▒ ▓▒ ░▒   ▒ ░ ▒░▒░▒░ 
 ░ ▒  ▒ ░░▒░ ░ ░   ░  ▒   ░ ░▒ ▒░ ░ ▒  ▒ ░░▒░ ░ ░   ░  ▒   ░ ░▒ ▒░  ░   ░   ░ ▒ ▒░ 
 ░ ░  ░  ░░░ ░ ░ ░        ░ ░░ ░  ░ ░  ░  ░░░ ░ ░ ░        ░ ░░ ░ ░ ░   ░ ░ ░ ░ ▒  
   ░       ░     ░ ░      ░  ░      ░       ░     ░ ░      ░  ░         ░     ░ ░  
 ░               ░                ░               ░
  Search and advanced search in DuckDuckGo 
  ========================================

  Perform searches and advanced searches on DuckDuckGo from the command line.
```

> 🚀 **duckduckgo**: A powerful Rust-based command-line tool for seamless DuckDuckGo searches.

## 📖 Table of Contents

- [Installation](#-installation)
- [Features](#-features)
- [Usage](#-usage)
- [Options](#-options)
- [Contributing](#-contributing)
- [License](#-license)

## 🚀 Installation

To install `duckduckgo`, use the following Cargo command:

```bash
cargo install --locked duckduckgo
```

## ✨ Features

- Perform DuckDuckGo searches with or without operators.
- Customizable user agent, proxy, and cookie support.
- Beautiful ANSI-colored output.

## 🚗 Usage

Learn how to use the duckduckgo and explore its features with the following examples:

### Perform a basic search:

```bash
duckduckgo --query "rust lang"
```

### Use search operators:

```bash
duckduckgo --query "rust lang" --operators "+tutorial"
```

### Enable safe search:

```bash
duckduckgo --query "rust lang" --safe
```

### Set the output format to detailed:

```bash
duckduckgo --query "rust lang" --format
```

### Limit the number of results to 3:

```bash
duckduckgo --query "rust lang" --limit 3
```

### Set user agent:

```bash
duckduckgo --query "rust lang" --user-agent "chrome"
```

<details>
<summary><code>Available Browsers/Agents</code></summary>

| Browser/Agent             |
|---------------------------|
| firefox                   |
| chrome                    |
| edge                      |
| safari                    |
| opera                     |
| ie11                      |
| android                   |
| ios                       |
| edge_android              |
| opera_mini                |
| uc_browser                |
| blackberry                |
| mozilla                   |
| bingbot                   |
| yahoo_slurp               |
| duckduckgo                |
| baiduspider               |
| yandexbot                 |
| ahrefsbot                 |
| mj12bot                   |
| semrushbot                |
| sogou_spider              |
| exabot                    |
| dotbot                    |
| facebook                  |
| pinterest                 |
| slackbot                  |
| discord                   |
| zoom                      |
| whatsapp                  |
| applebot                  |
| flipboard                 |
| outlook                   |
| linux_firefox             |
| linux_firefox_alternative |
| windows_firefox           |
| older_windows_firefox     |
| linux_chrome              |
| macos_safari              |
| android_chrome            |
| ios_chrome                |
| linux_opera               |
| macos_edge                |
| windows_edge              |
| android_samsung_browser   |
| ios_samsung_browser       |
| linux_brave               |
| windows_brave             |
| android_brave             |
| ios_brave                 |
| linux_firefox_new         |
| linux_chrome_new          |
| macos_safari_new          |
| windows_ie_new            |
| android_chrome_new         |
| ios_chrome_new             |
| linux_opera_new            |
| macos_edge_new              |
| android_samsung_browser_new |
| ios_samsung_browser_new     |
| linux_brave_new              |
| windows_brave_new            |
| android_brave_new            |
| ios_brave_new                |
| linux_firefox_alternative_new |
| windows_firefox_new           |
| linux_chrome_alternative_new  |
| macos_safari_alternative_new  |
| windows_ie_alternative_new    |
| android_chrome_alternative_new |
| ios_chrome_alternative_new     |
| linux_opera_alternative_new    |
| macos_edge_alternative_new      |
| windows_edge_alternative_new    |
| android_samsung_browser_alternative_new |
| ios_samsung_browser_alternative_new     |
| linux_brave_alternative_new              |
| windows_brave_alternative_new            |
| android_brave_alternative_new            |
| ios_brave_alternative_new                |

</details>

### Set cookie for subsequent requests:

```bash
duckduckgo --query "rust lang" --cookie
```

### Set proxy:

```bash
duckduckgo --query "rust lang" --proxy "socks5://192.168.1.1:9000"
```

## 🎨 Options

| Option                   | Default Value | Description                                              |
|--------------------------|---------------|----------------------------------------------------------|
| `--safe`                 | `false`       | Enable safe search.                                      |
| `--proxy`                | `""`          | Set a proxy for the search (e.g., "socks5://192.168.1.1:9000"). |
| `--user-agent`           | `firefox` | Set a custom user agent for the search.                   |
| `--cookie`               | `true`        | Set a cookie for the search.                              |
| `--format`               | `false`       | Set the output format (`false` for list or `true` for detailed). |
| `--limit`                | `10`          | Limit the number of results (default is 10).             |

## 🤝 Contributing

Contributions and feedback are welcome! If you'd like to contribute, report an issue, or suggest an enhancement, please engage with the project on [GitHub](https://github.com/wiseaidev/duckduckgo).
Your contributions help improve this CLI for the community.

## 📄 License

This project is licensed under the [MIT License](LICENSE).
