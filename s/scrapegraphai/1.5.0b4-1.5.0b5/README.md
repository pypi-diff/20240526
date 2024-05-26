# Comparing `tmp/scrapegraphai-1.5.0b4.tar.gz` & `tmp/scrapegraphai-1.5.0b5.tar.gz`

## Comparing `scrapegraphai-1.5.0b4.tar` & `scrapegraphai-1.5.0b5.tar`

### file list

```diff
@@ -1,284 +1,284 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.gitattributes
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.releaserc.yml
--rw-r--r--   0        0        0    48115 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/CHANGELOG.md
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/CONTRIBUTING.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/Dockerfile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/SECURITY.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/citation.cff
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docker-compose.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/readthedocs.yml
--rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements-dev.lock
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements-dev.txt
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements.lock
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.github/workflows/release.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/Makefile
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/make.bat
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_1.png
--rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_2.png
--rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_3.png
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/apikey_4.png
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/codespaces-badge.png
--rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/logo_authors.png
--rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/omniscrapergraph.png
--rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/omnisearchgraph.png
--rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.fig
--rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.png
--rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/scrapegraphai_logo.png
--rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/searchgraph.png
--rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/serp_api_logo.png
--rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/smartscrapergraph.png
--rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/speechgraph.png
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/assets/transparent_stat.png
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/conf.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/index.rst
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/getting_started/examples.rst
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/introduction/contributing.rst
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/introduction/overview.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/modules.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.builders.rst
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.docloaders.rst
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.graphs.rst
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.helpers.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.integrations.rst
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.models.rst
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.nodes.rst
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.rst
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.utils.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/benchmarks.rst
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/graph_config.rst
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/graphs.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/docs/source/scrapers/llm.rst
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/readme.md
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/anthropic/smart_scraper_haiku.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/json_scraper_azure.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/search_graph_azure.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/smart_scraper_azure_openai.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/xml_scraper_azure.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/azure/inputs/username.csv
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/.env.example
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/README.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/csv_scraper_bedrock.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/custom_graph_bedrock.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/json_scraper_bedrock.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/scrape_plain_text_bedrock.py
--rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/scrapegraphai_bedrock.png
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/script_generator_bedrock.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/search_graph_bedrock.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/smart_scraper_bedrock.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/xml_scraper_bedrock.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/books.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/bedrock/inputs/username.csv
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/readme.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/.env.example
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/.env.example
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/Readme.md
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_docker.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_groq.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_llama3.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_mistral.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_1.txt
--rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_2.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/.env.example
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/csv_scraper_deepseek.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/json_scraper_deepseek.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/script_generator_deepseek.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/search_graph_deepseek.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/smart_scarper_deepseek.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/xml_scraper_deepseek.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/inputs/example.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/deepseek/inputs/username.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/.env.example
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/csv_scraper_gemini.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/custom_graph_gemini.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/json_scraper_gemini.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/readme.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/scrape_plain_text_gemini.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/scrape_xml_gemini.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/script_generator_gemini.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/search_graph_gemini.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/smart_scraper_gemini.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/gemini/inputs/username.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/.env.example
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/search_graph_groq_openai.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_ollama.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_openai.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/huggingfacehub/smart_scraper_huggingfacehub.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/csv_scraper_ollama.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/json_scraper_ollama.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/scrape_plain_text_ollama.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/scrape_xml_ollama.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/script_generator_ollama.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/search_graph_ollama.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/smart_scraper_ollama.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/xml_scraper_ollama.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/local_models/inputs/username.csv
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/.env.example
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/readme.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/search_graph_groq_ollama.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/smart_scraper_mixed.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/mixed_models/inputs/plain_html_example.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/.env.example
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/csv_scraper_openai.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/custom_graph_openai.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/deep_scraper_openai.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/json_scraper_openai.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/omni_scraper_openai.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/omni_search_graph_openai.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/pdf_scraper_openai.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/readme.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/scrape_plain_text_openai.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/script_generator_openai.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/search_graph_openai.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/smart_scraper_multi_openai.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/smart_scraper_openai.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/smart_scraper_schema_openai.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/speech_graph_openai.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/xml_scraper_openai.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/openai/inputs/username.csv
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/fetch_node.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/image2text_node.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/kg_node.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/examples/single_node/robot_node.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/commit_and_push.sh
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/commit_and_push_with_tests.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/deploy_on_pip.sh
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/manual deployment/installation.sh
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/docloaders/__init__.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/docloaders/chromium.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    15389 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/deep_scraper_graph.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_scraper_graph.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_search_graph.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_multi_graph.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_prompts.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/integrations/__init__.py
--rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/integrations/burr_bridge.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/anthropic.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/deepseek.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_omni_node.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_node_with_context.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/cleanup_html.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/logging.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/sys_dynamic_import.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/Readme.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_json_ollama.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_llama3_test.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_mistral_test.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/scrape_xml_ollama_test.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/script_generator_test.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/smart_scraper_ollama_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/graphs/inputs/username.csv
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/fetch_node_test.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/robot_node_test.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/search_link_node_test.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/books.xml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/example.json
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/plain_html_example.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/nodes/inputs/username.csv
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/utils/test_proxy_rotation.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/tests/utils/test_sys_dynamic_import.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/LICENSE
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/README.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/pyproject.toml
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.gitattributes
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.releaserc.yml
+-rw-r--r--   0        0        0    48703 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/CHANGELOG.md
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/Dockerfile
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/SECURITY.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/citation.cff
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docker-compose.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/readthedocs.yml
+-rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/requirements-dev.lock
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/requirements-dev.txt
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/requirements.lock
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/Makefile
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/make.bat
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/apikey_1.png
+-rw-r--r--   0        0        0   123826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/apikey_2.png
+-rw-r--r--   0        0        0    60775 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/apikey_3.png
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/apikey_4.png
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/codespaces-badge.png
+-rw-r--r--   0        0        0  1178826 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/logo_authors.png
+-rw-r--r--   0        0        0    73949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/omniscrapergraph.png
+-rw-r--r--   0        0        0    58062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/omnisearchgraph.png
+-rw-r--r--   0        0        0    53007 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/project_overview_diagram.fig
+-rw-r--r--   0        0        0    83949 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/project_overview_diagram.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/scrapegraphai_logo.png
+-rw-r--r--   0        0        0    54611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/searchgraph.png
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/serp_api_logo.png
+-rw-r--r--   0        0        0    61095 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/smartscrapergraph.png
+-rw-r--r--   0        0        0    49312 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/speechgraph.png
+-rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/assets/transparent_stat.png
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/conf.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/index.rst
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/getting_started/examples.rst
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/introduction/contributing.rst
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/introduction/overview.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/modules.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.builders.rst
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.docloaders.rst
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.graphs.rst
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.helpers.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.integrations.rst
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.models.rst
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.nodes.rst
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.rst
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.utils.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/scrapers/benchmarks.rst
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/scrapers/graph_config.rst
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/scrapers/graphs.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/docs/source/scrapers/llm.rst
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/readme.md
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/anthropic/smart_scraper_haiku.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/azure/json_scraper_azure.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/azure/search_graph_azure.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/azure/smart_scraper_azure_openai.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/azure/xml_scraper_azure.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/azure/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/azure/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/azure/inputs/username.csv
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/.env.example
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/README.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/csv_scraper_bedrock.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/custom_graph_bedrock.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/json_scraper_bedrock.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/scrape_plain_text_bedrock.py
+-rw-r--r--   0        0        0    82480 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/scrapegraphai_bedrock.png
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/script_generator_bedrock.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/search_graph_bedrock.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/smart_scraper_bedrock.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/xml_scraper_bedrock.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/inputs/books.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/bedrock/inputs/username.csv
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/readme.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/.env.example
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/.env.example
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/Readme.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_docker.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_groq.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_llama3.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_mistral.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/inputs/example_1.txt
+-rw-r--r--   0        0        0  2590773 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/inputs/example_2.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/.env.example
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/csv_scraper_deepseek.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/json_scraper_deepseek.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/script_generator_deepseek.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/search_graph_deepseek.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/smart_scarper_deepseek.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/xml_scraper_deepseek.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/inputs/example.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/deepseek/inputs/username.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/.env.example
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/csv_scraper_gemini.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/custom_graph_gemini.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/json_scraper_gemini.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/readme.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/scrape_plain_text_gemini.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/scrape_xml_gemini.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/script_generator_gemini.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/search_graph_gemini.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/smart_scraper_gemini.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/gemini/inputs/username.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/groq/.env.example
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/groq/search_graph_groq_openai.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/groq/smart_scraper_groq_ollama.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/groq/smart_scraper_groq_openai.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/huggingfacehub/smart_scraper_huggingfacehub.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/csv_scraper_ollama.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/json_scraper_ollama.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/scrape_plain_text_ollama.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/scrape_xml_ollama.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/script_generator_ollama.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/search_graph_ollama.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/smart_scraper_ollama.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/xml_scraper_ollama.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/local_models/inputs/username.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/mixed_models/.env.example
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/mixed_models/readme.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/mixed_models/search_graph_groq_ollama.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/mixed_models/smart_scraper_mixed.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/mixed_models/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/mixed_models/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/mixed_models/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/.env.example
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/csv_scraper_openai.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/custom_graph_openai.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/deep_scraper_openai.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/json_scraper_openai.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/omni_scraper_openai.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/omni_search_graph_openai.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/pdf_scraper_openai.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/readme.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/scrape_plain_text_openai.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/script_generator_openai.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/search_graph_openai.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/smart_scraper_multi_openai.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/smart_scraper_openai.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/smart_scraper_schema_openai.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/speech_graph_openai.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/xml_scraper_openai.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/openai/inputs/username.csv
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/single_node/fetch_node.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/single_node/image2text_node.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/single_node/kg_node.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/examples/single_node/robot_node.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/manual deployment/commit_and_push.sh
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/manual deployment/commit_and_push_with_tests.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/manual deployment/deploy_on_pip.sh
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/manual deployment/installation.sh
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/docloaders/__init__.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/docloaders/chromium.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    15389 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/deep_scraper_graph.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/omni_scraper_graph.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/omni_search_graph.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/smart_scraper_multi_graph.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_csv_prompts.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_omni_prompts.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_prompts.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/integrations/__init__.py
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/integrations/burr_bridge.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/anthropic.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/deepseek.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_omni_node.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/search_node_with_context.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/cleanup_html.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/logging.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/sys_dynamic_import.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/Readme.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/scrape_json_ollama.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/scrape_plain_text_llama3_test.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/scrape_plain_text_mistral_test.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/scrape_xml_ollama_test.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/script_generator_test.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/smart_scraper_ollama_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/graphs/inputs/username.csv
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/nodes/fetch_node_test.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/nodes/robot_node_test.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/nodes/search_link_node_test.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/nodes/inputs/books.xml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/nodes/inputs/example.json
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/nodes/inputs/plain_html_example.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/nodes/inputs/username.csv
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/utils/test_proxy_rotation.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/tests/utils/test_sys_dynamic_import.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/LICENSE
+-rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/README.md
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/pyproject.toml
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 scrapegraphai-1.5.0b5/PKG-INFO
```

