# JavaScript/TypeScript Landscape

A beautiful, interactive landscape inspired by [CNCF Landscape2](https://github.com/cncf/landscape2), showcasing the JavaScript and TypeScript ecosystem—frameworks, libraries, tools, and more.

---

## 🌟 Overview

This project uses [landscape2](https://github.com/cncf/landscape2) to generate a static, customizable landscape site from simple YAML files.  
You can explore, extend, and share your own curated view of the JS/TS world.

---

## 🚀 Quick Start

### 1. Clone the Repository

```sh
git clone https://github.com/yourusername/js-landscape.git
cd my-landscape
```

### 2. Install landscape2

```sh
npm install -g landscape2
```

### 3. Build the Landscape

```sh
landscape2 build --data-file data.yml --settings-file settings.yml --logos-path logos --output-dir build
```

### 4. Serve Locally

```sh
landscape2 serve --landscape-dir build
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

---

## 🛠️ Configuration

- **`data.yml`** — Main landscape data (categories, subcategories, items)
- **`settings.yml`** — Site configuration (colors, groups, footer, header, etc.)
- **`guide.yml`** — Category and subcategory descriptions
- **`games.yml`** — Quiz and games configuration

See [landscape2 docs](https://github.com/cncf/landscape2/tree/main/docs/config) for full details.

---

## 🔑 GitHub Integration

To enable GitHub repo stats (stars, contributors, etc.), set a GitHub token:

**PowerShell (temporary):**
```powershell
$env:GITHUB_TOKEN = "your_token_here"
landscape2 build --data-file data.yml --settings-file settings.yml --logos-path logos --output-dir build
```

**Permanent (add to your PowerShell profile):**
```powershell
notepad $PROFILE
# Add this line:
$env:GITHUB_TOKEN = "your_token_here"
```

**Linux/macOS:**
```sh
export GITHUB_TOKEN=your_token_here
landscape2 build --data-file data.yml --settings-file settings.yml --logos-path logos --output-dir build
```

---

## 🤝 Contributing

We welcome contributions!  
To add or update projects, categories, or improve the site:

1. **Fork** this repo and create a new branch.
2. **Edit the YAML files** (`data.yml`, `settings.yml`, etc.).
3. **Build and preview** your changes locally.
4. **Commit and push** your changes.
5. **Open a Pull Request**.

Please follow the [landscape2 contribution guidelines](https://github.com/cncf/landscape2/blob/main/CONTRIBUTING.md) for best practices.

---

## 📁 Project Structure

```
my-landscape/
├── data.yml         # Landscape data
├── settings.yml     # Site configuration
├── guide.yml        # Guide content
├── games.yml        # Games/quiz config
├── logos/           # Project logos
├── build/           # Generated static site
└── ...
```

---

## 📄 License

This project is open source, available under the [Apache 2.0 License](LICENSE).

---

## 🙋‍♂️ Questions?

- See [landscape2 documentation](https://github.com/cncf/landscape2/tree/main/docs)
- Open an [issue](https://github.com/yourusername/my-landscape/issues) for help or suggestions

---

Happy exploring! 🚀