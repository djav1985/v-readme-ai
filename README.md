<p align="center">
  <img src="https://img.icons8.com/?size=512&id=55494&format=png" width="99">
  <img src="https://img.icons8.com/?size=512&id=kTuxVYRKeKEY&format=png" width="99">
</p>
<h1 align="center">README-AI</h1>
<p align="center">
  <em>Automated <code>README</code> file generator, powered by large language model APIs</em>
</p>
<p align="center">
  <a href="https://github.com/eli64s/readme-ai/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/eli64s/readme-ai/release-pipeline.yml?logo=githubactions&label=CICD&logoColor=white&color=c125ff"
    alt="github-actions">
  </a>
  <a href="https://app.codecov.io/gh/eli64s/readme-ai">
    <img src="https://img.shields.io/codecov/c/github/eli64s/readme-ai?logo=codecov&logoColor=white&label=Coverage&color=c125ff"
    alt="codecov">
  </a>
  <a href="https://pypi.python.org/pypi/readmeai/">
    <img src="https://img.shields.io/pypi/v/readmeai?logo=Python&logoColor=white&label=PyPI&color=c125ff" alt="pypi-version">
  </a>
  <a href="https://www.pepy.tech/projects/readmeai">
    <img src="https://img.shields.io/pepy/dt/readmeai?logo=PyPI&logoColor=white&label=Downloads&color=c125ff"
    alt="pepy-total-downloads">
  </a>
  <a href="https://opensource.org/license/mit/">
    <img src="https://img.shields.io/github/license/eli64s/readme-ai?logo=opensourceinitiative&logoColor=white&label=License&color=c125ff"
    alt="license">
  </a>
</p>

