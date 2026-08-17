<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>

<body>

<h1>Agentic Product Research System</h1>

<p>
An AI-powered <strong>multi-agent product research system</strong> built with
<strong>CrewAI</strong>. The system takes a user's buying request, researches
products across the web, analyzes the best options, and generates an
<strong>HTML report with the Top 5 recommendations</strong>.
</p>

<h2>How It Works</h2>

<p>
You simply tell the system what you want to buy, for example:
</p>

<blockquote>
    I want to buy a coffee machine for the office.
</blockquote>

<p>The agents automatically:</p>

<ol>
    <li>Generate optimized search queries.</li>
    <li>Search the web for suitable coffee machines.</li>
    <li>Investigate the most promising products in detail.</li>
    <li>Compare the results and recommend the Top 5.</li>
    <li>Generate a final HTML report.</li>
</ol>

<h2>Multi-Agent Architecture</h2>

<table>
    <tr>
        <th>Agent</th>
        <th>Responsibility</th>
        <th>Tools</th>
    </tr>
    <tr>
        <td>🔎 Search Query Agent</td>
        <td>Converts the user's requirements into optimized search queries.</td>
        <td>Gemini or Ollama LLM</td>
    </tr>
    <tr>
        <td>🌐 Product Search Agent</td>
        <td>Searches the web and finds relevant products.</td>
        <td>Tavily</td>
    </tr>
    <tr>
        <td>🕷️ Product Details Agent</td>
        <td>Scrapes and extracts detailed information about the best products.</td>
        <td>ScrapeGraphAI</td>
    </tr>
    <tr>
        <td>📊 Report Agent</td>
        <td>Analyzes the products, compares them, and generates the Top 5 recommendations.</td>
        <td>Gemini or Ollama LLM</td>
    </tr>
</table>

<h2>Workflow Example</h2>

<pre>
User
  │
  │ "I need a coffee machine for the office"
  ▼
┌─────────────────────────┐
│ 1. Query Generator      │
│ Generates search        │
│ queries                 │
└────────────┬────────────┘
             ▼
┌─────────────────────────┐
│ 2. Product Search       │
│ Searches the web        │
│ using Tavily            │
└────────────┬────────────┘
             ▼
┌─────────────────────────┐
│ 3. Product Research     │
│ Scrapes product pages   │
│ using ScrapeGraphAI     │
└────────────┬────────────┘
             ▼
┌─────────────────────────┐
│ 4. Report Generator     │
│ Compares products and   │
│ selects Top 5           │
└────────────┬────────────┘
             ▼
       HTML Report
</pre>

<h2>Technologies</h2>

<ul>
    <li><strong>CrewAI</strong> — Multi-agent orchestration</li>
    <li><strong>AgentOps</strong> — Agent monitoring and observability</li>
    <li><strong>Tavily</strong> — Web search</li>
    <li><strong>ScrapeGraphAI</strong> — Web scraping and information extraction</li>
    <li><strong>Gemini</strong> — Cloud LLM</li>
    <li><strong>Ollama</strong> — Local LLM option</li>
    <li><strong>Pydantic</strong> — Structured data validation and management</li>
    <li><strong>Python</strong> — Core language</li>
    <li><strong>Jupyter Notebook</strong> — Complete implementation</li>
</ul>

<h2>Example</h2>

<p>
For a request such as:
</p>

<blockquote>
    <strong>"Find the best coffee machine for our office."</strong>
</blockquote>

<p>
The system researches different machines, gathers specifications,
prices, features, reviews and other relevant information, then produces
a report similar to:
</p>

<ol>
    <li>🏆 Best Overall Coffee Machine</li>
    <li>💰 Best Value</li>
    <li>☕ Best for Large Offices</li>
    <li>⚡ Best for Convenience</li>
    <li>💎 Premium Choice</li>
</ol>

<p>
The final report contains the researched products, detailed information,
comparison results, and the <strong>Top 5 recommendations</strong>.
</p>

<h2>LLM Options</h2>

<p>
The notebook supports two approaches:
</p>

<ul>
    <li>☁️ <strong>Gemini</strong> for cloud-based inference.</li>
    <li>🖥️ <strong>Ollama</strong> for running an LLM locally.</li>
</ul>

<p>
This makes it possible to switch between cloud and local models depending
on the user's requirements.
</p>

<h2>Monitoring</h2>

<p>
<strong>AgentOps</strong> is integrated to monitor the agentic workflow,
including agent executions, LLM calls, tool usage and overall task
performance.
</p>

<h2>Goal</h2>

<p>
This project demonstrates how specialized AI agents can collaborate with
external tools to perform a complete real-world research task:
</p>

<p>
<strong>Plan → Search → Investigate → Analyze → Recommend → Report</strong>
</p>

</body>
</html>
