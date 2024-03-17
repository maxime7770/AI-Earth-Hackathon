# AI-Earth-Hackathon


In response to the proliferation of circular solutions, there's a pressing need to assess their efficacy. With numerous options available, determining the most effective ones is crucial for advancing sustainable practices. As circular economy initiatives gain momentum, the abundance of available solutions necessitates a reliable method to rank and prioritize them effectively. By evaluating metrics such as relevance to problem, impact, feasibility, and scalability, organizations can make informed decisions to drive meaningful environmental change. This tool leverages NLP techniques, Zero Shot Classification, and Gemini Pro LLM to evaluate circular economy solutions on the aforementionned metrics and more with each metric being scored between 1-3 and an average score being used to rank the solutions.


## How to run the demo locally?

### 1. Install the dependencies

- Use python 3.9
- Install the dependencies with `pip install -r requirements.txt`

### 2. Use your own API key

- Create a file named `secrets.toml` in the `.streamlit` folder
- Write your API key with the following format:
```
GEMINI_API_KEY = "xxx"
```

### 2. Run the demo

- Run the demo with `streamlit run main.py`


## How to run the demo online?

- Simply use the following link: https://ai-earth-hackathon.streamlit.app/


## How to use the demo?

- You can either manually enter a problem statement and the proposed solution, or you can upload a CSV file with the same format as the training data.
- When clicking on the "Evaluate" button, our tool will use the different models and combine their results to provide scores for the different criteria, and an overall score.
- If the user has manually entered one problem and solution, the "Explanations of the scores" section provides interpretability for the scores using the Gemini API.
- If the user has uploaded a CSV file, we instead provide a new CSV file with the scores for each row, that the user can download.
