# RAG AI Python Agent

RAG (Retrieve and Generate) AI Python Agent is an intelligent system designed to retrieve information and generate responses. It utilizes a population dataset to inform its responses and integrates with GPT-3.5 to provide detailed information about the world population, demographics, and specific data about Canada.

## Features

- Data retrieval from structured data sources (CSV files).
- Integration with OpenAI's GPT-3.5 for natural language understanding and response generation.
- Modular tool integration allowing for expandable and customizable data sources.
- Interactive prompt system for real-time query handling.

## Getting Started

Before you run the agent, make sure you have installed all required packages:

```bash
pip install llama-index pypdf python-dotenv pandas
```

### Environment Variables

The application uses environment variables for configuration. Create a `.env` file in the root directory with the following variables:

```plaintext
OPENAI_API_KEY=your_openai_api_key
```

Replace `your_openai_api_key` with your actual OpenAI API key.

### Usage

Execute the script in your terminal:

```bash
python main.py
```

Follow the interactive prompts and enter queries to receive information about world populations and demographics or specific data regarding Canada. To exit the application, type `q`.

### Data Sources

- `population.csv`: Contains world population and demographics data.
- `canada.csv`: Contains detailed data about Canada.

These CSV files are loaded into `PandasQueryEngine` instances to provide an interface for querying the data.

## Modules

The application is comprised of several modules:

- `dotenv`: For loading environment variables from the `.env` file.
- `pandas`: For handling CSV data.
- `llama_index`: Framework for building AI tools and agents.
- `prompts`: For managing and updating query prompts.
- `note_engine`: For note-taking and data aggregation.
- `pdf`: Custom module for processing PDFs (specifically `canada_engine`).

## Contributing

Contributions to the RAG AI Python Agent are welcome! If you have suggestions for improvements or new data sources, feel free to fork the repository and submit a pull request.

## License

This project is open-sourced under the MIT License. See the LICENSE file for more information.

## Contact

For any further queries, please reach out to greg.bolton.28@gmail.com.

Acknowledgments
This project was inspired by the work done in the PythonAgentAI repository by Tech With Tim.