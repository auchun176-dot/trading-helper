# trading-helper
# 1. 创建并激活虚拟环境（推荐）
python -m venv .venv
source .venv/bin/activate  # Windows 用 .venv\Scripts\activate

# 2. 安装 Vibe-Trading（PyPI 包名是 vibe-trading-ai）
pip install vibe-trading-ai

# 3. 交互式初始化配置
vibe-trading init
OPENAI_API_KEY=sk-...
# 或 ANTHROPIC_API_KEY=sk-ant-...
# 如需代理
HTTPS_PROXY=http://127.0.0.1:7890
vibe-trading run -p "Backtest a BTC-USDT 20/50 moving-average strategy for 2024, summarize return and drawdown, then export the report"
