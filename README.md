# Project

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./assets/css/styles.css">
</head>
<body>
<div class="difficulty-container">
<ul class="difficulty-list">
    <li class="level">Beginner</li>
    <li class="level selected"><strong>Intermediate</strong></li>
    <li class="level">Advanced</li>
</ul>
</div>
</body>

[![thumbnail](https://img.youtube.com/vi/quJtzVxoMtE/maxresdefault.jpg)](https://www.youtube.com/watch?v=quJtzVxoMtE)

This tutorial demonstrates how to use [spaCy Layout](https://github.com/explosion/spacy-layout), a powerful extension that combines layout detection, OCR, and NLP capabilities into a streamlined spaCy pipeline. Learn how to extract and analyze text from documents while preserving spatial information and document structure.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wjbmattingly/youtube-spacy-layout/blob/main/notebooks/01-demo.ipynb)


# Installation

```bash
git clone github.com/wjbmattingly/youtube-spacy-layout
```

# Quick Code

```python
import spacy
from spacy_layout import spaCyLayout

nlp = spacy.load("en_core_web_sm")
layout = spaCyLayout(nlp)
doc = layout("../data/RG-50.030.0045_trs_en.pdf")
print(doc.text)
```
