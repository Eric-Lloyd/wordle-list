# wordle-list
To fetch list with _curl_ use the following command:
```bash
curl -s https://raw.githubusercontent.com/Eric-Lloyd/wordle-list/main/words
```

To fetch list in _Python_ use the following code:
```python
import requests

def fetch_words():
  url = "https://raw.githubusercontent.com/Eric-Lloyd/wordle-list/main/words"
  response = requests.get(url)
  return response.text.split("\n")

words = fetch_words()
```