> <details><summary>Documentation</summary>
>
> - [Read the official readme-ai docs *(🚧 WIP)*](https://eli64s.github.io/readme-ai)
>
> </details>
>
> <details><summary>Quick Links</summary>
>
> - [📍 Overview](#-overview)
> - [👾 Demo](#-demo)
> - [🧬 Features](#-features)
> - [🚀 Getting Started](#-getting-started)
>   - [⚙️ Installation](#️-installation)
>   - [🤖 Usage](#-usage)
>   - [🧪 Testing](#-testing)
> - [🔧 Configuration](#-configuration)
> - [🎨 Examples](#-examples)
> - [🤝 Contributing](#-contributing)
>
> </details>

---

## 📍 Overview

***Objective***

Readme-ai is a developer tool that auto-generates README.md files using a combination of data extraction and generative ai. Simply provide a repository URL or local path to your codebase and a well-structured and detailed README file will be generated for you.

***Motivation***

Streamlines documentation creation and maintenance, enhancing developer productivity. This project aims to enable all skill levels, across all domains, to better understand, use, and contribute to open-source software.<br>

<!--
> [!IMPORTANT]
>
> <sub>Readme-ai is currently under development with an opinionated configuration and setup. It is vital to review all generated text from the LLM API to ensure it accurately represents your project.</sub>
-->

---

## 👾 Demo

### CLI

[readmeai-cli-demo](https://github.com/eli64s/artifacts/assets/43382407/55b8d1b9-06a7-4b1f-b6a7-aaeccdb27679)

### Streamlit

[readmeai-streamlit-demo](https://github.com/eli64s/artifacts/assets/43382407/3eb39fcf-c1df-49c6-bb5c-63e141857ae3)

> [!TIP]
>
> <sub>Check out this [YouTube tutorial](https://www.youtube.com/watch?v=NiUrm1ni7bE) created by a community member!</sub>
>

<!--
> [!TIP]
>
> <sub>Offline mode is useful for generating a boilerplate README at no cost. View the offline README.md example [here!](https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-offline.md)</sub>
-->

---

## 🧬 Features

- **Flexible README Generation**: Robust repository context extraction engine combined with generative AI.
- **Customizable Output**: Dozens of CLI options for styling/formatting, badges, header designs, and more.
- **Language Agnostic**: Works across a wide range of programming languages and project types.
- **Multi-LLM Support**: Compatible with `OpenAI`, `Ollama`, `Google Gemini` and `Offline Mode`.
  - **Offline Mode**: Generate a boilerplate README without calling an external API.

See a few examples of the README-AI customization options below:

<table>
  <!-- row 0 -->
  <tr>
    <td colspan="2" align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/project-logo-custom.png" alt="default-header" width="900"/><br>
      <code>--emojis --image custom --badge-color DE3163 --header-style compact --toc-style links</code>
    </td>
  </tr>
  <!-- row 1 -->
  <tr>
    <td colspan="2" align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-minimal.png" width="900"/><br>
      <code>--image cloud --header-style compact --toc-style fold</code>
    </td>
  </tr>
  <!-- row 2 -->
  <tr>
    <td align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-cloud.png" alt="cloud-db-logo" width="450"/><br>
      <code>--align left --badge-style flat-square --image cloud</code>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-gradient.png" alt="gradient-markdown-logo" width="450"/><br>
      <code>--align left --badge-style flat --image gradient</code>
    </td>
  </tr>
  <!-- row 3 -->
  <tr>
    <td align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-custom.png" alt="custom-logo" width="450"/><br>
      <code>--badge-style flat --image custom</code>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-skills.png" alt="skills-light" width="450"/><br>
      <code>--badge-style skills-light --image grey</code>
    </td>
  </tr>
  <tr>
  <!-- row 4 -->
    <td align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-flat-square.png" alt="readme-ai-header" width="450"/><br>
      <code>--badge-style flat-square</code>
    </td>
    <td align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-black.png" alt="black-logo" width="450"/><br>
      <code>--badge-style flat --image black</code>
    </td>
  </tr>
  <!-- row 5 -->
  <tr>
    <td colspan="2" align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-default-v2.png" alt="default-header" width="900"/><br>
      <code>--image custom --badge-color 00ffe9 --badge-style flat-square --header-style classic</code>
    </td>
  </tr>
  <!-- row 6 -->
  <tr>
    <td colspan="2" align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/project-logo-dalle.png" alt="default-header" width="900"/><br>
      <code>--image llm --badge-style plastic --header-style classic</code>
    </td>
  </tr>
  <!-- row 7 -->
  <tr>
    <td colspan="2" align="center">
      <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/header-padded.png" alt="default-header" width="900"/><br>
      <code>--image custom --badge-color BA0098 --badge-style flat-square --header-style modern --toc-style fold</code>
    </td>
  </tr>
</table>

See the <a href="https://github.com/eli64s/readme-ai?tab=readme-ov-file#-configuration">Configuration</a> section for a complete list of CLI options.

<details closed>
  <summary><strong>👋 Overview</strong></summary><br>
  <table>
    <tr>
      <td><b>Overview</b><br>
        <p>
        <ol>
          - High-level introduction of the project, focused on the value proposition and use-cases, rather than technical aspects.
        </ol>
      </td>
    </tr>
    <tr>
      <td align="center"><img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/llm-overview.png" alt="llm-overview" width="700" /></td>
    </tr>
  </table>
</details>

<details closed>
  <summary><strong>🧩 Features</strong></summary><br>
  <table>
    <tr>
      <td><b>Features Table</b><br>
        <p>
        <ol>
          - Generated markdown table that highlights the key technical features and components of the codebase. This table is generated using a structured <a href="https://github.com/eli64s/readme-ai/blob/main/readmeai/config/settings/prompts.toml#L18">prompt template.</a>
        </ol>
        </p>
      </td>
    </tr>
    <tr>
      <td align="center"><img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/llm-features.png" alt="llm-features" width="700" /></td>
    </tr>
  </table>
</details>

<details closed>
  <summary><strong>📄 Codebase Documentation</strong></summary><br>
  <table>
    <tr>
      <td><b>Repository Structure</b><br>
        <p>
        <ol>
          - Directory tree structure is generated using pure Python <a href="https://github.com/eli64s/readme-ai/blob/main/readmeai/generators/tree.py">(tree.py)</a> and embedded in the README.
        </ol>
        </p>
      </td>
    </tr>
    <tr>
      <td align="center">
        <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/directory-tree.png" alt="directory-tree" width="700" />
      </td>
    </tr>
    <tr>
      <td style="padding-top:20px;">
        <b>File Summaries</b><br>
        <p>
        <ol>
          - Summarizes key files in the codebase, and also used as context for additional <a href="https://github.com/eli64s/readme-ai/blob/main/readmeai/config/settings/prompts.toml">prompts!</a>
        </ol>
        </p>
      </td>
    </tr>
    <tr>
      <td align="center">
        <img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/llm-summaries.png" alt="llm-summaries" width="700" />
    </tr>
  </table>
</details>

<details closed>
  <summary><strong>🚀 Quickstart Commands</strong></summary>
  <br>
  <table>
    <tr>
      <td><b>Getting Started</b><br>
      <p>
      <ol>
        - Auto-generated setup guides based on <em>language</em> and <em>dependency</em> analysis.
      </ol>
      <ol>
        - <code>Install</code>, <code>Usage</code>, and <code>Test</code> guides are supported for many languages.
      </ol>
      <ol>
        - The <a href="https://github.com/eli64s/readme-ai/tree/main/readmeai/parsers">parsers</a> module is a collection of tool-specific parsers that extract dependencies and metadata.
      </ol>
      </p>
      </td>
    </tr>
    <tr>
    <td align="center"><img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/quickstart.png" alt="quick-start" width="700" />
    </td>
    </tr>
  </table>
</details>

<details closed>
  <summary><strong>🔰 Contributing Guidelines</strong></summary>
  <br>
  <table>
    <tr>
      <td><b>Contributing Guide</b><br>
      <p>
        <ol>- Dropdown section that outlines general process for contributing to your project.</ol>
        <ol>- Provides links to your contributing guidelines, issues page, and more resources.</ol>
        <ol>- Graph of contributors is also included.</ol>
      </p>
      </td>
    </tr>
    <tr>
      <td align="center"><img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/contributing_guidelines.png" alt="contributing-guidelines" width="700" /></td>
    </tr>
    <tr>
      <td><b>Additional Sections</b><br>
      <p>
        <ol>
          - <code>Project Roadmap</code>, <code>Contributing Guidelines</code>, <code>License</code>, and <code>Acknowledgements</code> are included by default.
        </ol>
      </p>
      </td>
    </tr>
    <tr>
      <td align="center"><img src="https://raw.githubusercontent.com/eli64s/readme-ai/main/examples/images/additional-sections.png" alt="contributing-and-more" width="700" /></td>
    </tr>
  </table>
</details>

---

## 🚀 Getting Started

**System Requirements:**

  - Python 3.9+
  - Package manager/Container: `pip`, `pipx`, `docker`
  - LLM service: `OpenAI`, `Ollama`, `Google Gemini`, `Offline Mode`
    - `Anthropic` and `LiteLLM` coming soon!

**Repository URL or Local Path:**

Make sure to have a repository URL or local directory path ready for the CLI.

- [**GitHub**](https://github.com/)
- [**GitLab**](https://gitlab.com/)
- [**Bitbucket**](https://bitbucket.org/)
- [**File System**](https://en.wikipedia.org/wiki/File_system)

**Select an LLM API Service:**
- [**OpenAI**](https://platform.openai.com/docs/quickstart/account-setup): Recommended, requires an account setup and API key.
- [**Ollama**](https://github.com/ollama/ollama): Free and open-source, potentially slower and more resource-intensive.
- [**Google Gemini**](https://ai.google.dev/tutorials/python_quickstart): Requires a Google Cloud account and API key.
- [**Offline Mode**](https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-offline.md): Generates a boilerplate README without making API calls.

<!--
**OpenAI API Key**

An OpenAI API account and API key are needed to use readme-ai. Get started by creating an account [here](https://platform.openai.com/docs/quickstart/account-setup). Once you have an account, you can create an API key on the [API settings page](https://platform.openai.com/api-keys).

> [!WARNING]
>
> Before using readme-ai, its essential to understand the potential risks and costs associated with using AI-powered tools.
>
> * **Review Sensitive Information**: Ensure all content in your repository is free of sensitive information before running the tool. This project does not remove sensitive data from your codebase, nor from the output README file.
>
> * **API Usage Costs**: The OpenAI API is not free and costs can accumulate quickly! You will be charged for each request made by readme-ai. Be sure to monitor API usage costs using the [OpenAI API Usage Dashboard](https://platform.openai.com/account/usage).
-->

---

### ⚙️ Installation

#### Using `pip`
[![pip](https://img.shields.io/badge/PyPI-3775A9.svg?style=flat&logo=PyPI&logoColor=white)](https://pypi.org/project/readmeai/)

```sh
❯ pip install readmeai
```

#### Using `pipx`
[![pipx](https://img.shields.io/badge/pipx-2CFFAA.svg?style=flat&logo=pipx&logoColor=black)](https://pipxproject.github.io/pipx/installation/)

```sh
❯ pipx install readmeai
```

> [!TIP]
>
> <sub>Use [pipx](https://pipx.pypa.io/stable/installation/) to install and run Python command-line applications without causing dependency conflicts with other packages!</sub>


#### Using `docker`
[![docker](https://img.shields.io/badge/Docker-2496ED.svg?style=flat&logo=Docker&logoColor=white)](https://hub.docker.com/r/zeroxeli/readme-ai)

```sh
❯ docker pull zeroxeli/readme-ai:latest
```

<!--
#### Using `conda`
[![conda](https://img.shields.io/badge/Anaconda-44A833.svg?style=flat&logo=Anaconda&logoColor=white)](https://anaconda.org/zeroxeli/readmeai)

```sh
❯ conda install -c conda-forge readmeai
```
-->

#### From `source`

<details closed><summary><i>Build readme-ai</i></summary><br>

Clone repository and navigate to the project directory:

```sh
❯ git clone https://github.com/eli64s/readme-ai
❯ cd readme-ai
```

#### Using `bash`
[![bash](https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?style=flat&logo=GNU-Bash&logoColor=white)](https://www.gnu.org/software/bash/)

```sh
❯ bash setup/setup.sh
```

#### Using `poetry`
[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)

```sh
❯ poetry install
```

</details>

---

### 🤖 Usage

#### Environment Variables

**OpenAI**

Generate a OpenAI API key and set it as the environment variable `OPENAI_API_KEY`.
```sh
# Using Linux or macOS
❯ export OPENAI_API_KEY=<your_api_key>

# Using Windows
❯ set OPENAI_API_KEY=<your_api_key>
```

**Ollama**

Pull model of your choice from the Ollama registry as follows:
```sh
# i.e. mistral, llama3, gemma2, etc.
❯ ollama pull mistral:latest
```

Start the Ollama server:
```sh
❯ export OLLAMA_HOST=127.0.0.1 && ollama serve
```

<sub>For more details, check out the [Ollama](https://github.com/ollama/ollama-python?tab=readme-ov-file) repository.</sub>

**Google Gemini**

Generate a Google API key and set it as the environment variable `GOOGLE_API_KEY`.
```sh
❯ export GOOGLE_API_KEY=<your_api_key>
```

#### Running `README-AI`

#### Using `pip`
[![pip](https://img.shields.io/badge/PyPI-3775A9.svg?style=flat&logo=PyPI&logoColor=white)](https://pypi.org/project/readmeai/)

With OpenAI API:
```sh
❯ readmeai --repository https://github.com/eli64s/readme-ai \
        --api openai \
        --model gpt-3.5-turbo
```

With Ollama:
```sh
❯ readmeai --repository https://github.com/eli64s/readme-ai \
        --api ollama \
        --model llama3
```

With Gemini:
```sh
❯ readmeai --repository https://github.com/eli64s/readme-ai \
        --api gemini
        --model gemini-1.5-flash
```

Advanced Options:
```sh
❯ readmeai --repository https://github.com/eli64s/readme-ai \
        --output readmeai.md \
        --api openai \
        --model gpt-4-turbo \
        --badge-color A931EC \
        --badge-style flat-square \
        --header-style compact \
        --toc-style fold \
        --temperature 0.1 \
        --tree-depth 2
        --image LLM \
        --emojis
```

#### Using `docker`

[![docker](https://img.shields.io/badge/Docker-2496ED.svg?style=flat&logo=Docker&logoColor=white)](https://hub.docker.com/r/zeroxeli/readme-ai)

```sh
❯ docker run -it \
        -e OPENAI_API_KEY=$OPENAI_API_KEY \
        -v "$(pwd)":/app zeroxeli/readme-ai:latest \
        -r https://github.com/eli64s/readme-ai
```

#### Using `streamlit`

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://readme-ai.streamlit.app/)

<sub>Try directly in your browser on <a href="https://streamlit.io/">Streamlit</a>, no installation required! For more details, see the <a href="https://github.com/eli64s/readme-ai-streamlit">readme-ai-streamlit</a> repository.</sub>

#### From `source`

<details closed><summary><i>Using readme-ai</i></summary><br>

#### Using `bash`
[![bash](https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?style=flat&logo=GNU-Bash&logoColor=white)](https://www.gnu.org/software/bash/)

```sh
❯ conda activate readmeai
❯ python3 -m readmeai.cli.main -r https://github.com/eli64s/readme-ai
```

#### Using `poetry`
[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)

```sh
❯ poetry shell
❯ poetry run python3 -m readmeai.cli.main -r https://github.com/eli64s/readme-ai
```

</details>

---

### 🧪 Testing

#### Using `pytest`
[![pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://docs.pytest.org/en/7.1.x/contents.html)

```sh
❯ make test
```

#### Using `nox`

```sh
❯ make test-nox
```

> [!TIP]
>
> <sub>Use [nox](https://nox.thea.codes/en/stable/) to test application against multiple Python environments and dependencies!</sub>

---

## 🔧 Configuration

Customize your README generation using these CLI options:

| Option | Description | Default |
|--------|-------------|---------|
| `--align` | Text align in header | `center` |
| `--api` | LLM API service (openai, ollama, offline) | `offline` |
| `--badge-color` | Badge color name or hex code | `0080ff` |
| `--badge-style` | Badge icon style type |  `flat` |
| `--base-url` | Base URL for the repository | `v1/chat/completions` |
| `--context-window` | Maximum context window of the LLM API | `3999` |
| `--emojis` | Adds emojis to the README header sections | `False` |
| `--header-style` | Header template style | `classic` |
| `--image` | Project logo image | `blue` |
| `--model` | Specific LLM model to use | `gpt-3.5-turbo` |
| `--output` | Output filename | `readme-ai.md` |
| `--rate-limit` | Maximum API requests per minute | `5` |
| `--repository` | Repository URL or local directory path | `None` |
| `--temperature` | Creativity level for content generation | `0.9` |
| `--toc-style` | Table of contents template style | `bullet` |
| `--top-p` | Probability of the top-p sampling method | `0.9` |
| `--tree-depth` | Maximum depth of the directory tree structure | `2` |

> [!TIP]
> For a full list of options, run `readmeai --help` in your terminal.
<!--
> See the official documentation for more details on [CLI options](https://eli64s.github.io/readme-ai/cli-options).
-->

---

### Project Badges

The `--badge-style` option lets you select the style of the default badge set.

<table>
  <tr>
    <th style="text-align: left;">Style</th>
    <th style="text-align: center;">Preview</th>
  </tr>
  <tr>
    <td><strong>default</strong></td>
    <td align="center"><a href="https://img.shields.io/github/license/eli64s/readme-ai?flat&color=0080ff&logo=opensourceinitiative&logoColor=white" target="_blank"><img src="https://img.shields.io/github/license/eli64s/readme-ai?flat&color=0080ff&logo=opensourceinitiative&logoColor=white"></a> <a href="https://img.shields.io/github/last-commit/eli64s/readme-ai?flat&color=0080ff&logo=git&logoColor=white" target="_blank"><img src="https://img.shields.io/github/last-commit/eli64s/readme-ai?flat&color=0080ff&logo=git&logoColor=white"></a> <a href="https://img.shields.io/github/languages/top/eli64s/readme-ai?flat&color=0080ff" target="_blank"><img src="https://img.shields.io/github/languages/top/eli64s/readme-ai?flat&color=0080ff"></a> <a href="https://img.shields.io/github/languages/count/eli64s/readme-ai?flat&color=0080ff" target="_blank"><img src="https://img.shields.io/github/languages/count/eli64s/readme-ai?flat&color=0080ff"></a></td>
  </tr>
  <tr>
    <td><strong>flat</strong></td>
    <td align="center"><a href="https://img.shields.io/badge/Python-3776AB.svg?&style=flat&logo=Python&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB.svg?&style=flat&logo=Python&logoColor=white"></a></td>
  </tr>
  <tr>
    <td><strong>flat-square</strong></td>
    <td align="center"><a href="https://img.shields.io/badge/Python-3776AB.svg?&style=flat-square&logo=Python&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB.svg?&style=flat-square&logo=Python&logoColor=white"></a></td>
  </tr>
  <tr>
    <td><strong>for-the-badge</strong></td>
    <td align="center"><a href="https://img.shields.io/badge/Python-3776AB.svg?&style=for-the-badge&logo=Python&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB.svg?&style=for-the-badge&logo=Python&logoColor=white"></a></td>
  </tr>
  <tr>
    <td><strong>plastic</strong></td>
    <td align="center"><a href="https://img.shields.io/badge/Python-3776AB.svg?&style=plastic&logo=Python&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB.svg?&style=plastic&logo=Python&logoColor=white"></a></td>
  </tr>
  <tr>
    <td><strong>skills</strong></td>
    <td align="center"><a href="https://skillicons.dev/" target="_blank"><img src="https://skillicons.dev/icons?i=py" alt="Python Skill Icon"></a></td>
  </tr>
  <tr>
    <td><strong>skills-light</strong></td>
    <td align="center"><a href="https://skillicons.dev/" target="_blank"><img src="https://skillicons.dev/icons?i=py&theme=light" alt="Python Skill Light Icon"></a></td>
  </tr>
  <tr>
    <td><strong>social</strong></td>
    <td align="center"><a href="https://img.shields.io/badge/Python-3776AB.svg?&style=social&logo=Python&logoColor=white" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB.svg?&style=social&logo=Python&logoColor=white"></a></td>
  </tr>
</table>

When providing the `--badge-style` option, readme-ai does two things:

1. Formats the default badge set to match the selection (i.e. flat, flat-square, etc.).
2. Generates an additional badge set representing your projects dependencies and tech stack (i.e. Python, Docker, etc.)

#### Example
>
> ```sh
> ❯ readmeai --badge-style flat-square --repository https://github.com/eli64s/readme-ai
> ```
>

#### Output
>
> {... project logo ...}
>
> {... project name ...}
>
> {...project slogan...}
>
> <img src="https://img.shields.io/github/license/eli64s/readme-ai?style=flat-square&color=0080ff&logo=opensourceinitiative&logoColor=white">
> <img src="https://img.shields.io/github/last-commit/eli64s/readme-ai?style=flat-square&color=0080ff&logo=git&logoColor=white">
> <img src="https://img.shields.io/github/languages/top/eli64s/readme-ai?style=flat-square&color=0080ff">
> <img src="https://img.shields.io/github/languages/count/eli64s/readme-ai?style=flat-square&color=0080ff">
>
> <br>
>
>	*Developed with the software and tools below.*
>
> <img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?style=flat-square&logo=GNU-Bash&logoColor=white">
> <img src="https://img.shields.io/badge/tqdm-FFC107.svg?style=flat-square&logo=tqdm&logoColor=black">
> <img src="https://img.shields.io/badge/Pydantic-E92063.svg?style=flat-square&logo=Pydantic&logoColor=white">
> <img src="https://img.shields.io/badge/YAML-CB171E.svg?style=flat-square&logo=YAML&logoColor=white" alt="YAML">
> <img src="https://img.shields.io/badge/Poetry-60A5FA.svg?style=flat-square&logo=Poetry&logoColor=white">
> <img src="https://img.shields.io/badge/OpenAI-412991.svg?style=flat-square&logo=OpenAI&logoColor=white">
> <br>
> <img src="https://img.shields.io/badge/Python-3776AB.svg?style=flat-square&logo=Python&logoColor=white">
> <img src="https://img.shields.io/badge/AIOHTTP-2C5BB4.svg?style=flat-square&logo=AIOHTTP&logoColor=white">
> <img src="https://img.shields.io/badge/Docker-2496ED.svg?style=flat-square&logo=Docker&logoColor=white">
> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat-square&logo=GitHub-Actions&logoColor=white">
> <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat-square&logo=Pytest&logoColor=white">
>
> <br>
>
> {... end of header ...}
>

---

### Project Logo

Select a project logo using the `--image` option.

<table>
  <tr>
    <td><strong>blue</strong></td>
    <td><strong>gradient</strong></td>
    <td><strong>black</strong></td>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100"></td>
    <td><img src="https://img.icons8.com/?size=512&id=55494&format=png" width="100"></td>
    <td><img src="https://img.icons8.com/external-tal-revivo-regular-tal-revivo/96/external-readme-is-a-easy-to-build-a-developer-hub-that-adapts-to-the-user-logo-regular-tal-revivo.png" width="100"></td>
  </tr>
  <tr>
    <td><strong>cloud</strong></td>
    <td><strong>purple</strong></td>
    <td><strong>grey</strong></td>
  </tr>
  <tr>
    <td><img src="https://cdn-icons-png.flaticon.com/512/6295/6295417.png" width="100"></td>
    <td><img src="https://img.icons8.com/external-tal-revivo-duo-tal-revivo/100/external-markdown-a-lightweight-markup-language-with-plain-text-formatting-syntax-logo-duo-tal-revivo.png" width="100"></td>
    <td><img src="https://img.icons8.com/external-tal-revivo-filled-tal-revivo/96/external-markdown-a-lightweight-markup-language-with-plain-text-formatting-syntax-logo-filled-tal-revivo.png" width="100"></td>
  </tr>
</table>

For custom images, see the following options:
- Use `--image custom` to invoke a prompt to upload a local image file path or URL.
- Use `--image llm` to generate a project logo using a LLM API (OpenAI only).

---

## 🎨 Examples

| Language/Framework | Output File | Input Repository | Description |
|--------------------|-------------|------------------|-------------|
| Python | [readme-python.md][0a] | [readme-ai][0b] | Core readme-ai project |
| TypeScript & React | [readme-typescript.md][1a] | [ChatGPT App][1b] | React Native ChatGPT app |
| PostgreSQL & DuckDB | [readme-postgres.md][2a] | [Buenavista][2b] | Postgres proxy server |
| Kotlin & Android | [readme-kotlin.md][3a] | [file.io Client][3b] | Android file sharing app |
| Streamlit | [readme-streamlit.md][4a] | [readme-ai-streamlit][4b] | Streamlit UI for readme-ai app |
| Rust & C | [readme-rust-c.md][5a] | [CallMon][5b] | System call monitoring tool |
| Docker & Go | [readme-go.md][6a] | [docker-gs-ping][6b] | Dockerized Go app |
| Java | [readme-java.md][7a] | [Minimal-Todo][7b] | Minimalist todo Java app |
| FastAPI & Redis | [readme-fastapi-redis.md][8a] | [async-ml-inference][8b] | Async ML inference service |
| Jupyter Notebook | [readme-mlops.md][9a] | [mlops-course][9b] | MLOps course repository |
| Apache Flink | [readme-local.md][10a] | Local Directory | Example using a local directory |

> [!NOTE]
> See additional README file examples [here](https://github.com/eli64s/readme-ai/tree/main/examples/markdown).

[0a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-python.md "readme-python.md"
[0b]: https://github.com/eli64s/readme-ai "readme-ai"
[1a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-typescript.md "readme-typescript.md"
[1b]: https://github.com/Yuberley/ChatGPT-App-React-Native-TypeScript "ChatGPT App"
[2a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-postgres.md "readme-postgres.md"
[2b]: https://github.com/jwills/buenavista "Buenavista"
[3a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-kotlin.md "readme-kotlin.md"
[3b]: https://github.com/rumaan/file.io-Android-Client "file.io Client"
[4a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-streamlit.md "readme-streamlit.md"
[4b]: https://github.com/eli64s/readme-ai-streamlit "readme-ai-streamlit"
[5a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-rust-c.md "readme-rust-c.md"
[5b]: https://github.com/DownWithUp/CallMon "CallMon"
[6a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-go.md "readme-go.md"
[6b]: https://github.com/olliefr/docker-gs-ping "docker-gs-ping"
[7a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-java.md "readme-java.md"
[7b]: https://github.com/avjinder/Minimal-Todo "Minimal-Todo"
[8a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-fastapi-redis.md "readme-fastapi-redis.md"
[8b]: https://github.com/FerrariDG/async-ml-inference "async-ml-inference"
[9a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-mlops.md "readme-mlops.md"
[9b]: https://github.com/GokuMohandas/mlops-course "mlops-course"
[10a]: https://github.com/eli64s/readme-ai/blob/main/examples/markdown/readme-local.md "readme-local.md"

---

## 📌 Roadmap

- [ ] **v1.0** release with new features, bug fixes, and improved performance.
- [ ] Develop `readmeai-vscode` extension to generate README files (WIP).
- [ ] Add new CLI options to enhance README file customization.
  - [ ] `--audit` to review existing README files and suggest improvements.
  - [ ] `--template` to select a README template style (i.e. ai, data, web, etc.)
  - [ ] `--language` to generate README files in any language (i.e. zh-CN, ES, FR, JA, KO, RU)
- [ ] Develop robust documentation generator to build full project docs (i.e. Sphinx, MkDocs)
- [ ] Create community-driven templates for README files and gallery of readme-ai examples.
- [ ] GitHub Actions script to automatically update README file content on repository push.

---

## 📒 Changelog

[Changelog][0]

---

## 🤝 Contributing

To grow the project, we need your help! See the links below to get started.

- [🔰 Contributing Guide][1]
- [👋 Start a Discussion][2]
- [🐛 Open an Issue][3]

<br>
<p align="left">
  <a href="https://github.com{/eli64s/readme-ai/}graphs/contributors">
    <img src="https://contrib.rocks/image?repo=eli64s/readme-ai">
  </a>
</p>

---

## 🎗 License

[MIT][4]

---

## 👊 Acknowledgments

- [Shields.io](https://shields.io/)
- [Aveek-Saha/GitHub-Profile-Badges](https://github.com/Aveek-Saha/GitHub-Profile-Badges)
- [Ileriayo/Markdown-Badges](https://github.com/Ileriayo/markdown-badges)
- [tandpfun/skill-icons](https://github.com/tandpfun/skill-icons)

<p align="right">
  <a href="#-overview">⬆️ Top</a>
</p>

---

[0]: https://github.com/eli64s/readme-ai/blob/main/CHANGELOG.md "📒 Changelog"
[1]: https://github.com/eli64s/readme-ai/blob/main/CONTRIBUTING.md "🔰 Contributing Guide"
[2]: https://github.com/eli64s/readme-ai/discussions "👋 Start a Discussion"
[3]: https://github.com/eli64s/readme-ai/issues "🐛 Open an Issue"
[4]: https://github.com/eli64s/readme-ai/blob/main/LICENSE "🎗 License"
