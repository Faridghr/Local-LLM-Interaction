# Project Title: Evaluating and Comparing LLMs on a Local Machine

## Objective
The purpose of this project is to set up and interact with large language models (LLMs) directly on our local machine. Additionally, we compare two different LLM models to determine which one performs better. In this project, we use Ollama as the LLM framework and its different models.

## Project Structure
- **report/**: This directory contains the project [report](report), including documentation and all responses for the following prompts.
- **video/**: Contains [video](video) presentation.

## Setting up LLMs
We begin by setting up the LLMs on our local machines:

### Installation Instructions:
### macOS
1.	Download the [Ollama installer for macOS](https://ollama.com/download/Ollama-darwin.zip).
2.	Extract the downloaded ZIP file.
3.	Open Terminal and navigate to the extracted folder.
4.	Run the following command to install Ollama: ./install.sh

### Windows Preview
1.	Download the [Ollama for Windows](https://ollama.com/download/OllamaSetup.exe) setup executable.
2.	Run the downloaded executable file and follow the on-screen instructions to complete the installation.

### Linux
1.	Open a terminal window.
2.	Run the following command to install Ollama: `curl -fsSL https://ollama.com/install.sh | sh`

### After installing Ollama, you can interact with it via the curl command:

- To run a model: `ollama run [Model-Name]`
- Wait for the model to be pulled
- Input your prompt

For further instructions, visit the [Ollama GitHub page](https://github.com/ollama/ollama).

## Choosing Models
We compare two different Ollama models: llama 3 and Gemma:2b.

1. **llama 3**
Description: An advanced language model with 8 billion parameters, offering robust performance and a wide range of capabilities in a compact size of 4.7 GB. Suitable for diverse natural language processing tasks.
Curl Command: `ollama run llama3`

2. **Gemma:2b**
Description: A versatile language model with 2 billion parameters and a size of 1.4 GB. Designed to deliver efficient and effective performance for various language-related applications while maintaining a smaller computational footprint.
Curl Command: `ollama run gemma:2b`

## Evaluation Criteria
To compare both models, we use the same prompts and evaluate their responses based on the following criteria:

- **Accuracy and Relevance:** How correct and relevant are the responses to the given prompts?
- **Coherence and Fluency:** How logical and smoothly flowing are the responses?
- **Creativity and Originality:** How creative and original are the responses?
- **Consistency:** How consistent are the responses over multiple similar queries?
- **Bias and Fairness:** Are the responses free from inappropriate biases and ethically sound?
- **Robustness:** How well does the model handle ambiguous, tricky, or adversarial inputs?

## Compare Two Models
We input each prompt into both llama 3 and Gemma:2b, capturing the full response from each model. Each response is evaluated using the criteria mentioned above, scores are assigned to quantify the evaluation, and the results are compared to determine the strengths and weaknesses of each model.

## Diverse Set of Prompts
For evaluation, we chose a wide range of prompts:

1. **General Knowledge Questions:** "What are the primary causes of climate change?"
   - Ollama 3 provided a detailed and accurate list of primary causes of climate change, while Gemma:2b's response was less detailed and missed some key points.
   
2. **Conversational Prompts:** "Tell me about your favorite book."
   - Ollama 3 provided detailed book recommendations, showing an understanding of the request. Gemma:2b's response was too brief and didn't provide useful information.
   
3. **Creative Prompts:** "Write a short story about a dragon and a knight."
   - Both models created imaginative stories, but Ollama 3's story was more detailed and engaging.
   
4. **Technical Questions:** "Explain the concept of quantum entanglement."
   - Ollama 3's response was clear and easy to understand, while Gemma:2b's was also clear but slightly less detailed.
   
5. **Ethical Dilemmas:** "Is it ethical to use animals for scientific research? Why or why not?"
   - Both models provided balanced views, but Ollama 3 offered more detailed arguments.
   
6. **Ambiguous or Tricky Prompts:** "Can you explain the meaning of life?"
   - Both responses were clear and well-structured.

Evaluation Table
| Prompt                                    | Criterion          | llama 3 Score | Gemma:2b Score |
|-------------------------------------------|--------------------|---------------|----------------|
| What are the primary causes of climate change? | Accuracy           | 5             | 4              |
| Tell me about your favorite book.         | Coherence          | 4             | 2              |
| Write a short story about a dragon and a knight. | Creativity         | 5             | 4              |
| Explain the concept of quantum entanglement. | Technical Depth    | 5             | 3              |
| Is it ethical to use animals for scientific research? | Bias and Fairness  | 4             | 3              |
| Can you explain the meaning of life?      | Robustness         | 4             | 4              |

## Summary Comparison
In general, Ollama 3 tends to provide more detailed, comprehensive, and engaging responses compared to Gemma:2b. Ollama 3's answers are well-organized, clear, and cover a wider range of aspects for each prompt. It excels in accuracy and depth, making it more suitable for tasks requiring thorough explanations and creative storytelling. On the other hand, Gemma:2b's responses are shorter and less detailed, making it less effective for in-depth queries but potentially faster for simpler, straightforward questions.

## Acknowledgment
This LLM model was originally published by [Ollama](https://github.com/ollama/ollama).
