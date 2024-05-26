# Comparing `tmp/scrapegraphai-1.5.0b3.tar.gz` & `tmp/scrapegraphai-1.5.0b4.tar.gz`

## Comparing `scrapegraphai-1.5.0b3.tar` & `scrapegraphai-1.5.0b4.tar`

### file list

```diff
@@ -1,276 +1,284 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.gitattributes
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.releaserc.yml
--rw-r--r--   0        0        0    47020 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/CHANGELOG.md
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/CONTRIBUTING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/Dockerfile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/SECURITY.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/citation.cff
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docker-compose.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/readthedocs.yml
--rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements-dev.lock
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements-dev.txt
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements.lock
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.github/workflows/release.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/Makefile
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/make.bat
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_1.png
--rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_2.png
--rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_3.png
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/apikey_4.png
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/codespaces-badge.png
--rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/logo_authors.png
--rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/omniscrapergraph.png
--rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/omnisearchgraph.png
--rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.fig
--rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/scrapegraphai_logo.png
--rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/searchgraph.png
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/serp_api_logo.png
--rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/smartscrapergraph.png
--rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/speechgraph.png
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/assets/transparent_stat.png
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/conf.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/index.rst
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/getting_started/examples.rst
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/introduction/contributing.rst
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/introduction/overview.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/modules.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.graphs.rst
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.nodes.rst
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/benchmarks.rst
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/graph_config.rst
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/graphs.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/docs/source/scrapers/llm.rst
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/readme.md
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/anthropic/smart_scraper_haiku.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/json_scraper_azure.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/search_graph_azure.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/smart_scraper_azure_openai.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/xml_scraper_azure.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/azure/inputs/username.csv
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/.env.example
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/README.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/csv_scraper_bedrock.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/custom_graph_bedrock.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/json_scraper_bedrock.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/scrape_plain_text_bedrock.py
--rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/scrapegraphai_bedrock.png
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/script_generator_bedrock.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/search_graph_bedrock.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/smart_scraper_bedrock.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/xml_scraper_bedrock.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/books.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/bedrock/inputs/username.csv
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/readme.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/.env.example
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/.env.example
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/Readme.md
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/.env.example
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/csv_scraper_deepseek.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/json_scraper_deepseek.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/script_generator_deepseek.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/search_graph_deepseek.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/smart_scarper_deepseek.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/xml_scraper_deepseek.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/deepseek/inputs/username.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/.env.example
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/csv_scraper_gemini.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/custom_graph_gemini.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/json_scraper_gemini.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/readme.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/scrape_plain_text_gemini.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/scrape_xml_gemini.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/script_generator_gemini.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/search_graph_gemini.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/smart_scraper_gemini.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/gemini/inputs/username.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/.env.example
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/search_graph_groq_openai.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_ollama.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_openai.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/huggingfacehub/smart_scraper_huggingfacehub.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/csv_scraper_ollama.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/json_scraper_ollama.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/scrape_plain_text_ollama.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/scrape_xml_ollama.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/script_generator_ollama.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/search_graph_ollama.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/smart_scraper_ollama.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/xml_scraper_ollama.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/local_models/inputs/username.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/.env.example
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/readme.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/search_graph_groq_ollama.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/smart_scraper_mixed.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/mixed_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/.env.example
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/csv_scraper_openai.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/custom_graph_openai.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/deep_scraper_openai.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/json_scraper_openai.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/omni_scraper_openai.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/omni_search_graph_openai.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/pdf_scraper_openai.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/readme.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/scrape_plain_text_openai.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/script_generator_openai.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/search_graph_openai.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/smart_scraper_multi_openai.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/smart_scraper_openai.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/smart_scraper_schema_openai.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/speech_graph_openai.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/openai/inputs/username.csv
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/fetch_node.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/image2text_node.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/kg_node.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/examples/single_node/robot_node.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/commit_and_push.sh
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/commit_and_push_with_tests.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/deploy_on_pip.sh
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/manual deployment/installation.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/docloaders/__init__.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/docloaders/chromium.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/deep_scraper_graph.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_scraper_graph.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_search_graph.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_multi_graph.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_prompts.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/anthropic.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/deepseek.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_omni_node.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_node_with_context.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/cleanup_html.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/logging.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/sys_dynamic_import.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/Readme.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_json_ollama.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_llama3_test.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_mistral_test.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/scrape_xml_ollama_test.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/script_generator_test.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/smart_scraper_ollama_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/graphs/inputs/username.csv
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/fetch_node_test.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/robot_node_test.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/search_link_node_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/nodes/inputs/username.csv
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/utils/test_proxy_rotation.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/tests/utils/test_sys_dynamic_import.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/LICENSE
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/README.md
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/pyproject.toml
--rw-r--r--   0        0        0    10804 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.gitattributes
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.releaserc.yml
+-rw-r--r--   0        0        0    48115 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/CHANGELOG.md
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/Dockerfile
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/SECURITY.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/citation.cff
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docker-compose.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/readthedocs.yml
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements-dev.lock
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements-dev.txt
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements.lock
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/Makefile
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/make.bat
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_1.png
+-rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_2.png
+-rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_3.png
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_4.png
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/codespaces-badge.png
+-rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/logo_authors.png
+-rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/omniscrapergraph.png
+-rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/omnisearchgraph.png
+-rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.fig
+-rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/scrapegraphai_logo.png
+-rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/searchgraph.png
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/serp_api_logo.png
+-rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/smartscrapergraph.png
+-rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/speechgraph.png
+-rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/transparent_stat.png
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/conf.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/index.rst
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/getting_started/examples.rst
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/introduction/contributing.rst
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/introduction/overview.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/modules.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.builders.rst
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.docloaders.rst
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.graphs.rst
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.helpers.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.integrations.rst
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.models.rst
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.nodes.rst
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.rst
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.utils.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/benchmarks.rst
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/graph_config.rst
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/graphs.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/llm.rst
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/readme.md
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/anthropic/smart_scraper_haiku.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/json_scraper_azure.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/search_graph_azure.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/smart_scraper_azure_openai.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/xml_scraper_azure.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/inputs/username.csv
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/.env.example
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/README.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/csv_scraper_bedrock.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/custom_graph_bedrock.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/json_scraper_bedrock.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/scrape_plain_text_bedrock.py
+-rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/scrapegraphai_bedrock.png
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/script_generator_bedrock.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/search_graph_bedrock.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/smart_scraper_bedrock.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/xml_scraper_bedrock.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/books.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/username.csv
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/readme.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/.env.example
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/.env.example
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/Readme.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/.env.example
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/csv_scraper_deepseek.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/json_scraper_deepseek.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/script_generator_deepseek.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/search_graph_deepseek.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/smart_scarper_deepseek.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/xml_scraper_deepseek.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/.env.example
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/csv_scraper_gemini.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/custom_graph_gemini.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/json_scraper_gemini.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/readme.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/scrape_plain_text_gemini.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/scrape_xml_gemini.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/script_generator_gemini.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/search_graph_gemini.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/smart_scraper_gemini.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/username.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/.env.example
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/search_graph_groq_openai.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_ollama.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_openai.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/huggingfacehub/smart_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/csv_scraper_ollama.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/json_scraper_ollama.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/scrape_plain_text_ollama.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/scrape_xml_ollama.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/script_generator_ollama.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/search_graph_ollama.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/smart_scraper_ollama.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/xml_scraper_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/username.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/.env.example
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/readme.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/search_graph_groq_ollama.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/smart_scraper_mixed.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/.env.example
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/csv_scraper_openai.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/custom_graph_openai.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/deep_scraper_openai.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/json_scraper_openai.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/omni_scraper_openai.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/omni_search_graph_openai.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/pdf_scraper_openai.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/readme.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/scrape_plain_text_openai.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/script_generator_openai.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/search_graph_openai.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/smart_scraper_multi_openai.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/smart_scraper_openai.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/smart_scraper_schema_openai.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/speech_graph_openai.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/username.csv
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/fetch_node.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/image2text_node.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/kg_node.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/robot_node.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/commit_and_push.sh
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/commit_and_push_with_tests.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/deploy_on_pip.sh
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/installation.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/docloaders/__init__.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/docloaders/chromium.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    15389 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/deep_scraper_graph.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_scraper_graph.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_search_graph.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_multi_graph.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_prompts.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/integrations/__init__.py
+-rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/integrations/burr_bridge.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/anthropic.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/deepseek.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_omni_node.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_node_with_context.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/cleanup_html.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/logging.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/sys_dynamic_import.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/Readme.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_json_ollama.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_llama3_test.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_mistral_test.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_xml_ollama_test.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/script_generator_test.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/smart_scraper_ollama_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/username.csv
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/fetch_node_test.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/robot_node_test.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/search_link_node_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/username.csv
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/utils/test_proxy_rotation.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/utils/test_sys_dynamic_import.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/LICENSE
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/README.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/pyproject.toml
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/PKG-INFO
```

