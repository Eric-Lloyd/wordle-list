# wordle-list
To fetch list with _curl_ use the following command:
```bash
curl -s https://raw.githubusercontent.com/Eric-Lloyd/wordle-list/main/words-dict.json
```

To fetch list in _Python_ use the following code:
```python
import requests

def fetch_words():
  url = "https://raw.githubusercontent.com/Eric-Lloyd/wordle-list/main/words-dict.json"
  response = requests.get(url)
  return response.json()["words"]

words = fetch_words()
```