### Comparing `scrapegraphai-1.5.0b4/.releaserc.yml` & `scrapegraphai-1.5.0b5/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/CHANGELOG.md` & `scrapegraphai-1.5.0b5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## [1.5.0-beta.5](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.0-beta.4...v1.5.0-beta.5) (2024-05-26)
+
+
+### Features
+
+* **version:** python 3.12 is now supported 🚀 ([5fb9115](https://github.com/VinciGit00/Scrapegraph-ai/commit/5fb9115330141ac2c1dd97490284d4f1fa2c01c3))
+
+
+### Docs
+
+* **faq:** added faq section and refined installation ([545374c](https://github.com/VinciGit00/Scrapegraph-ai/commit/545374c17e9101a240fd1fbc380ce813c5aa6c2e))
+* updated requirements ([e43b801](https://github.com/VinciGit00/Scrapegraph-ai/commit/e43b8018f5f360b88c52e45ff4e1b4221386ea8e))
+
 ## [1.5.0-beta.4](https://github.com/VinciGit00/Scrapegraph-ai/compare/v1.5.0-beta.3...v1.5.0-beta.4) (2024-05-25)
 
 
 ### Features
 
 * **burr:** added burr integration in graphs and optional burr installation ([ac10128](https://github.com/VinciGit00/Scrapegraph-ai/commit/ac10128ff3af35c52b48c79d085e458524e8e48a))
 * **burr-bridge:** BurrBridge class to integrate inside BaseGraph ([6cbd84f](https://github.com/VinciGit00/Scrapegraph-ai/commit/6cbd84f254ebc1f1c68699273bdd8fcdb0fe26d4))
```

### Comparing `scrapegraphai-1.5.0b4/CODE_OF_CONDUCT.md` & `scrapegraphai-1.5.0b5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/CONTRIBUTING.md` & `scrapegraphai-1.5.0b5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/readthedocs.yml` & `scrapegraphai-1.5.0b5/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/requirements-dev.lock` & `scrapegraphai-1.5.0b5/requirements-dev.lock`

 * *Files 2% similar despite different names*

```diff
@@ -26,32 +26,29 @@
 anyio==4.3.0
     # via anthropic
     # via groq
     # via httpx
     # via openai
     # via starlette
     # via watchfiles
-async-timeout==4.0.3
-    # via aiohttp
-    # via langchain
 attrs==23.2.0
     # via aiohttp
     # via jsonschema
     # via referencing
 babel==2.15.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
     # via google
     # via scrapegraphai
 blinker==1.8.2
     # via streamlit
-boto3==1.34.110
+boto3==1.34.113
     # via langchain-aws
-botocore==1.34.110
+botocore==1.34.113
     # via boto3
     # via s3transfer
 burr==0.19.1
     # via burr
     # via scrapegraphai
 cachetools==5.3.3
     # via google-auth
@@ -77,54 +74,45 @@
 contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
 dataclasses-json==0.6.6
     # via langchain
     # via langchain-community
-decorator==5.1.1
-    # via ipython
 defusedxml==0.7.1
     # via langchain-anthropic
 distro==1.9.0
     # via anthropic
     # via groq
     # via openai
 dnspython==2.6.1
     # via email-validator
 docutils==0.19
     # via sphinx
 email-validator==2.1.1
     # via fastapi
-exceptiongroup==1.2.1
-    # via anyio
-    # via ipython
-    # via pytest
-executing==2.0.1
-    # via stack-data
 faiss-cpu==1.8.0
     # via scrapegraphai
 fastapi==0.111.0
     # via burr
     # via fastapi-pagination
 fastapi-cli==0.0.4
     # via fastapi
 fastapi-pagination==0.12.24
     # via burr
 filelock==3.14.0
     # via huggingface-hub
-fonttools==4.51.0
+fonttools==4.52.1
     # via matplotlib
 free-proxy==1.1.1
     # via scrapegraphai
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 fsspec==2024.5.0
-fsspec==2024.5.0
     # via huggingface-hub
 furo==2024.5.6
     # via scrapegraphai
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via streamlit
@@ -132,15 +120,15 @@
     # via scrapegraphai
 google-ai-generativelanguage==0.6.4
     # via google-generativeai
 google-api-core==2.19.0
     # via google-ai-generativelanguage
     # via google-api-python-client
     # via google-generativeai
-google-api-python-client==2.129.0
+google-api-python-client==2.130.0
     # via google-generativeai
 google-auth==2.29.0
     # via google-ai-generativelanguage
     # via google-api-core
     # via google-api-python-client
     # via google-auth-httplib2
     # via google-generativeai
@@ -153,15 +141,15 @@
     # via grpcio-status
 graphviz==0.20.3
     # via burr
     # via scrapegraphai
 greenlet==3.0.3
     # via playwright
     # via sqlalchemy
-groq==0.7.0
+groq==0.8.0
     # via langchain-groq
 grpcio==1.64.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
@@ -177,15 +165,14 @@
 httptools==0.6.1
     # via uvicorn
 httpx==0.27.0
     # via anthropic
     # via fastapi
     # via groq
     # via openai
-    # via yahoo-search-py
 huggingface-hub==0.23.1
     # via tokenizers
 idna==3.7
     # via anyio
     # via email-validator
     # via httpx
     # via requests
@@ -196,24 +183,22 @@
     # via pytest
 jinja2==3.1.4
     # via altair
     # via burr
     # via fastapi
     # via pydeck
     # via sphinx
-jiter==0.1.0
+jiter==0.4.0
     # via anthropic
 jmespath==1.0.1
     # via boto3
     # via botocore
 jsonpatch==1.33
     # via langchain
     # via langchain-core
-jsonpickle==3.0.4
-    # via pyvis
 jsonpointer==2.4
     # via jsonpatch
 jsonschema==4.22.0
     # via altair
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
@@ -239,15 +224,15 @@
     # via scrapegraphai
 langchain-groq==0.1.3
     # via scrapegraphai
 langchain-openai==0.1.6
     # via scrapegraphai
 langchain-text-splitters==0.0.2
     # via langchain
-langsmith==0.1.60
+langsmith==0.1.63
     # via langchain
     # via langchain-community
     # via langchain-core
 loguru==0.7.2
     # via burr
 lxml==5.2.2
     # via free-proxy
@@ -264,31 +249,28 @@
 minify-html==0.15.0
     # via scrapegraphai
 multidict==6.0.5
     # via aiohttp
     # via yarl
 mypy-extensions==1.0.0
     # via typing-inspect
-networkx==3.3
-    # via pyvis
-    # via scrapegraphai
 numpy==1.26.4
     # via altair
     # via contourpy
     # via faiss-cpu
     # via langchain
     # via langchain-aws
     # via langchain-community
     # via matplotlib
     # via pandas
     # via pyarrow
     # via pydeck
     # via sf-hamilton
     # via streamlit
-openai==1.30.1
+openai==1.30.3
     # via burr
     # via langchain-openai
 orjson==3.10.3
     # via fastapi
     # via langsmith
 packaging==23.2
     # via altair
@@ -308,16 +290,14 @@
     # via matplotlib
     # via streamlit
 playwright==1.43.0
     # via scrapegraphai
     # via undetected-playwright
 pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
-    # via ipython
 proto-plus==1.23.0
     # via google-ai-generativelanguage
     # via google-api-core
 protobuf==4.25.3
     # via google-ai-generativelanguage
     # via google-api-core
     # via google-generativeai
@@ -339,27 +319,24 @@
     # via fastapi-pagination
     # via google-generativeai
     # via groq
     # via langchain
     # via langchain-core
     # via langsmith
     # via openai
-    # via yahoo-search-py
 pydantic-core==2.18.2
     # via pydantic
 pydeck==0.9.1
     # via streamlit
 pyee==11.1.0
     # via playwright
 pygments==2.18.0
     # via furo
     # via rich
     # via sphinx
-pygments==2.18.0
-    # via ipython
 pyparsing==3.1.2
     # via httplib2
     # via matplotlib
 pytest==8.0.0
     # via pytest-mock
 pytest-mock==3.14.0
 python-dateutil==2.9.0.post0
@@ -369,16 +346,14 @@
 python-dotenv==1.0.1
     # via scrapegraphai
     # via uvicorn
 python-multipart==0.0.9
     # via fastapi
 pytz==2024.1
     # via pandas
-pyvis==0.3.2
-    # via scrapegraphai
 pyyaml==6.0.1
     # via huggingface-hub
     # via langchain
     # via langchain-community
     # via langchain-core
     # via uvicorn
 referencing==0.35.1
@@ -403,22 +378,19 @@
 rpds-py==0.18.1
     # via jsonschema
     # via referencing
 rsa==4.9
     # via google-auth
 s3transfer==0.10.1
     # via boto3
-selectolax==0.3.21
-    # via yahoo-search-py
 sf-hamilton==1.63.0
     # via burr
 shellingham==1.5.4
     # via typer
 six==1.16.0
-    # via asttokens
     # via python-dateutil
 smmap==5.0.1
     # via gitdb
 sniffio==1.3.1
     # via anthropic
     # via anyio
     # via groq
@@ -447,89 +419,75 @@
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sqlalchemy==2.0.30
     # via langchain
     # via langchain-community
 starlette==0.37.2
     # via fastapi
-streamlit==1.34.0
+streamlit==1.35.0
     # via burr
-stack-data==0.6.3
-    # via ipython
 tenacity==8.3.0
     # via langchain
     # via langchain-community
     # via langchain-core
     # via streamlit
 tiktoken==0.6.0
     # via langchain-openai
     # via scrapegraphai
 tokenizers==0.19.1
     # via anthropic
 toml==0.10.2
     # via streamlit
-tomli==2.0.1
-    # via pytest
 toolz==0.12.1
     # via altair
 tornado==6.4
     # via streamlit
 tqdm==4.66.4
     # via google-generativeai
     # via huggingface-hub
     # via openai
     # via scrapegraphai
 typer==0.12.3
     # via fastapi-cli
-traitlets==5.14.3
-    # via ipython
-    # via matplotlib-inline
-typing-extensions==4.11.0
-    # via altair
+typing-extensions==4.12.0
     # via anthropic
-    # via anyio
     # via fastapi
     # via fastapi-pagination
     # via google-generativeai
     # via groq
     # via huggingface-hub
-    # via ipython
     # via openai
     # via pydantic
     # via pydantic-core
     # via pyee
     # via sf-hamilton
     # via sqlalchemy
     # via streamlit
     # via typer
     # via typing-inspect
-    # via uvicorn
 typing-inspect==0.9.0
     # via dataclasses-json
     # via sf-hamilton
 tzdata==2024.1
     # via pandas
-undetected-playwright==0.3.0
-    # via scrapegraphai
 ujson==5.10.0
     # via fastapi
+undetected-playwright==0.3.0
+    # via scrapegraphai
 uritemplate==4.1.1
     # via google-api-python-client
 urllib3==2.2.1
     # via botocore
     # via requests
-    # via yahoo-search-py
 uvicorn==0.29.0
     # via burr
     # via fastapi
-watchdog==4.0.0
+watchdog==4.0.1
     # via streamlit
 watchfiles==0.21.0
     # via uvicorn
 websockets==12.0
     # via uvicorn
 win32-setctime==1.1.0
     # via loguru
-yahoo-search-py==0.3
-    # via scrapegraphai
 yarl==1.9.4
     # via aiohttp
```

### Comparing `scrapegraphai-1.5.0b4/requirements.lock` & `scrapegraphai-1.5.0b5/requirements.lock`

 * *Files 27% similar despite different names*

```diff
@@ -18,27 +18,22 @@
 anthropic==0.26.1
     # via langchain-anthropic
 anyio==4.3.0
     # via anthropic
     # via groq
     # via httpx
     # via openai
-asttokens==2.4.1
-    # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
-    # via langchain
 attrs==23.2.0
     # via aiohttp
 beautifulsoup4==4.12.3
     # via google
     # via scrapegraphai
-boto3==1.34.110
+boto3==1.34.113
     # via langchain-aws
-botocore==1.34.110
+botocore==1.34.113
     # via boto3
     # via s3transfer
 cachetools==5.3.3
     # via google-auth
 certifi==2024.2.2
     # via httpcore
     # via httpx
@@ -46,48 +41,40 @@
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via tqdm
 dataclasses-json==0.6.6
     # via langchain
     # via langchain-community
-decorator==5.1.1
-    # via ipython
 defusedxml==0.7.1
     # via langchain-anthropic
 distro==1.9.0
     # via anthropic
     # via groq
     # via openai
-exceptiongroup==1.2.1
-    # via anyio
-    # via ipython
-executing==2.0.1
-    # via stack-data
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
-fsspec==2024.5.0
     # via huggingface-hub
 google==3.0.0
     # via scrapegraphai
 google-ai-generativelanguage==0.6.4
     # via google-generativeai
 google-api-core==2.19.0
     # via google-ai-generativelanguage
     # via google-api-python-client
     # via google-generativeai
-google-api-python-client==2.129.0
+google-api-python-client==2.130.0
     # via google-generativeai
 google-auth==2.29.0
     # via google-ai-generativelanguage
     # via google-api-core
     # via google-api-python-client
     # via google-auth-httplib2
     # via google-generativeai
@@ -99,15 +86,15 @@
     # via google-api-core
     # via grpcio-status
 graphviz==0.20.3
     # via scrapegraphai
 greenlet==3.0.3
     # via playwright
     # via sqlalchemy
-groq==0.7.0
+groq==0.8.0
     # via langchain-groq
 grpcio==1.64.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
@@ -119,32 +106,29 @@
 httplib2==0.22.0
     # via google-api-python-client
     # via google-auth-httplib2
 httpx==0.27.0
     # via anthropic
     # via groq
     # via openai
-    # via yahoo-search-py
 huggingface-hub==0.23.1
     # via tokenizers
 idna==3.7
     # via anyio
     # via httpx
     # via requests
     # via yarl
-jiter==0.1.0
+jiter==0.4.0
     # via anthropic
 jmespath==1.0.1
     # via boto3
     # via botocore
 jsonpatch==1.33
     # via langchain
     # via langchain-core
-jsonpickle==3.0.4
-    # via pyvis
 jsonpointer==2.4
     # via jsonpatch
 langchain==0.1.15
     # via scrapegraphai
 langchain-anthropic==0.1.11
     # via scrapegraphai
 langchain-aws==0.1.3
@@ -164,106 +148,84 @@
     # via scrapegraphai
 langchain-groq==0.1.3
     # via scrapegraphai
 langchain-openai==0.1.6
     # via scrapegraphai
 langchain-text-splitters==0.0.2
     # via langchain
-langsmith==0.1.60
+langsmith==0.1.63
     # via langchain
     # via langchain-community
     # via langchain-core
 lxml==5.2.2
     # via free-proxy
-markupsafe==2.1.5
-    # via jinja2
 marshmallow==3.21.2
     # via dataclasses-json
-matplotlib-inline==0.1.7
-    # via ipython
 minify-html==0.15.0
     # via scrapegraphai
 multidict==6.0.5
     # via aiohttp
     # via yarl
 mypy-extensions==1.0.0
     # via typing-inspect
-networkx==3.3
-    # via pyvis
-    # via scrapegraphai
 numpy==1.26.4
     # via faiss-cpu
     # via langchain
     # via langchain-aws
     # via langchain-community
     # via pandas
-openai==1.30.1
+openai==1.30.3
     # via langchain-openai
 orjson==3.10.3
     # via langsmith
 packaging==23.2
     # via huggingface-hub
     # via langchain-core
     # via marshmallow
 pandas==2.2.2
     # via scrapegraphai
-parso==0.8.4
-    # via jedi
-pexpect==4.9.0
-    # via ipython
 playwright==1.43.0
     # via scrapegraphai
     # via undetected-playwright
-prompt-toolkit==3.0.43
-    # via ipython
 proto-plus==1.23.0
     # via google-ai-generativelanguage
     # via google-api-core
 protobuf==4.25.3
     # via google-ai-generativelanguage
     # via google-api-core
     # via google-generativeai
     # via googleapis-common-protos
     # via grpcio-status
     # via proto-plus
-ptyprocess==0.7.0
-    # via pexpect
-pure-eval==0.2.2
-    # via stack-data
 pyasn1==0.6.0
     # via pyasn1-modules
     # via rsa
 pyasn1-modules==0.4.0
     # via google-auth
 pydantic==2.7.1
     # via anthropic
     # via google-generativeai
     # via groq
     # via langchain
     # via langchain-core
     # via langsmith
     # via openai
-    # via yahoo-search-py
 pydantic-core==2.18.2
     # via pydantic
 pyee==11.1.0
     # via playwright
-pygments==2.18.0
-    # via ipython
 pyparsing==3.1.2
     # via httplib2
 python-dateutil==2.9.0.post0
     # via botocore
     # via pandas
 python-dotenv==1.0.1
     # via scrapegraphai
 pytz==2024.1
     # via pandas
-pyvis==0.3.2
-    # via scrapegraphai
 pyyaml==6.0.1
     # via huggingface-hub
     # via langchain
     # via langchain-community
     # via langchain-core
 regex==2024.5.15
     # via tiktoken
@@ -275,56 +237,46 @@
     # via langchain-community
     # via langsmith
     # via tiktoken
 rsa==4.9
     # via google-auth
 s3transfer==0.10.1
     # via boto3
-selectolax==0.3.21
-    # via yahoo-search-py
 six==1.16.0
-    # via asttokens
     # via python-dateutil
 sniffio==1.3.1
     # via anthropic
     # via anyio
     # via groq
     # via httpx
     # via openai
 soupsieve==2.5
     # via beautifulsoup4
 sqlalchemy==2.0.30
     # via langchain
     # via langchain-community
-stack-data==0.6.3
-    # via ipython
 tenacity==8.3.0
     # via langchain
     # via langchain-community
     # via langchain-core
 tiktoken==0.6.0
     # via langchain-openai
     # via scrapegraphai
 tokenizers==0.19.1
     # via anthropic
 tqdm==4.66.4
     # via google-generativeai
     # via huggingface-hub
     # via openai
     # via scrapegraphai
-traitlets==5.14.3
-    # via ipython
-    # via matplotlib-inline
-typing-extensions==4.11.0
+typing-extensions==4.12.0
     # via anthropic
-    # via anyio
     # via google-generativeai
     # via groq
     # via huggingface-hub
-    # via ipython
     # via openai
     # via pydantic
     # via pydantic-core
     # via pyee
     # via sqlalchemy
     # via typing-inspect
 typing-inspect==0.9.0
@@ -332,17 +284,11 @@
 tzdata==2024.1
     # via pandas
 undetected-playwright==0.3.0
     # via scrapegraphai
 uritemplate==4.1.1
     # via google-api-python-client
 urllib3==2.2.1
-urllib3==2.2.1
     # via botocore
     # via requests
-    # via yahoo-search-py
-wcwidth==0.2.13
-    # via prompt-toolkit
-yahoo-search-py==0.3
-    # via scrapegraphai
 yarl==1.9.4
     # via aiohttp
```

### Comparing `scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/bug_report.md` & `scrapegraphai-1.5.0b5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/.github/ISSUE_TEMPLATE/feature_request.md` & `scrapegraphai-1.5.0b5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/.github/workflows/codeql.yml` & `scrapegraphai-1.5.0b5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/.github/workflows/dependency-review.yml` & `scrapegraphai-1.5.0b5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/.github/workflows/pylint.yml` & `scrapegraphai-1.5.0b5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/.github/workflows/python-publish.yml` & `scrapegraphai-1.5.0b5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/.github/workflows/release.yml` & `scrapegraphai-1.5.0b5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/Makefile` & `scrapegraphai-1.5.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/README.md` & `scrapegraphai-1.5.0b5/docs/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/make.bat` & `scrapegraphai-1.5.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/apikey_1.png` & `scrapegraphai-1.5.0b5/docs/assets/apikey_1.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/apikey_2.png` & `scrapegraphai-1.5.0b5/docs/assets/apikey_2.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/apikey_3.png` & `scrapegraphai-1.5.0b5/docs/assets/apikey_3.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/apikey_4.png` & `scrapegraphai-1.5.0b5/docs/assets/apikey_4.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/codespaces-badge.png` & `scrapegraphai-1.5.0b5/docs/assets/codespaces-badge.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/logo_authors.png` & `scrapegraphai-1.5.0b5/docs/assets/logo_authors.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/omniscrapergraph.png` & `scrapegraphai-1.5.0b5/docs/assets/omniscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/omnisearchgraph.png` & `scrapegraphai-1.5.0b5/docs/assets/omnisearchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.fig` & `scrapegraphai-1.5.0b5/docs/assets/project_overview_diagram.fig`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/project_overview_diagram.png` & `scrapegraphai-1.5.0b5/docs/assets/project_overview_diagram.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/scrapegraphai_logo.png` & `scrapegraphai-1.5.0b5/docs/assets/scrapegraphai_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/searchgraph.png` & `scrapegraphai-1.5.0b5/docs/assets/searchgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/serp_api_logo.png` & `scrapegraphai-1.5.0b5/docs/assets/serp_api_logo.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/smartscrapergraph.png` & `scrapegraphai-1.5.0b5/docs/assets/smartscrapergraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/speechgraph.png` & `scrapegraphai-1.5.0b5/docs/assets/speechgraph.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/assets/transparent_stat.png` & `scrapegraphai-1.5.0b5/docs/assets/transparent_stat.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/conf.py` & `scrapegraphai-1.5.0b5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/index.rst` & `scrapegraphai-1.5.0b5/docs/source/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -28,13 +28,22 @@
 
 .. toctree::
    :maxdepth: 2
    :caption: Modules
 
    modules/modules
 
+.. toctree::
+   :hidden:
+   :caption: EXTERNAL RESOURCES
+
+   GitHub <https://github.com/VinciGit00/Scrapegraph-ai>
+   Discord <https://discord.gg/uJN7TYcpNa>
+   Linkedin <https://www.linkedin.com/company/scrapegraphai/>
+   Twitter <https://twitter.com/scrapegraphai>
+
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `scrapegraphai-1.5.0b4/docs/source/getting_started/examples.rst` & `scrapegraphai-1.5.0b5/docs/source/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/getting_started/installation.rst` & `scrapegraphai-1.5.0b5/docs/source/getting_started/installation.rst`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,26 @@
 
    pip install scrapegraphai
 
 .. important::
    
    It is higly recommended to install the library in a virtual environment (conda, venv, etc.)
 
-If your clone the repository, you can install the library using `poetry <https://python-poetry.org/docs/>`_:
+If your clone the repository, it is recommended to use a package manager like `rye <https://rye.astral.sh/>`_.
+To install the library using rye, you can run the following command:
 
 .. code-block:: bash
 
-   poetry install
+   rye pin 3.10
+   rye sync
+   rye build
+
+.. caution::
+   
+      **Rye** must be installed first by following the instructions on the `official website <https://rye.astral.sh/>`_.
 
 Additionally on Windows when using WSL
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you are using Windows Subsystem for Linux (WSL) and you are facing issues with the installation of the library, you might need to install the following packages:
 
 .. code-block:: bash
```

### Comparing `scrapegraphai-1.5.0b4/docs/source/introduction/contributing.rst` & `scrapegraphai-1.5.0b5/docs/source/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.graphs.rst` & `scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.helpers.rst` & `scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.helpers.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.models.rst` & `scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.models.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.nodes.rst` & `scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.nodes.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/modules/scrapegraphai.utils.rst` & `scrapegraphai-1.5.0b5/docs/source/modules/scrapegraphai.utils.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/scrapers/benchmarks.rst` & `scrapegraphai-1.5.0b5/docs/source/scrapers/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/scrapers/graph_config.rst` & `scrapegraphai-1.5.0b5/docs/source/scrapers/graph_config.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 - `headless`: If set to `False`, the web browser will be opened on the URL requested and close right after the HTML is fetched.
 - `max_results`: The maximum number of results to be fetched from the search engine. Useful in `SearchGraph`.
 - `output_path`: The path where the output files will be saved. Useful in `SpeechGraph`.
 - `loader_kwargs`: A dictionary with additional parameters to be passed to the `Loader` class, such as `proxy`.
 - `burr_kwargs`: A dictionary with additional parameters to enable `Burr` graphical user interface.
 - `max_images`: The maximum number of images to be analyzed. Useful in `OmniScraperGraph` and `OmniSearchGraph`.
 
+.. _Burr:
+
 Burr Integration
 ^^^^^^^^^^^^^^^^
 
 `Burr` is an open source python library that allows the creation and management of state machine applications. Discover more about it `here <https://github.com/DAGWorks-Inc/burr>`_.
 It is possible to enable a local hosted webapp to visualize the scraping pipelines and the data flow.
 First, we need to install the `burr` library as follows:
 
@@ -39,14 +41,16 @@
         "llm":{...},
         "burr_kwargs": {
             "project_name": "test-scraper",
             "app_instance_id":"some_id",
         }
     }
 
+.. _Proxy:
+
 Proxy Rotation
 ^^^^^^^^^^^^^^
 
 It is possible to rotate the proxy by setting the `proxy` option in the graph configuration.
 We provide a free proxy service which is based on `free-proxy <https://pypi.org/project/free-proxy/>`_ library and can be used as follows:
 
 .. code-block:: python
```

### Comparing `scrapegraphai-1.5.0b4/docs/source/scrapers/graphs.rst` & `scrapegraphai-1.5.0b5/docs/source/scrapers/graphs.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/docs/source/scrapers/llm.rst` & `scrapegraphai-1.5.0b5/docs/source/scrapers/llm.rst`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/readme.md` & `scrapegraphai-1.5.0b5/examples/readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/anthropic/smart_scraper_haiku.py` & `scrapegraphai-1.5.0b5/examples/anthropic/smart_scraper_haiku.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/azure/json_scraper_azure.py` & `scrapegraphai-1.5.0b5/examples/azure/json_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/azure/search_graph_azure.py` & `scrapegraphai-1.5.0b5/examples/azure/search_graph_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/azure/smart_scraper_azure_openai.py` & `scrapegraphai-1.5.0b5/examples/azure/smart_scraper_azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/azure/xml_scraper_azure.py` & `scrapegraphai-1.5.0b5/examples/azure/xml_scraper_azure.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/azure/inputs/books.xml` & `scrapegraphai-1.5.0b5/examples/azure/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/azure/inputs/example.json` & `scrapegraphai-1.5.0b5/examples/azure/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/csv_scraper_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/csv_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/custom_graph_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/custom_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/json_scraper_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/json_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/scrape_plain_text_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/scrape_plain_text_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/scrapegraphai_bedrock.png` & `scrapegraphai-1.5.0b5/examples/bedrock/scrapegraphai_bedrock.png`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/script_generator_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/script_generator_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/search_graph_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/search_graph_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/smart_scraper_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/smart_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/xml_scraper_bedrock.py` & `scrapegraphai-1.5.0b5/examples/bedrock/xml_scraper_bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/inputs/books.xml` & `scrapegraphai-1.5.0b5/examples/bedrock/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/inputs/example.json` & `scrapegraphai-1.5.0b5/examples/bedrock/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/bedrock/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b5/examples/bedrock/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/Readme.md` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/GenerateScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b5/examples/benchmarks/GenerateScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/Readme.md` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/Readme.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_docker.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_docker.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_groq.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_llama3.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_llama3.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_mistral.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_mistral.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/benchmark_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_1.txt` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/inputs/example_1.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/benchmarks/SmartScraper/inputs/example_2.txt` & `scrapegraphai-1.5.0b5/examples/benchmarks/SmartScraper/inputs/example_2.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/csv_scraper_deepseek.py` & `scrapegraphai-1.5.0b5/examples/deepseek/csv_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/json_scraper_deepseek.py` & `scrapegraphai-1.5.0b5/examples/deepseek/json_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/script_generator_deepseek.py` & `scrapegraphai-1.5.0b5/examples/deepseek/script_generator_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/search_graph_deepseek.py` & `scrapegraphai-1.5.0b5/examples/deepseek/search_graph_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/smart_scarper_deepseek.py` & `scrapegraphai-1.5.0b5/examples/deepseek/smart_scarper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/xml_scraper_deepseek.py` & `scrapegraphai-1.5.0b5/examples/deepseek/xml_scraper_deepseek.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/inputs/books.xml` & `scrapegraphai-1.5.0b5/examples/deepseek/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/deepseek/inputs/example.json` & `scrapegraphai-1.5.0b5/examples/deepseek/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/csv_scraper_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/csv_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/custom_graph_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/custom_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/json_scraper_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/json_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/scrape_plain_text_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/scrape_plain_text_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/scrape_xml_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/scrape_xml_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/script_generator_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/script_generator_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/search_graph_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/search_graph_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/smart_scraper_gemini.py` & `scrapegraphai-1.5.0b5/examples/gemini/smart_scraper_gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/xml_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/gemini/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/inputs/books.xml` & `scrapegraphai-1.5.0b5/examples/gemini/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/inputs/example.json` & `scrapegraphai-1.5.0b5/examples/gemini/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/gemini/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b5/examples/gemini/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/groq/search_graph_groq_openai.py` & `scrapegraphai-1.5.0b5/examples/groq/search_graph_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_ollama.py` & `scrapegraphai-1.5.0b5/examples/groq/smart_scraper_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/groq/smart_scraper_groq_openai.py` & `scrapegraphai-1.5.0b5/examples/groq/smart_scraper_groq_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/huggingfacehub/smart_scraper_huggingfacehub.py` & `scrapegraphai-1.5.0b5/examples/huggingfacehub/smart_scraper_huggingfacehub.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/csv_scraper_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/csv_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/json_scraper_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/json_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/scrape_plain_text_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/scrape_plain_text_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/scrape_xml_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/scrape_xml_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/script_generator_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/script_generator_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/search_graph_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/search_graph_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/smart_scraper_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/smart_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/xml_scraper_ollama.py` & `scrapegraphai-1.5.0b5/examples/local_models/xml_scraper_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/inputs/books.xml` & `scrapegraphai-1.5.0b5/examples/local_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/inputs/example.json` & `scrapegraphai-1.5.0b5/examples/local_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/local_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b5/examples/local_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/mixed_models/search_graph_groq_ollama.py` & `scrapegraphai-1.5.0b5/examples/mixed_models/search_graph_groq_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/mixed_models/smart_scraper_mixed.py` & `scrapegraphai-1.5.0b5/examples/mixed_models/smart_scraper_mixed.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/mixed_models/inputs/books.xml` & `scrapegraphai-1.5.0b5/examples/mixed_models/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/mixed_models/inputs/example.json` & `scrapegraphai-1.5.0b5/examples/mixed_models/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/mixed_models/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b5/examples/mixed_models/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/csv_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/csv_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/custom_graph_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/custom_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/deep_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/deep_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/json_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/json_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/omni_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/omni_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/omni_search_graph_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/omni_search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/pdf_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/pdf_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/scrape_plain_text_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/scrape_plain_text_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/script_generator_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/script_generator_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/search_graph_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/search_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/smart_scraper_multi_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/smart_scraper_multi_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/smart_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/smart_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/smart_scraper_schema_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/smart_scraper_schema_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/speech_graph_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/speech_graph_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/xml_scraper_openai.py` & `scrapegraphai-1.5.0b5/examples/openai/xml_scraper_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/inputs/books.xml` & `scrapegraphai-1.5.0b5/examples/openai/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/inputs/example.json` & `scrapegraphai-1.5.0b5/examples/openai/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/openai/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b5/examples/openai/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/single_node/fetch_node.py` & `scrapegraphai-1.5.0b5/examples/single_node/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/single_node/image2text_node.py` & `scrapegraphai-1.5.0b5/examples/single_node/image2text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/single_node/kg_node.py` & `scrapegraphai-1.5.0b5/examples/single_node/kg_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/examples/single_node/robot_node.py` & `scrapegraphai-1.5.0b5/examples/single_node/robot_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/manual deployment/commit_and_push.sh` & `scrapegraphai-1.5.0b5/manual deployment/commit_and_push.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/manual deployment/commit_and_push_with_tests.sh` & `scrapegraphai-1.5.0b5/manual deployment/commit_and_push_with_tests.sh`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-1.5.0b5/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/docloaders/chromium.py` & `scrapegraphai-1.5.0b5/scrapegraphai/docloaders/chromium.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/__init__.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/deep_scraper_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/deep_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_scraper_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/omni_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/omni_search_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/omni_search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/smart_scraper_multi_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/smart_scraper_multi_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-1.5.0b5/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/__init__.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_csv_prompts.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_csv_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_omni_prompts.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_omni_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_pdf_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/generate_answer_node_prompts.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/generate_answer_node_prompts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/helpers/schemas.py` & `scrapegraphai-1.5.0b5/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/integrations/burr_bridge.py` & `scrapegraphai-1.5.0b5/scrapegraphai/integrations/burr_bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Bridge class to integrate Burr into ScrapeGraphAI graphs
 [Burr](https://github.com/DAGWorks-Inc/burr)
 """
 
 import re
 from typing import Any, Dict, List, Tuple
+import inspect
 
 try:
     import burr
 except ImportError:
     raise ImportError("burr package is not installed. Please install it with 'pip install scrapegraphai[burr]'")
 
 from burr import tracking
@@ -50,14 +51,17 @@
 
     @property
     def writes(self) -> list[str]:
         return self.node.output
 
     def update(self, result: dict, state: State) -> State:
         return state.update(**result)
+    
+    def get_source(self) -> str:
+        return inspect.getsource(self.node.__class__)
 
 
 def parse_boolean_expression(expression: str) -> List[str]:
     """
     Parse a boolean expression to extract the keys used in the expression, without boolean operators.
 
     Args:
```

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/models/bedrock.py` & `scrapegraphai-1.5.0b5/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/models/gemini.py` & `scrapegraphai-1.5.0b5/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/models/openai_itt.py` & `scrapegraphai-1.5.0b5/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/models/openai_tts.py` & `scrapegraphai-1.5.0b5/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/__init__.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/base_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_omni_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_omni_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/search_node_with_context.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/search_node_with_context.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-1.5.0b5/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/cleanup_html.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/cleanup_html.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/logging.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/research_web.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/research_web.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Module for making the request on the web
 """
 import re
 from typing import List
 from langchain_community.tools import DuckDuckGoSearchResults
 from googlesearch import search as google_search
-from yahoo_search import search as yahoo_search
 
 
 def search_on_web(query: str, search_engine: str = "Google", max_results: int = 10) -> List[str]:
     """
     Searches the web for a given query using specified search engine options.
 
     Args:
@@ -39,20 +38,9 @@
     elif search_engine.lower() == "duckduckgo":
         research = DuckDuckGoSearchResults(max_results=max_results)
         res = research.run(query)
 
         links = re.findall(r'https?://[^\s,\]]+', res)
 
         return links
-    elif search_engine.lower() == "yahoo":
-        list_result = yahoo_search(query)
-        results = []
-        for page in list_result.pages:
-            if len(results) >= max_results:  # Check if max_results has already been reached
-                break  # Exit loop if max_results has been reached
-            try:
-                results.append(page.link)
-            except AttributeError:
-                continue
-        return results
     raise ValueError(
         "The only search engines available are DuckDuckGo or Google")
```

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/sys_dynamic_import.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-1.5.0b5/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/scrape_json_ollama.py` & `scrapegraphai-1.5.0b5/tests/graphs/scrape_json_ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_llama3_test.py` & `scrapegraphai-1.5.0b5/tests/graphs/scrape_plain_text_llama3_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/scrape_plain_text_mistral_test.py` & `scrapegraphai-1.5.0b5/tests/graphs/scrape_plain_text_mistral_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/scrape_xml_ollama_test.py` & `scrapegraphai-1.5.0b5/tests/graphs/scrape_xml_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/script_generator_test.py` & `scrapegraphai-1.5.0b5/tests/graphs/script_generator_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/smart_scraper_ollama_test.py` & `scrapegraphai-1.5.0b5/tests/graphs/smart_scraper_ollama_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/inputs/books.xml` & `scrapegraphai-1.5.0b5/tests/graphs/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/inputs/example.json` & `scrapegraphai-1.5.0b5/tests/graphs/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/graphs/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b5/tests/graphs/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/nodes/fetch_node_test.py` & `scrapegraphai-1.5.0b5/tests/nodes/fetch_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/nodes/robot_node_test.py` & `scrapegraphai-1.5.0b5/tests/nodes/robot_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/nodes/search_link_node_test.py` & `scrapegraphai-1.5.0b5/tests/nodes/search_link_node_test.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/nodes/inputs/books.xml` & `scrapegraphai-1.5.0b5/tests/nodes/inputs/books.xml`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/nodes/inputs/example.json` & `scrapegraphai-1.5.0b5/tests/nodes/inputs/example.json`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/nodes/inputs/plain_html_example.txt` & `scrapegraphai-1.5.0b5/tests/nodes/inputs/plain_html_example.txt`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/utils/test_proxy_rotation.py` & `scrapegraphai-1.5.0b5/tests/utils/test_proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/tests/utils/test_sys_dynamic_import.py` & `scrapegraphai-1.5.0b5/tests/utils/test_sys_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/LICENSE` & `scrapegraphai-1.5.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-1.5.0b4/README.md` & `scrapegraphai-1.5.0b5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -164,32 +164,33 @@
 
 ## 🤝 Contributing
 
 Feel free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
 Please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
-[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
+[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/uJN7TYcpNa)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 [![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraphai)
 
 ## 📈 Roadmap
 Check out the project roadmap [here](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/docs/README.md)! 🚀
 
 Wanna visualize the roadmap in a more interactive way? Check out the [markmap](https://markmap.js.org/repl) visualization by copy pasting the markdown content in the editor!
 
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
+
 ## Sponsors
 <div style="text-align: center;">
   <a href="https://serpapi.com?utm_source=scrapegraphai">
     <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/serp_api_logo.png" alt="SerpAPI" style="width: 10%;">
   </a>
   <a href="https://dashboard.statproxies.com/?refferal=scrapegraph">
-    <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/transparent_stat.png" alt="Stats" style="width: 10%;">
+    <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/transparent_stat.png" alt="Stats" style="width: 15%;">
   </a>
 </div>
 
 ## 🎓 Citations
 If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
```

### Comparing `scrapegraphai-1.5.0b4/pyproject.toml` & `scrapegraphai-1.5.0b5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "scrapegraphai"
 
 
-version = "1.5.0b4"
+version = "1.5.0b5"
 
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     { name = "Marco Vinciguerra", email = "mvincig11@gmail.com" },
     { name = "Marco Perini", email = "perinim.98@gmail.com" },
     { name = "Lorenzo Padoan", email = "lorenzo.padoan977@gmail.com" }
@@ -26,15 +26,14 @@
     "tiktoken==0.6.0",
     "tqdm==4.66.4",
     "graphviz==0.20.3",
     "minify-html==0.15.0",
     "free-proxy==1.1.1",
     "playwright==1.43.0",
     "google==3.0.0",
-    "yahoo-search-py==0.3",
     "undetected-playwright==0.3.0",
 ]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://scrapegraphai.com/"
 repository = "https://github.com/VinciGit00/Scrapegraph-ai"
@@ -60,15 +59,15 @@
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.9,<3.12"
+requires-python = ">=3.9,<4.0"
 
 [project.optional-dependencies]
 burr = ["burr[start]==0.19.1"]
 docs = ["sphinx==6.0", "furo==2024.5.6"]
 
 [build-system]
 requires = ["hatchling"]
```

### Comparing `scrapegraphai-1.5.0b4/PKG-INFO` & `scrapegraphai-1.5.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: scrapegraphai
-Version: 1.5.0b4
+Version: 1.5.0b5
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Author-email: Marco Vinciguerra <mvincig11@gmail.com>, Marco Perini <perinim.98@gmail.com>, Lorenzo Padoan <lorenzo.padoan977@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ai,artificial intelligence,gpt,graph,langchain,machine learning,natural language processing,nlp,openai,rag,scrapegraph,scrapegraphai,scraping,web scraping,web scraping library,web scraping tool,webscraping
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <3.12,>=3.9
+Requires-Python: <4.0,>=3.9
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: free-proxy==1.1.1
 Requires-Dist: google==3.0.0
 Requires-Dist: graphviz==0.20.3
 Requires-Dist: html2text==2024.2.26
 Requires-Dist: langchain-anthropic==0.1.11
@@ -26,15 +26,14 @@
 Requires-Dist: minify-html==0.15.0
 Requires-Dist: pandas==2.2.2
 Requires-Dist: playwright==1.43.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: tqdm==4.66.4
 Requires-Dist: undetected-playwright==0.3.0
-Requires-Dist: yahoo-search-py==0.3
 Provides-Extra: burr
 Requires-Dist: burr[start]==0.19.1; extra == 'burr'
 Provides-Extra: docs
 Requires-Dist: furo==2024.5.6; extra == 'docs'
 Requires-Dist: sphinx==6.0; extra == 'docs'
 Description-Content-Type: text/markdown
 
@@ -204,32 +203,33 @@
 
 ## 🤝 Contributing
 
 Feel free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
 Please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
-[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
+[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/uJN7TYcpNa)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
 [![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraphai)
 
 ## 📈 Roadmap
 Check out the project roadmap [here](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/docs/README.md)! 🚀
 
 Wanna visualize the roadmap in a more interactive way? Check out the [markmap](https://markmap.js.org/repl) visualization by copy pasting the markdown content in the editor!
 
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
+
 ## Sponsors
 <div style="text-align: center;">
   <a href="https://serpapi.com?utm_source=scrapegraphai">
     <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/serp_api_logo.png" alt="SerpAPI" style="width: 10%;">
   </a>
   <a href="https://dashboard.statproxies.com/?refferal=scrapegraph">
-    <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/transparent_stat.png" alt="Stats" style="width: 10%;">
+    <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/transparent_stat.png" alt="Stats" style="width: 15%;">
   </a>
 </div>
 
 ## 🎓 Citations
 If you have used our library for research purposes please quote us with the following reference:
 ```text
   @misc{scrapegraph-ai,
```