### Comparing `scrapegraphai-1.5.0b3/.releaserc.yml` & `scrapegraphai-1.5.0b4/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/CHANGELOG.md` & `scrapegraphai-1.5.0b4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## [1.5.0-beta.4](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.0-beta.3...v1.5.0-beta.4) (2024-05-25)
+
+
+### Features
+
+* **burr:** added burr integration in graphs and optional burr installation ([ac10128](https://github.com/VinciGit00/Scrapegraph-ai/commit/ac10128ff3af35c52b48c79d085e458524e8e48a))
+* **burr-bridge:** BurrBridge class to integrate inside BaseGraph ([6cbd84f](https://github.com/VinciGit00/Scrapegraph-ai/commit/6cbd84f254ebc1f1c68699273bdd8fcdb0fe26d4))
+* **burr:** first burr integration and docs ([19b27bb](https://github.com/VinciGit00/Scrapegraph-ai/commit/19b27bbe852f134cf239fc1945e7906bc24d7098))
+* **burr-node:** working burr bridge ([654a042](https://github.com/VinciGit00/Scrapegraph-ai/commit/654a04239640a89d9fa408ccb2e4485247ab84df))
+
+
+### Docs
+
+* **burr:** added dependecies and switched to furo ([819f071](https://github.com/VinciGit00/Scrapegraph-ai/commit/819f071f2dc64d090cb05c3571aff6c9cb9196d7))
+* **graph:** added new graphs and schema ([d27cad5](https://github.com/VinciGit00/Scrapegraph-ai/commit/d27cad591196b932c1bbcbaa936479a030ac67b5))
+
 ## [1.5.0-beta.3](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.0-beta.2...v1.5.0-beta.3) (2024-05-24)
 
 
 ### Bug Fixes
 
 * **kg:** removed unused nodes and utils ([5684578](https://github.com/VinciGit00/Scrapegraph-ai/commit/5684578fab635e862de58f7847ad736c6a57f766))
```

### Comparing `scrapegraphai-1.5.0b3/CODE_OF_CONDUCT.md` & `scrapegraphai-1.5.0b4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/CONTRIBUTING.md` & `scrapegraphai-1.5.0b4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/readthedocs.yml` & `scrapegraphai-1.5.0b4/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/requirements-dev.lock` & `scrapegraphai-1.5.0b4/requirements.lock`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 -e file:.
 aiohttp==3.9.5
     # via langchain
     # via langchain-community
 aiosignal==1.3.1
     # via aiohttp
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
-anthropic==0.25.9
+anthropic==0.26.1
     # via langchain-anthropic
 anyio==4.3.0
     # via anthropic
     # via groq
     # via httpx
     # via openai
 asttokens==2.4.1
@@ -28,58 +28,60 @@
     # via aiohttp
     # via langchain
 attrs==23.2.0
     # via aiohttp
 beautifulsoup4==4.12.3
     # via google
     # via scrapegraphai
-boto3==1.34.105
+boto3==1.34.110
     # via langchain-aws
-botocore==1.34.105
+botocore==1.34.110
     # via boto3
     # via s3transfer
 cachetools==5.3.3
     # via google-auth
 certifi==2024.2.2
     # via httpcore
     # via httpx
     # via requests
 charset-normalizer==3.3.2
     # via requests
+colorama==0.4.6
+    # via tqdm
 dataclasses-json==0.6.6
     # via langchain
     # via langchain-community
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via langchain-anthropic
 distro==1.9.0
     # via anthropic
     # via groq
     # via openai
 exceptiongroup==1.2.1
     # via anyio
     # via ipython
-    # via pytest
 executing==2.0.1
     # via stack-data
 faiss-cpu==1.8.0
     # via scrapegraphai
 filelock==3.14.0
     # via huggingface-hub
 free-proxy==1.1.1
     # via scrapegraphai
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 fsspec==2024.5.0
+fsspec==2024.5.0
     # via huggingface-hub
 google==3.0.0
     # via scrapegraphai
-google-ai-generativelanguage==0.6.3
+google-ai-generativelanguage==0.6.4
     # via google-generativeai
 google-api-core==2.19.0
     # via google-ai-generativelanguage
     # via google-api-python-client
     # via google-generativeai
 google-api-python-client==2.129.0
     # via google-generativeai
@@ -87,26 +89,27 @@
     # via google-ai-generativelanguage
     # via google-api-core
     # via google-api-python-client
     # via google-auth-httplib2
     # via google-generativeai
 google-auth-httplib2==0.2.0
     # via google-api-python-client
-google-generativeai==0.5.3
+google-generativeai==0.5.4
     # via langchain-google-genai
 googleapis-common-protos==1.63.0
     # via google-api-core
     # via grpcio-status
 graphviz==0.20.3
     # via scrapegraphai
 greenlet==3.0.3
     # via playwright
-groq==0.5.0
+    # via sqlalchemy
+groq==0.7.0
     # via langchain-groq
-grpcio==1.63.0
+grpcio==1.64.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
     # via httpcore
 html2text==2024.2.26
@@ -117,29 +120,23 @@
     # via google-api-python-client
     # via google-auth-httplib2
 httpx==0.27.0
     # via anthropic
     # via groq
     # via openai
     # via yahoo-search-py
-huggingface-hub==0.23.0
+huggingface-hub==0.23.1
     # via tokenizers
 idna==3.7
     # via anyio
     # via httpx
     # via requests
     # via yarl
-iniconfig==2.0.0
-    # via pytest
-ipython==8.24.0
-    # via pyvis
-jedi==0.19.1
-    # via ipython
-jinja2==3.1.4
-    # via pyvis
+jiter==0.1.0
+    # via anthropic
 jmespath==1.0.1
     # via boto3
     # via botocore
 jsonpatch==1.33
     # via langchain
     # via langchain-core
 jsonpickle==3.0.4
@@ -165,17 +162,17 @@
     # via langchain-text-splitters
 langchain-google-genai==1.0.3
     # via scrapegraphai
 langchain-groq==0.1.3
     # via scrapegraphai
 langchain-openai==0.1.6
     # via scrapegraphai
-langchain-text-splitters==0.0.1
+langchain-text-splitters==0.0.2
     # via langchain
-langsmith==0.1.58
+langsmith==0.1.60
     # via langchain
     # via langchain-community
     # via langchain-core
 lxml==5.2.2
     # via free-proxy
 markupsafe==2.1.5
     # via jinja2
@@ -203,26 +200,23 @@
     # via langchain-openai
 orjson==3.10.3
     # via langsmith
 packaging==23.2
     # via huggingface-hub
     # via langchain-core
     # via marshmallow
-    # via pytest
 pandas==2.2.2
     # via scrapegraphai
 parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 playwright==1.43.0
     # via scrapegraphai
     # via undetected-playwright
-pluggy==1.5.0
-    # via pytest
 prompt-toolkit==3.0.43
     # via ipython
 proto-plus==1.23.0
     # via google-ai-generativelanguage
     # via google-api-core
 protobuf==4.25.3
     # via google-ai-generativelanguage
@@ -253,34 +247,31 @@
     # via pydantic
 pyee==11.1.0
     # via playwright
 pygments==2.18.0
     # via ipython
 pyparsing==3.1.2
     # via httplib2
-pytest==8.0.0
-    # via pytest-mock
-pytest-mock==3.14.0
 python-dateutil==2.9.0.post0
     # via botocore
     # via pandas
 python-dotenv==1.0.1
     # via scrapegraphai
 pytz==2024.1
     # via pandas
 pyvis==0.3.2
     # via scrapegraphai
 pyyaml==6.0.1
     # via huggingface-hub
     # via langchain
     # via langchain-community
     # via langchain-core
-regex==2024.5.10
+regex==2024.5.15
     # via tiktoken
-requests==2.31.0
+requests==2.32.2
     # via free-proxy
     # via google-api-core
     # via huggingface-hub
     # via langchain
     # via langchain-community
     # via langsmith
     # via tiktoken
@@ -311,16 +302,14 @@
     # via langchain-community
     # via langchain-core
 tiktoken==0.6.0
     # via langchain-openai
     # via scrapegraphai
 tokenizers==0.19.1
     # via anthropic
-tomli==2.0.1
-    # via pytest
 tqdm==4.66.4
     # via google-generativeai
     # via huggingface-hub
     # via openai
     # via scrapegraphai
 traitlets==5.14.3
     # via ipython
@@ -343,14 +332,15 @@
 tzdata==2024.1
     # via pandas
 undetected-playwright==0.3.0
     # via scrapegraphai
 uritemplate==4.1.1
     # via google-api-python-client
 urllib3==2.2.1
+urllib3==2.2.1
     # via botocore
     # via requests
     # via yahoo-search-py
 wcwidth==0.2.13
     # via prompt-toolkit
 yahoo-search-py==0.3
     # via scrapegraphai
```

### Comparing `scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/bug_report.md` & `scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/.github/ISSUE_TEMPLATE/feature_request.md` & `scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/.github/workflows/codeql.yml` & `scrapegraphai-1.5.0b4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/.github/workflows/dependency-review.yml` & `scrapegraphai-1.5.0b4/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/.github/workflows/pylint.yml` & `scrapegraphai-1.5.0b4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/.github/workflows/python-publish.yml` & `scrapegraphai-1.5.0b4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/.github/workflows/release.yml` & `scrapegraphai-1.5.0b4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/Makefile` & `scrapegraphai-1.5.0b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/README.md` & `scrapegraphai-1.5.0b4/docs/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/make.bat` & `scrapegraphai-1.5.0b4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/apikey_1.png` & `scrapegraphai-1.5.0b4/docs/assets/apikey_1.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/apikey_2.png` & `scrapegraphai-1.5.0b4/docs/assets/apikey_2.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/apikey_3.png` & `scrapegraphai-1.5.0b4/docs/assets/apikey_3.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/apikey_4.png` & `scrapegraphai-1.5.0b4/docs/assets/apikey_4.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/codespaces-badge.png` & `scrapegraphai-1.5.0b4/docs/assets/codespaces-badge.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/logo_authors.png` & `scrapegraphai-1.5.0b4/docs/assets/logo_authors.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/omniscrapergraph.png` & `scrapegraphai-1.5.0b4/docs/assets/omniscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/omnisearchgraph.png` & `scrapegraphai-1.5.0b4/docs/assets/omnisearchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.fig` & `scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.fig`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/project_overview_diagram.png` & `scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/scrapegraphai_logo.png` & `scrapegraphai-1.5.0b4/docs/assets/scrapegraphai_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/searchgraph.png` & `scrapegraphai-1.5.0b4/docs/assets/searchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/serp_api_logo.png` & `scrapegraphai-1.5.0b4/docs/assets/serp_api_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/smartscrapergraph.png` & `scrapegraphai-1.5.0b4/docs/assets/smartscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/speechgraph.png` & `scrapegraphai-1.5.0b4/docs/assets/speechgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/assets/transparent_stat.png` & `scrapegraphai-1.5.0b4/docs/assets/transparent_stat.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/source/index.rst` & `scrapegraphai-1.5.0b4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/source/getting_started/examples.rst` & `scrapegraphai-1.5.0b4/docs/source/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/source/getting_started/installation.rst` & `scrapegraphai-1.5.0b4/docs/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/source/introduction/contributing.rst` & `scrapegraphai-1.5.0b4/docs/source/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/source/introduction/overview.rst` & `scrapegraphai-1.5.0b4/docs/source/introduction/overview.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.graphs.rst` & `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.graphs.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,133 @@
 scrapegraphai.graphs package
 ============================
 
 Submodules
 ----------
 
+scrapegraphai.graphs.abstract\_graph module
+-------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.abstract_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 scrapegraphai.graphs.base\_graph module
 ---------------------------------------
 
 .. automodule:: scrapegraphai.graphs.base_graph
    :members:
    :undoc-members:
    :show-inheritance:
 
+scrapegraphai.graphs.csv\_scraper\_graph module
+-----------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.csv_scraper_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.deep\_scraper\_graph module
+------------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.deep_scraper_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.json\_scraper\_graph module
+------------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.json_scraper_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.omni\_scraper\_graph module
+------------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.omni_scraper_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.omni\_search\_graph module
+-----------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.omni_search_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.pdf\_scraper\_graph module
+-----------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.pdf_scraper_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.script\_creator\_graph module
+--------------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.script_creator_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.search\_graph module
+-----------------------------------------
+
+.. automodule:: scrapegraphai.graphs.search_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 scrapegraphai.graphs.smart\_scraper\_graph module
 -------------------------------------------------
 
 .. automodule:: scrapegraphai.graphs.smart_scraper_graph
    :members:
    :undoc-members:
    :show-inheritance:
 
+scrapegraphai.graphs.smart\_scraper\_graph\_burr module
+-------------------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.smart_scraper_graph_burr
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.smart\_scraper\_graph\_hamilton module
+-----------------------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.smart_scraper_graph_hamilton
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.speech\_graph module
+-----------------------------------------
+
+.. automodule:: scrapegraphai.graphs.speech_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+scrapegraphai.graphs.xml\_scraper\_graph module
+-----------------------------------------------
+
+.. automodule:: scrapegraphai.graphs.xml_scraper_graph
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: scrapegraphai.graphs
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.nodes.rst` & `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.helpers.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,45 @@
-scrapegraphai.nodes package
-===========================
+scrapegraphai.helpers package
+=============================
 
 Submodules
 ----------
 
-scrapegraphai.nodes.base\_node module
--------------------------------------
+scrapegraphai.helpers.models\_tokens module
+-------------------------------------------
 
-.. automodule:: scrapegraphai.nodes.base_node
+.. automodule:: scrapegraphai.helpers.models_tokens
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.nodes.conditional\_node module
+scrapegraphai.helpers.nodes\_metadata module
 --------------------------------------------
 
-.. automodule:: scrapegraphai.nodes.conditional_node
+.. automodule:: scrapegraphai.helpers.nodes_metadata
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.nodes.fetch\_html\_node module
---------------------------------------------
-
-.. automodule:: scrapegraphai.nodes.fetch_html_node
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-scrapegraphai.nodes.generate\_answer\_node module
--------------------------------------------------
+scrapegraphai.helpers.robots module
+-----------------------------------
 
-.. automodule:: scrapegraphai.nodes.generate_answer_node
+.. automodule:: scrapegraphai.helpers.robots
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.nodes.get\_probable\_tags\_node module
-----------------------------------------------------
-
-.. automodule:: scrapegraphai.nodes.get_probable_tags_node
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-scrapegraphai.nodes.parse\_html\_node module
---------------------------------------------
+scrapegraphai.helpers.schemas module
+------------------------------------
 
-.. automodule:: scrapegraphai.nodes.parse_html_node
+.. automodule:: scrapegraphai.helpers.schemas
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: scrapegraphai.nodes
+.. automodule:: scrapegraphai.helpers
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scrapegraphai-1.5.0b3/docs/source/modules/scrapegraphai.rst` & `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.models.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,101 @@
-scrapegraphai package
-=====================
-
-Subpackages
------------
-
-.. toctree::
-   :maxdepth: 4
-
-   scrapegraphai.graphs
-   scrapegraphai.nodes
+scrapegraphai.models package
+============================
 
 Submodules
 ----------
 
-scrapegraphai.class\_creator module
------------------------------------
+scrapegraphai.models.anthropic module
+-------------------------------------
 
-.. automodule:: scrapegraphai.class_creator
+.. automodule:: scrapegraphai.models.anthropic
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.class\_generator module
--------------------------------------
+scrapegraphai.models.azure\_openai module
+-----------------------------------------
 
-.. automodule:: scrapegraphai.class_generator
+.. automodule:: scrapegraphai.models.azure_openai
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.convert\_to\_csv module
--------------------------------------
+scrapegraphai.models.bedrock module
+-----------------------------------
 
-.. automodule:: scrapegraphai.convert_to_csv
+.. automodule:: scrapegraphai.models.bedrock
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.convert\_to\_json module
---------------------------------------
+scrapegraphai.models.deepseek module
+------------------------------------
 
-.. automodule:: scrapegraphai.convert_to_json
+.. automodule:: scrapegraphai.models.deepseek
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.dictionaries module
----------------------------------
+scrapegraphai.models.gemini module
+----------------------------------
 
-.. automodule:: scrapegraphai.dictionaries
+.. automodule:: scrapegraphai.models.gemini
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.getter module
----------------------------
+scrapegraphai.models.groq module
+--------------------------------
 
-.. automodule:: scrapegraphai.getter
+.. automodule:: scrapegraphai.models.groq
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.json\_getter module
----------------------------------
+scrapegraphai.models.hugging\_face module
+-----------------------------------------
 
-.. automodule:: scrapegraphai.json_getter
+.. automodule:: scrapegraphai.models.hugging_face
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.pydantic\_class module
-------------------------------------
+scrapegraphai.models.ollama module
+----------------------------------
 
-.. automodule:: scrapegraphai.pydantic_class
+.. automodule:: scrapegraphai.models.ollama
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.remover module
-----------------------------
+scrapegraphai.models.openai module
+----------------------------------
 
-.. automodule:: scrapegraphai.remover
+.. automodule:: scrapegraphai.models.openai
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.request module
-----------------------------
+scrapegraphai.models.openai\_itt module
+---------------------------------------
 
-.. automodule:: scrapegraphai.request
+.. automodule:: scrapegraphai.models.openai_itt
    :members:
    :undoc-members:
    :show-inheritance:
 
-scrapegraphai.token\_calculator module
---------------------------------------
+scrapegraphai.models.openai\_tts module
+---------------------------------------
 
-.. automodule:: scrapegraphai.token_calculator
+.. automodule:: scrapegraphai.models.openai_tts
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: scrapegraphai
+.. automodule:: scrapegraphai.models
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scrapegraphai-1.5.0b3/docs/source/scrapers/benchmarks.rst` & `scrapegraphai-1.5.0b4/docs/source/scrapers/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/docs/source/scrapers/graphs.rst` & `scrapegraphai-1.5.0b4/docs/source/scrapers/graphs.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Graphs
 ======
 
 Graphs are scraping pipelines aimed at solving specific tasks. They are composed by nodes which can be configured individually to address different aspects of the task (fetching data, extracting information, etc.).
 
-There are three types of graphs available in the library:
+There are several types of graphs available in the library, each with its own purpose and functionality. The most common ones are:
 
-- **SmartScraperGraph**: one-page scraper that requires a user-defined prompt and a URL (or local file) to extract information from using LLM.
+- **SmartScraperGraph**: one-page scraper that requires a user-defined prompt and a URL (or local file) to extract information using LLM.
+- **SmartScraperMultiGraph**: multi-page scraper that requires a user-defined prompt and a list of URLs (or local files) to extract information using LLM. It is built on top of SmartScraperGraph.
 - **SearchGraph**: multi-page scraper that only requires a user-defined prompt to extract information from a search engine using LLM. It is built on top of SmartScraperGraph.
 - **SpeechGraph**: text-to-speech pipeline that generates an answer as well as a requested audio file. It is built on top of SmartScraperGraph and requires a user-defined prompt and a URL (or local file).
+- **ScriptCreatorGraph**: script generator that creates a Python script to scrape a website using the specified library (e.g. BeautifulSoup). It requires a user-defined prompt and a URL (or local file).
 
 With the introduction of `GPT-4o`, two new powerful graphs have been created:
 
 - **OmniScraperGraph**: similar to `SmartScraperGraph`, but with the ability to scrape images and describe them.
 - **OmniSearchGraph**: similar to `SearchGraph`, but with the ability to scrape images and describe them.
 
+
 .. note::
 
    They all use a graph configuration to set up LLM models and other parameters. To find out more about the configurations, check the :ref:`LLM` and :ref:`Configuration` sections.
 
+
+.. note::
+
+   We can pass an optional `schema` parameter to the graph constructor to specify the output schema. If not provided or set to `None`, the schema will be generated by the LLM itself.
+
 OmniScraperGraph
 ^^^^^^^^^^^^^^^^
 
 .. image:: ../../assets/omniscrapergraph.png
    :align: center
    :width: 90%
    :alt: OmniScraperGraph
@@ -37,15 +45,16 @@
    graph_config = {
       "llm": {...},
    }
 
    omni_scraper_graph = OmniScraperGraph(
       prompt="List me all the projects with their titles and image links and descriptions.",
       source="https://perinim.github.io/projects",
-      config=graph_config
+      config=graph_config,
+      schema=schema
    )
 
    result = omni_scraper_graph.run()
    print(result)
 
 OmniSearchGraph
 ^^^^^^^^^^^^^^^
@@ -66,23 +75,24 @@
    graph_config = {
       "llm": {...},
    }
 
    # Create the OmniSearchGraph instance
    omni_search_graph = OmniSearchGraph(
       prompt="List me all Chioggia's famous dishes and describe their pictures.",
-      config=graph_config
+      config=graph_config,
+      schema=schema
    )
 
    # Run the graph
    result = omni_search_graph.run()
    print(result)
 
-SmartScraperGraph
-^^^^^^^^^^^^^^^^^
+SmartScraperGraph & SmartScraperMultiGraph
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. image:: ../../assets/smartscrapergraph.png
    :align: center
    :width: 90%
    :alt: SmartScraperGraph
 |
 
@@ -96,20 +106,22 @@
    graph_config = {
       "llm": {...},
    }
 
    smart_scraper_graph = SmartScraperGraph(
       prompt="List me all the projects with their descriptions",
       source="https://perinim.github.io/projects",
-      config=graph_config
+      config=graph_config,
+      schema=schema
    )
 
    result = smart_scraper_graph.run()
    print(result)
 
+**SmartScraperMultiGraph** is similar to SmartScraperGraph, but it can handle multiple sources. We define the graph configuration, create an instance of the SmartScraperMultiGraph class, and run the graph.
 
 SearchGraph
 ^^^^^^^^^^^
 
 .. image:: ../../assets/searchgraph.png
    :align: center
    :width: 80%
@@ -128,15 +140,16 @@
       "llm": {...},
       "embeddings": {...},
    }
 
    # Create the SearchGraph instance
    search_graph = SearchGraph(
       prompt="List me all the traditional recipes from Chioggia",
-      config=graph_config
+      config=graph_config,
+      schema=schema
    )
 
    # Run the graph
    result = search_graph.run()
    print(result)
 
 
@@ -165,11 +178,12 @@
    # Create the SpeechGraph instance and run it
    # ************************************************
 
    speech_graph = SpeechGraph(
       prompt="Make a detailed audio summary of the projects.",
       source="https://perinim.github.io/projects/",
       config=graph_config,
+      schema=schema
    )
 
    result = speech_graph.run()
    print(result)
```

### Comparing `scrapegraphai-1.5.0b3/docs/source/scrapers/llm.rst` & `scrapegraphai-1.5.0b4/docs/source/scrapers/llm.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/readme.md` & `scrapegraphai-1.5.0b4/examples/readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/anthropic/smart_scraper_haiku.py` & `scrapegraphai-1.5.0b4/examples/anthropic/smart_scraper_haiku.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/azure/json_scraper_azure.py` & `scrapegraphai-1.5.0b4/examples/azure/json_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/azure/search_graph_azure.py` & `scrapegraphai-1.5.0b4/examples/azure/search_graph_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/azure/smart_scraper_azure_openai.py` & `scrapegraphai-1.5.0b4/examples/azure/smart_scraper_azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/azure/xml_scraper_azure.py` & `scrapegraphai-1.5.0b4/examples/azure/xml_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/azure/inputs/books.xml` & `scrapegraphai-1.5.0b4/examples/azure/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/azure/inputs/example.json` & `scrapegraphai-1.5.0b4/examples/azure/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/csv_scraper_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/csv_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/custom_graph_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/custom_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/json_scraper_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/json_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/scrape_plain_text_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/scrape_plain_text_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/scrapegraphai_bedrock.png` & `scrapegraphai-1.5.0b4/examples/bedrock/scrapegraphai_bedrock.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/script_generator_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/script_generator_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/search_graph_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/search_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/smart_scraper_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/smart_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/xml_scraper_bedrock.py` & `scrapegraphai-1.5.0b4/examples/bedrock/xml_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/inputs/books.xml` & `scrapegraphai-1.5.0b4/examples/bedrock/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/inputs/example.json` & `scrapegraphai-1.5.0b4/examples/bedrock/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/bedrock/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b4/examples/bedrock/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/Readme.md` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/GenerateScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/Readme.md` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_docker.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_docker.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/benchmarks/SmartScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/csv_scraper_deepseek.py` & `scrapegraphai-1.5.0b4/examples/deepseek/csv_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/json_scraper_deepseek.py` & `scrapegraphai-1.5.0b4/examples/deepseek/json_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/script_generator_deepseek.py` & `scrapegraphai-1.5.0b4/examples/deepseek/script_generator_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/search_graph_deepseek.py` & `scrapegraphai-1.5.0b4/examples/deepseek/search_graph_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/smart_scarper_deepseek.py` & `scrapegraphai-1.5.0b4/examples/deepseek/smart_scarper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/xml_scraper_deepseek.py` & `scrapegraphai-1.5.0b4/examples/deepseek/xml_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/inputs/books.xml` & `scrapegraphai-1.5.0b4/examples/deepseek/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/deepseek/inputs/example.json` & `scrapegraphai-1.5.0b4/examples/deepseek/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/csv_scraper_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/csv_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/custom_graph_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/custom_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/json_scraper_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/json_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/scrape_plain_text_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/scrape_plain_text_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/scrape_xml_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/scrape_xml_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/script_generator_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/script_generator_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/search_graph_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/search_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/smart_scraper_gemini.py` & `scrapegraphai-1.5.0b4/examples/gemini/smart_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/xml_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/gemini/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/inputs/books.xml` & `scrapegraphai-1.5.0b4/examples/gemini/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/inputs/example.json` & `scrapegraphai-1.5.0b4/examples/gemini/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/gemini/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b4/examples/gemini/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/groq/search_graph_groq_openai.py` & `scrapegraphai-1.5.0b4/examples/groq/search_graph_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_ollama.py` & `scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/groq/smart_scraper_groq_openai.py` & `scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/huggingfacehub/smart_scraper_huggingfacehub.py` & `scrapegraphai-1.5.0b4/examples/huggingfacehub/smart_scraper_huggingfacehub.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/csv_scraper_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/csv_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/json_scraper_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/json_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/scrape_plain_text_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/scrape_plain_text_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/scrape_xml_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/scrape_xml_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/script_generator_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/script_generator_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/search_graph_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/search_graph_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/smart_scraper_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/smart_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/xml_scraper_ollama.py` & `scrapegraphai-1.5.0b4/examples/local_models/xml_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/inputs/books.xml` & `scrapegraphai-1.5.0b4/examples/local_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/inputs/example.json` & `scrapegraphai-1.5.0b4/examples/local_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/local_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b4/examples/local_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/mixed_models/search_graph_groq_ollama.py` & `scrapegraphai-1.5.0b4/examples/mixed_models/search_graph_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/mixed_models/smart_scraper_mixed.py` & `scrapegraphai-1.5.0b4/examples/mixed_models/smart_scraper_mixed.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/mixed_models/inputs/books.xml` & `scrapegraphai-1.5.0b4/examples/mixed_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/mixed_models/inputs/example.json` & `scrapegraphai-1.5.0b4/examples/mixed_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/mixed_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b4/examples/mixed_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/csv_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/csv_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/custom_graph_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/custom_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/deep_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/deep_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/json_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/json_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/omni_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/omni_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/omni_search_graph_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/omni_search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/pdf_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/pdf_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/scrape_plain_text_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/scrape_plain_text_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/script_generator_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/script_generator_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/search_graph_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/smart_scraper_multi_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/smart_scraper_multi_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/smart_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/smart_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/smart_scraper_schema_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/smart_scraper_schema_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/speech_graph_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/speech_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/xml_scraper_openai.py` & `scrapegraphai-1.5.0b4/examples/openai/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/inputs/books.xml` & `scrapegraphai-1.5.0b4/examples/openai/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/inputs/example.json` & `scrapegraphai-1.5.0b4/examples/openai/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/openai/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b4/examples/openai/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/single_node/fetch_node.py` & `scrapegraphai-1.5.0b4/examples/single_node/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/single_node/image2text_node.py` & `scrapegraphai-1.5.0b4/examples/single_node/image2text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/single_node/kg_node.py` & `scrapegraphai-1.5.0b4/examples/single_node/kg_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/examples/single_node/robot_node.py` & `scrapegraphai-1.5.0b4/examples/single_node/robot_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/manual deployment/commit_and_push.sh` & `scrapegraphai-1.5.0b4/manual deployment/commit_and_push.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/manual deployment/commit_and_push_with_tests.sh` & `scrapegraphai-1.5.0b4/manual deployment/commit_and_push_with_tests.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-1.5.0b4/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/docloaders/chromium.py` & `scrapegraphai-1.5.0b4/scrapegraphai/docloaders/chromium.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/__init__.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/abstract_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 AbstractGraph Module
 """
 
 from abc import ABC, abstractmethod
 from typing import Optional
+import uuid
 
 from langchain_aws import BedrockEmbeddings
 from langchain_community.embeddings import HuggingFaceHubEmbeddings, OllamaEmbeddings
 from langchain_google_genai import GoogleGenerativeAIEmbeddings
 from langchain_google_genai.embeddings import GoogleGenerativeAIEmbeddings
 from langchain_openai import AzureOpenAIEmbeddings, OpenAIEmbeddings
 
@@ -97,14 +98,24 @@
             "loader_kwargs": self.loader_kwargs,
             "llm_model": self.llm_model,
             "embedder_model": self.embedder_model
             }
         
         self.set_common_params(common_params, overwrite=False)
 
+        # set burr config
+        self.burr_kwargs = config.get("burr_kwargs", None)
+        if self.burr_kwargs is not None:
+            self.graph.use_burr = True
+            if "app_instance_id" not in self.burr_kwargs:
+                # set a random uuid for the app_instance_id to avoid conflicts
+                self.burr_kwargs["app_instance_id"] = str(uuid.uuid4())
+
+            self.graph.burr_config = self.burr_kwargs
+
     def set_common_params(self, params: dict, overwrite=False):
         """
         Pass parameters to every node in the graph unless otherwise defined in the graph.
 
         Args:
             params (dict): Common parameters and their values.
         """
```

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/base_graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,28 +36,35 @@
         ...        generate_answer_node,
         ...    ],
         ...    edges=[
         ...        (fetch_node, parse_node),
         ...        (parse_node, rag_node),
         ...        (rag_node, generate_answer_node)
         ...    ],
-        ...    entry_point=fetch_node
+        ...    entry_point=fetch_node,
+        ...    use_burr=True,
+        ...    burr_config={"app_instance_id": "example-instance"}
         ... )
     """
 
-    def __init__(self, nodes: list, edges: list, entry_point: str):
+    def __init__(self, nodes: list, edges: list, entry_point: str, use_burr: bool = False, burr_config: dict = None):
 
         self.nodes = nodes
         self.edges = self._create_edges({e for e in edges})
         self.entry_point = entry_point.node_name
+        self.initial_state = {}
 
         if nodes[0].node_name != entry_point.node_name:
             # raise a warning if the entry point is not the first node in the list
             warnings.warn(
                 "Careful! The entry point node is different from the first node if the graph.")
+        
+        # Burr configuration
+        self.use_burr = use_burr
+        self.burr_config = burr_config or {}
 
     def _create_edges(self, edges: list) -> dict:
         """
         Helper method to create a dictionary of edges from the given iterable of tuples.
 
         Args:
             edges (iterable): An iterable of tuples representing the directed edges.
@@ -67,82 +74,98 @@
         """
 
         edge_dict = {}
         for from_node, to_node in edges:
             edge_dict[from_node.node_name] = to_node.node_name
         return edge_dict
 
-    def execute(self, initial_state: dict) -> Tuple[dict, list]:
+    def _execute_standard(self, initial_state: dict) -> Tuple[dict, list]:
         """
-        Executes the graph by traversing nodes starting from the entry point. The execution
-        follows the edges based on the result of each node's execution and continues until
-        it reaches a node with no outgoing edges.
+        Executes the graph by traversing nodes starting from the entry point using the standard method.
 
         Args:
             initial_state (dict): The initial state to pass to the entry point node.
 
         Returns:
             Tuple[dict, list]: A tuple containing the final state and a list of execution info.
         """
-
-        current_node_name = self.nodes[0]
+        current_node_name = self.entry_point
         state = initial_state
 
         # variables for tracking execution info
         total_exec_time = 0.0
         exec_info = []
         cb_total = {
             "total_tokens": 0,
             "prompt_tokens": 0,
             "completion_tokens": 0,
             "successful_requests": 0,
             "total_cost_USD": 0.0,
         }
 
-        for index in self.nodes:
-
+        while current_node_name:
             curr_time = time.time()
-            current_node = index
+            current_node = next(node for node in self.nodes if node.node_name == current_node_name)
 
             with get_openai_callback() as cb:
                 result = current_node.execute(state)
                 node_exec_time = time.time() - curr_time
                 total_exec_time += node_exec_time
 
-                cb = {
-                    "node_name": index.node_name,
+                cb_data = {
+                    "node_name": current_node.node_name,
                     "total_tokens": cb.total_tokens,
                     "prompt_tokens": cb.prompt_tokens,
                     "completion_tokens": cb.completion_tokens,
                     "successful_requests": cb.successful_requests,
                     "total_cost_USD": cb.total_cost,
                     "exec_time": node_exec_time,
                 }
 
-                exec_info.append(
-                    cb
-                )
-
-                cb_total["total_tokens"] += cb["total_tokens"]
-                cb_total["prompt_tokens"] += cb["prompt_tokens"]
-                cb_total["completion_tokens"] += cb["completion_tokens"]
-                cb_total["successful_requests"] += cb["successful_requests"]
-                cb_total["total_cost_USD"] += cb["total_cost_USD"]
+                exec_info.append(cb_data)
+
+                cb_total["total_tokens"] += cb_data["total_tokens"]
+                cb_total["prompt_tokens"] += cb_data["prompt_tokens"]
+                cb_total["completion_tokens"] += cb_data["completion_tokens"]
+                cb_total["successful_requests"] += cb_data["successful_requests"]
+                cb_total["total_cost_USD"] += cb_data["total_cost_USD"]
 
             if current_node.node_type == "conditional_node":
                 current_node_name = result
             elif current_node_name in self.edges:
                 current_node_name = self.edges[current_node_name]
             else:
                 current_node_name = None
 
         exec_info.append({
             "node_name": "TOTAL RESULT",
-            "total_tokens":  cb_total["total_tokens"],
-            "prompt_tokens":  cb_total["prompt_tokens"],
+            "total_tokens": cb_total["total_tokens"],
+            "prompt_tokens": cb_total["prompt_tokens"],
             "completion_tokens": cb_total["completion_tokens"],
             "successful_requests": cb_total["successful_requests"],
-            "total_cost_USD":   cb_total["total_cost_USD"],
+            "total_cost_USD": cb_total["total_cost_USD"],
             "exec_time": total_exec_time,
         })
 
-        return state, exec_info
+        return state, exec_info
+
+    def execute(self, initial_state: dict) -> Tuple[dict, list]:
+        """
+        Executes the graph by either using BurrBridge or the standard method.
+
+        Args:
+            initial_state (dict): The initial state to pass to the entry point node.
+
+        Returns:
+            Tuple[dict, list]: A tuple containing the final state and a list of execution info.
+        """
+
+        self.initial_state = initial_state
+        if self.use_burr:
+
+            from ..integrations import BurrBridge
+            
+            bridge = BurrBridge(self, self.burr_config)
+            result = bridge.execute(initial_state)
+            return (result["_state"], [])
+        else:
+            return self._execute_standard(initial_state)
```

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/deep_scraper_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/deep_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_scraper_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/omni_search_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/smart_scraper_multi_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_multi_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-1.5.0b4/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/__init__.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_csv_prompts.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_csv_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_omni_prompts.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_omni_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/generate_answer_node_prompts.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/helpers/schemas.py` & `scrapegraphai-1.5.0b4/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/models/bedrock.py` & `scrapegraphai-1.5.0b4/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/models/gemini.py` & `scrapegraphai-1.5.0b4/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/models/openai_itt.py` & `scrapegraphai-1.5.0b4/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/models/openai_tts.py` & `scrapegraphai-1.5.0b4/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/__init__.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/base_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_omni_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_omni_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/search_node_with_context.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_node_with_context.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-1.5.0b4/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/cleanup_html.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/cleanup_html.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/logging.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/research_web.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/sys_dynamic_import.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-1.5.0b4/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/scrape_json_ollama.py` & `scrapegraphai-1.5.0b4/tests/graphs/scrape_json_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_llama3_test.py` & `scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_llama3_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/scrape_plain_text_mistral_test.py` & `scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_mistral_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/scrape_xml_ollama_test.py` & `scrapegraphai-1.5.0b4/tests/graphs/scrape_xml_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/script_generator_test.py` & `scrapegraphai-1.5.0b4/tests/graphs/script_generator_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/smart_scraper_ollama_test.py` & `scrapegraphai-1.5.0b4/tests/graphs/smart_scraper_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/inputs/books.xml` & `scrapegraphai-1.5.0b4/tests/graphs/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/inputs/example.json` & `scrapegraphai-1.5.0b4/tests/graphs/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/graphs/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b4/tests/graphs/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/nodes/fetch_node_test.py` & `scrapegraphai-1.5.0b4/tests/nodes/fetch_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/nodes/robot_node_test.py` & `scrapegraphai-1.5.0b4/tests/nodes/robot_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/nodes/search_link_node_test.py` & `scrapegraphai-1.5.0b4/tests/nodes/search_link_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/nodes/inputs/books.xml` & `scrapegraphai-1.5.0b4/tests/nodes/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/nodes/inputs/example.json` & `scrapegraphai-1.5.0b4/tests/nodes/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/nodes/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b4/tests/nodes/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/utils/test_proxy_rotation.py` & `scrapegraphai-1.5.0b4/tests/utils/test_proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/tests/utils/test_sys_dynamic_import.py` & `scrapegraphai-1.5.0b4/tests/utils/test_sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/LICENSE` & `scrapegraphai-1.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/README.md` & `scrapegraphai-1.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b3/pyproject.toml` & `scrapegraphai-1.5.0b4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [project]
 name = "scrapegraphai"
 
 
-version = "1.5.0b3"
+version = "1.5.0b4"
 
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     { name = "Marco Vinciguerra", email = "mvincig11@gmail.com" },
     { name = "Marco Perini", email = "perinim.98@gmail.com" },
     { name = "Lorenzo Padoan", email = "lorenzo.padoan977@gmail.com" }
 ]
 dependencies = [
-    # python = ">=3.9, <3.12"
     "langchain==0.1.15",
     "langchain-openai==0.1.6",
     "langchain-google-genai==1.0.3",
     "langchain-groq==0.1.3",
     "langchain-aws==0.1.3",
     "langchain-anthropic==0.1.11",
     "html2text==2024.2.26",
@@ -28,24 +27,22 @@
     "tqdm==4.66.4",
     "graphviz==0.20.3",
     "minify-html==0.15.0",
     "free-proxy==1.1.1",
     "playwright==1.43.0",
     "google==3.0.0",
     "yahoo-search-py==0.3",
-    "networkx==3.3",
-    "pyvis==0.3.2",
     "undetected-playwright==0.3.0",
 ]
 
 license = "MIT"
 readme = "README.md"
-homepage = "https://scrapegraph-ai.readthedocs.io/"
+homepage = "https://scrapegraphai.com/"
 repository = "https://github.com/VinciGit00/Scrapegraph-ai"
-documentation = "https://scrapegraph-doc.onrender.com/"
+documentation = "https://scrapegraph-ai.readthedocs.io/en/latest/"
 keywords = [
     "scrapegraph",
     "scrapegraphai",
     "langchain",
     "ai",
     "artificial intelligence",
     "gpt",
@@ -65,24 +62,23 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.9,<3.12"
 
+[project.optional-dependencies]
+burr = ["burr[start]==0.19.1"]
+docs = ["sphinx==6.0", "furo==2024.5.6"]
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "pytest==8.0.0",
-    "pytest-mock==3.14.0"
-]
-
-[tool.rye.group.docs]
-optional = true
-
-[tool.rye.group.docs.dependencies]
-sphinx = "7.1.2"
-sphinx-rtd-theme = "2.0.0"
+    "pytest-mock==3.14.0",
+    "-e file:.[burr]",
+    "-e file:.[docs]",
+]
```

### Comparing `scrapegraphai-1.5.0b3/PKG-INFO` & `scrapegraphai-1.5.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scrapegraphai
-Version: 1.5.0b3
+Version: 1.5.0b4
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Author-email: Marco Vinciguerra <mvincig11@gmail.com>, Marco Perini <perinim.98@gmail.com>, Lorenzo Padoan <lorenzo.padoan977@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ai,artificial intelligence,gpt,graph,langchain,machine learning,natural language processing,nlp,openai,rag,scrapegraph,scrapegraphai,scraping,web scraping,web scraping library,web scraping tool,webscraping
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -20,23 +20,26 @@
 Requires-Dist: langchain-anthropic==0.1.11
 Requires-Dist: langchain-aws==0.1.3
 Requires-Dist: langchain-google-genai==1.0.3
 Requires-Dist: langchain-groq==0.1.3
 Requires-Dist: langchain-openai==0.1.6
 Requires-Dist: langchain==0.1.15
 Requires-Dist: minify-html==0.15.0
-Requires-Dist: networkx==3.3
 Requires-Dist: pandas==2.2.2
 Requires-Dist: playwright==1.43.0
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: pyvis==0.3.2
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: tqdm==4.66.4
 Requires-Dist: undetected-playwright==0.3.0
 Requires-Dist: yahoo-search-py==0.3
+Provides-Extra: burr
+Requires-Dist: burr[start]==0.19.1; extra == 'burr'
+Provides-Extra: docs
+Requires-Dist: furo==2024.5.6; extra == 'docs'
+Requires-Dist: sphinx==6.0; extra == 'docs'
 Description-Content-Type: text/markdown
 
 
 # 🕷️ ScrapeGraphAI: You Only Scrape Once
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
```

