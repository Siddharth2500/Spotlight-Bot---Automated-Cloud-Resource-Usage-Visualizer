# 🚀 Spotlight-Bot — Automated Cloud Resource Usage Visualizer

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg?logo=python&logoColor=white)  
![Tool](https://img.shields.io/badge/Resource-Visualizer-FF5252.svg?logo=cloud)  
![Features](https://img.shields.io/badge/Features-Usage%20&%20Cost-4CAF50.svg?logo=chart-bar)  
![Reports](https://img.shields.io/badge/Reports-PNG-2196F3.svg?logo=image)  
![CI/CD](https://img.shields.io/badge/CI/CD-Ready-2088FF.svg?logo=githubactions)  
![Dependencies](https://img.shields.io/badge/Dependencies-Matplotlib-green.svg?logo=python)

**Spotlight-Bot** is a **Python 3** tool designed to automatically load cloud-resource usage data (hours & cost) and generate visual charts of usage trends over time. It’s built for cloud engineers, operations teams, and cost-analysis dashboards who want a quick visual overview of resource consumption.

-----------

## 🛠 Tech & Languages

| Layer        | Tech / Format              | Purpose                              |
|--------------|----------------------------|--------------------------------------|
| Language     | **Python 3.10+**           | Main codebase                        |
| Core Logic   | JSON parsing + Matplotlib   | Load usage data, generate visual plots |
| Reports      | **PNG Image**              | Chart output for human review        |
| Execution    | Script / Colab / Notebook  | Flexible usage environment           |
| Logging      | Console output             | Print summary and file location      |

---

## 🌐 Architecture

Flow:  
1. Step 1 – Load `usage_data.json` containing daily usage and cost for each resource type  
2. Step 2 – For each resource type, sort data by date and extract usage-hours and cost-USD  
3. Step 3 – Use Matplotlib to plot line charts of hours and cost over the past N days  
4. Step 4 – Save the visualization as `usage_visualization.png` and display inline in Colab  

---

## ▶️ Run Spotlight-Bot

```bash
python spotlight_bot.py --input data/usage_data.json --output data/usage_visualization.png
