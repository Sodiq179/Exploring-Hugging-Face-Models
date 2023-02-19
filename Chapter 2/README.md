## What happens in the pipe line function [Sentiment-Analysis]?
This sections involves the breakdown of what happens in the pipeline function for a sentiment analysis use case.

```python
from transformers import pipeline

classifier = pipeline("sentiment-analysis")
classifier(
    [
        "I've been waiting for a HuggingFace course my whole life.",
        "I hate this so much!",
    ]
)
```

Output:

```python out
[{'label': 'POSITIVE', 'score': 0.9598047137260437},
 {'label': 'NEGATIVE', 'score': 0.9994558095932007}]
```

<div class="flex justify-center">
<img class="block dark:hidden" src="https://huggingface.co/datasets/huggingface-course/documentation-images/resolve/main/en/chapter2/full_nlp_pipeline.svg" alt="The full NLP pipeline: tokenization of text, conversion to IDs, and inference through the Transformer model and the model head."/>
</div>

