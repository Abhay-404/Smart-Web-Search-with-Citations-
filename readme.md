# AI-Powered Budget Web Search:😎

AI-powered web search application that provides comprehensive answers to your questions, along with relevant citations, all while being **significantly more cheaper** than alternatives like Google with grounding or ChatGPT web search.

<div>
    <a href="https://www.loom.com/share/4828d289aa234046930e19413aa3eb8f">
      <p></p>
    </a>
    <a href="https://www.loom.com/share/4828d289aa234046930e19413aa3eb8f">
      <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/4828d289aa234046930e19413aa3eb8f-98ff2633f0b0c283-full-play.gif">
    </a>
  </div>

## Features

- **Intelligent Query Analysis:** Uses Google AI's Gemini model to analyze user queries and determine if external web search is needed.
- **Atomic Question Decomposition:** Breaks down complex queries into smaller, atomic questions for focused research.
- **DuckDuckGo Search Integration:** Leverages DuckDuckGo for retrieving relevant search results.
- **Full Content Extraction:** Extracts the full content of web pages for deeper analysis.
- **Flash 2.0 Summarization:** Utilizes Flash 2.0 to generate concise summaries of search results in the context of each atomic question.
- **Citation Generation:** Provides clear citations for all information used in the final answer.
- **Markdown Support:** Formats the final answer and summaries using Markdown syntax for better readability.
- **Interactive UI:** Offers a user-friendly interface within Google Colab to input queries and view results.
- **Cost-Effective:**  **Significantly cheaper** than using Google with grounding or ChatGPT web search, making it ideal for budget-conscious users and researchers.


**Here's how saves you money:**

* **Reduced API Costs:** By using DuckDuckGo for search and Flash 2.0 for summarization, minimizes reliance on expensive APIs.
* **Efficient Processing:** The intelligent query analysis and atomic question decomposition help focus the search and reduce unnecessary computations.

## How it Works
![mermaid-diagram-2025-03-30-191814](https://github.com/user-attachments/assets/709aa95c-8db4-440c-88c2-8c5585922b80)

1. **Query Input:** The user enters a query in the search interface.
2. **Query Analysis:** The Gemini model determines if web search is needed based on the query's complexity and recency requirements.
3. **Atomic Questions:** If search is required, the query is broken down into atomic questions.
4. **Web Search:** DuckDuckGo is used to search for relevant web pages for each atomic question.
5. **Content Extraction:** The full content of the search results is extracted.
6. **Summarization:** Flash 2.0 summarizes the content of each search result in the context of the corresponding atomic question.
7. **Answer Synthesis:** Flash 2.0 combines the summaries and citations to generate a final answer to the user's original query.
8. **Output:** The answer, along with citations, is displayed in the UI, formatted using Markdown.

## Usage

1. **Set API Key:** Replace `YOUR_API_KEY_HERE` with your actual Google AI API key in the code.
2. **Run the App:** Execute the `run_search_app()` function.
3. **Enter Query:** Type your question in the search bar and click "Search".
4. **View Results:** The answer will be displayed along with citations and optional debug information.

## Dependencies

- `google-generativeai`
- `duckduckgo-search`
- `beautifulsoup4`
- `backoff`
- `ipywidgets`
- `requests`
- `tqdm`
- `ipython-autotime`
- `markdown2`

## Things to Do :
1. Implement Reranker for Better Search Result Prioritization
2. Caching Queries and Summaries
3. Maybe try to build deep research agent??
