## Outputs

```python
import enalsis
```

The variable `taxt_para` that we will be using to demonstrate our package's outputs.

```text
India is a vast and diverse country located in South Asia, known for its rich history, diverse cultures, and varied landscapes. With a population of over $ 1.3 billion people, India is the second-most populous country in the world. The country is characterized by a harmonious blend of tradition and modernity, where ancient customs coexist with rapidly evolving urban lifestyles.

Geographically, India boasts a wide range of terrains, from the snow-capped Himalayan mountains in the north to the tropical beaches in the south. The country is home to a myriad of ecosystems, supporting a diverse array of flora and fauna. The Ganges, one of the holiest rivers in Hinduism, flows through the heart of the country, playing a vital role in the cultural and spiritual fabric of India.

India's rich cultural heritage is reflected in its numerous festivals, art forms, and classical dance and music traditions. The country has a long history of contributions to science, mathematics, literature, and philosophy. Ancient texts such as the Vedas and Upanishads have left an indelible mark on the intellectual landscape of the world.

The Indian economy has undergone significant transformation in recent decades, emerging as one of the world's fastest-growing major economies. Information technology, software services, and a burgeoning startup ecosystem have contributed to India's position in the global economy. Despite these advancements, India faces challenges related to poverty, healthcare, and environmental sustainability, prompting ongoing efforts for inclusive development.

India's political landscape is characterized by a robust democratic system, with a diverse array of political parties. The country gained independence from British rule in 1947, led by Mahatma Gandhi and other prominent leaders. India's commitment to democracy is evident in its vibrant elections, where millions of citizens participate in shaping the nation's future.
```

-----

### Extract entities from the text

```python
print(enalsis.get_entities(text_para))
```

Output - The output format is a list of tuples: (text_entity, entity_label).

```python
[
    ("India", "GPE"),
    ("South Asia", "LOC"),
    ("over $ 1.3 billion", "MONEY"),
    ("India", "GPE"),
    ("second", "ORDINAL"),
    ("Geographically", "ORG"),
    ("India", "GPE"),
    ("Himalayan", "NORP"),
    ("Ganges", "ORG"),
    ("Hinduism", "GPE"),
    ("India", "GPE"),
    ("India", "GPE"),
    ("Upanishads", "PERSON"),
    ("Indian", "NORP"),
    ("recent decades", "DATE"),
    ("one", "CARDINAL"),
    ("India", "GPE"),
    ("India", "GPE"),
    ("healthcare", "ORG"),
    ("India", "GPE"),
    ("British", "NORP"),
    ("1947", "DATE"),
    ("Mahatma Gandhi", "PERSON"),
    ("India", "GPE"),
    ("millions", "CARDINAL"),
]
```

-----

### Extract sentences from the text


```python
print(enalsis.get_sentences(text_para))
```

Output - The output format is a list of strings, where each string represents sentences of text.

```python
[
    "India is a vast and diverse country located in South Asia, known for its rich history, diverse cultures, and varied landscapes.",
    "With a population of over $ 1.3 billion people, India is the second-most populous country in the world.",
    "The country is characterized by a harmonious blend of tradition and modernity, where ancient customs coexist with rapidly evolving urban lifestyles.\n\n",
    "Geographically, India boasts a wide range of terrains, from the snow-capped Himalayan mountains in the north to the tropical beaches in the south.",
    "The country is home to a myriad of ecosystems, supporting a diverse array of flora and fauna.",
    "The Ganges, one of the holiest rivers in Hinduism, flows through the heart of the country, playing a vital role in the cultural and spiritual fabric of India.\n\n",
    "India's rich cultural heritage is reflected in its numerous festivals, art forms, and classical dance and music traditions.",
    "The country has a long history of contributions to science, mathematics, literature, and philosophy.",
    "Ancient texts such as the Vedas and Upanishads have left an indelible mark on the intellectual landscape of the world.\n\n",
    "The Indian economy has undergone significant transformation in recent decades, emerging as one of the world's fastest-growing major economies.",
    "Information technology, software services, and a burgeoning startup ecosystem have contributed to India's position in the global economy.",
    "Despite these advancements, India faces challenges related to poverty, healthcare, and environmental sustainability, prompting ongoing efforts for inclusive development.\n\n",
    "India's political landscape is characterized by a robust democratic system, with a diverse array of political parties.",
    "The country gained independence from British rule in 1947, led by Mahatma Gandhi and other prominent leaders.",
    "India's commitment to democracy is evident in its vibrant elections, where millions of citizens participate in shaping the nation's future.",
]
```

-----

### Extract adjectives from the text

```python
print(enalsis.get_adjectives(text_para))
```


Output - The output format is a list of strings, where each string represents adjectives extracted from the given text.

```python
[
    "vast",
    "diverse",
    "rich",
    "diverse",
    "varied",
    "populous",
    "harmonious",
    "ancient",
    "urban",
    "wide",
    "Himalayan",
    "tropical",
    "diverse",
    "holiest",
    "vital",
    "cultural",
    "spiritual",
    "rich",
    "cultural",
    "numerous",
    "classical",
    "long",
    "Ancient",
    "such",
    "indelible",
    "intellectual",
    "Indian",
    "significant",
    "recent",
    "major",
    "global",
    "environmental",
    "ongoing",
    "inclusive",
    "political",
    "robust",
    "democratic",
    "diverse",
    "political",
    "British",
    "other",
    "prominent",
    "evident",
    "vibrant",
]
```

-----

### Extract adverbs from the text

```python
print(enalsis.get_adverbs(text_para))
```

Output - The output format is a list of strings, where each string represents adverbs extracted from the given text.

```python
['second', 'most', 'rapidly', 'fastest']
```

-----

### Extract nouns from the text

```python
print(enalsis.get_nouns(text_para))
```

Output - The output format is a list of strings, where each string represents nouns extracted from the given sentences.

```python
[
    "country",
    "history",
    "cultures",
    "landscapes",
    "population",
    "people",
    "country",
    "world",
    "country",
    "blend",
    "tradition",
    "modernity",
    "customs",
    "lifestyles",
    "range",
    "terrains",
    "snow",
    "mountains",
    "north",
    "beaches",
    "south",
    "country",
    "home",
    "myriad",
    "ecosystems",
    "array",
    "flora",
    "fauna",
    "rivers",
    "heart",
    "country",
    "role",
    "fabric",
    "heritage",
    "festivals",
    "art",
    "forms",
    "dance",
    "music",
    "traditions",
    "country",
    "history",
    "contributions",
    "science",
    "mathematics",
    "literature",
    "philosophy",
    "texts",
    "mark",
    "landscape",
    "world",
    "economy",
    "transformation",
    "decades",
    "world",
    "economies",
    "Information",
    "technology",
    "software",
    "services",
    "startup",
    "ecosystem",
    "position",
    "economy",
    "advancements",
    "challenges",
    "poverty",
    "healthcare",
    "sustainability",
    "efforts",
    "development",
    "landscape",
    "system",
    "array",
    "parties",
    "country",
    "independence",
    "rule",
    "leaders",
    "commitment",
    "democracy",
    "elections",
    "millions",
    "citizens",
    "nation",
    "future",
]
```

-----

### Extract pronouns from the text

```python
print(enalsis.get_pronouns(text_para))
```

Output - The output format is a list of strings, where each string represents pronouns extracted from the given text.

```python
[
    "its",
    "its",
    "its",
]
```

-----

### Extract proper nouns from the text

```python
print(enalsis.get_proper_nouns(text_para))
```

Output - The output format is a list of strings, where each string represents proper nouns extracted from the given text.

```python
[
    "India",
    "South",
    "Asia",
    "India",
    "Geographically",
    "India",
    "Ganges",
    "Hinduism",
    "India",
    "India",
    "Vedas",
    "Upanishads",
    "India",
    "India",
    "India",
    "Mahatma",
    "Gandhi",
    "India",
]
```

-----

### Extract verbs from the text

```python
print(enalsis.get_verbs(text_para))
```

Output - The output format is a list of strings, where each string represents verbs extracted from the given text.

```python
[
    "located",
    "known",
    "characterized",
    "coexist",
    "evolving",
    "boasts",
    "capped",
    "supporting",
    "flows",
    "playing",
    "reflected",
    "has",
    "left",
    "undergone",
    "emerging",
    "growing",
    "burgeoning",
    "contributed",
    "faces",
    "related",
    "prompting",
    "characterized",
    "gained",
    "led",
    "participate",
    "shaping",
]
```

-----

### Extract numbers from the text

```python
print(enalsis.get_numbers(text_para))
```

Output - The output format is a list of strings, where each string represents numbers extracted from the given text.

```python
[
    "1.3",
    "billion",
    "one",
    "one",
    "1947",
]
```

-----

### Detect language of the text

```python
print(enalsis.detect_language(text_para))
```

Output - The output format is the language name in which the given text is written.

```python
English
```

-----

### Perform syntax tree analysis on the given text

```python
print(enalsis.parse_syntax_tree(text_para))
```

Output - The output format is a list of dictionaries, where each dictionary represents a token with its corresponding dependency parsing information, including the text(`text`), dependency label (`dep`), part of speech tag (`pos`), and head token (`head`).

```python
{
    {"text": "India", "dep": "nsubj", "pos": "PROPN", "head": "is"},
    {"text": "is", "dep": "ROOT", "pos": "AUX", "head": "is"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "country"},
    {"text": "vast", "dep": "amod", "pos": "ADJ", "head": "country"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "vast"},
    {"text": "diverse", "dep": "conj", "pos": "ADJ", "head": "vast"},
    {"text": "country", "dep": "attr", "pos": "NOUN", "head": "is"},
    {"text": "located", "dep": "acl", "pos": "VERB", "head": "country"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "located"},
    {"text": "South", "dep": "compound", "pos": "PROPN", "head": "Asia"},
    {"text": "Asia", "dep": "pobj", "pos": "PROPN", "head": "in"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "Asia"},
    {"text": "known", "dep": "acl", "pos": "VERB", "head": "country"},
    {"text": "for", "dep": "prep", "pos": "ADP", "head": "known"},
    {"text": "its", "dep": "poss", "pos": "PRON", "head": "history"},
    {"text": "rich", "dep": "amod", "pos": "ADJ", "head": "history"},
    {"text": "history", "dep": "pobj", "pos": "NOUN", "head": "for"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "history"},
    {"text": "diverse", "dep": "amod", "pos": "ADJ", "head": "cultures"},
    {"text": "cultures", "dep": "conj", "pos": "NOUN", "head": "history"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "cultures"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "cultures"},
    {"text": "varied", "dep": "amod", "pos": "ADJ", "head": "landscapes"},
    {"text": "landscapes", "dep": "conj", "pos": "NOUN", "head": "cultures"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "is"},
    {"text": "With", "dep": "prep", "pos": "ADP", "head": "is"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "population"},
    {"text": "population", "dep": "pobj", "pos": "NOUN", "head": "With"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "population"},
    {"text": "over", "dep": "quantmod", "pos": "ADP", "head": "billion"},
    {"text": "$", "dep": "quantmod", "pos": "SYM", "head": "billion"},
    {"text": "1.3", "dep": "compound", "pos": "NUM", "head": "billion"},
    {"text": "billion", "dep": "nummod", "pos": "NUM", "head": "people"},
    {"text": "people", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "is"},
    {"text": "India", "dep": "nsubj", "pos": "PROPN", "head": "is"},
    {"text": "is", "dep": "ROOT", "pos": "AUX", "head": "is"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "country"},
    {"text": "second", "dep": "advmod", "pos": "ADV", "head": "most"},
    {"text": "-", "dep": "punct", "pos": "PUNCT", "head": "most"},
    {"text": "most", "dep": "advmod", "pos": "ADV", "head": "populous"},
    {"text": "populous", "dep": "amod", "pos": "ADJ", "head": "country"},
    {"text": "country", "dep": "attr", "pos": "NOUN", "head": "is"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "country"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "world"},
    {"text": "world", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "is"},
    {"text": "The", "dep": "det", "pos": "DET", "head": "country"},
    {"text": "country", "dep": "nsubjpass", "pos": "NOUN", "head": "characterized"},
    {"text": "is", "dep": "auxpass", "pos": "AUX", "head": "characterized"},
    {"text": "characterized", "dep": "ROOT", "pos": "VERB", "head": "characterized"},
    {"text": "by", "dep": "agent", "pos": "ADP", "head": "characterized"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "blend"},
    {"text": "harmonious", "dep": "amod", "pos": "ADJ", "head": "blend"},
    {"text": "blend", "dep": "pobj", "pos": "NOUN", "head": "by"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "blend"},
    {"text": "tradition", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "tradition"},
    {"text": "modernity", "dep": "conj", "pos": "NOUN", "head": "tradition"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "blend"},
    {"text": "where", "dep": "advmod", "pos": "SCONJ", "head": "coexist"},
    {"text": "ancient", "dep": "amod", "pos": "ADJ", "head": "customs"},
    {"text": "customs", "dep": "nsubj", "pos": "NOUN", "head": "coexist"},
    {"text": "coexist", "dep": "relcl", "pos": "VERB", "head": "blend"},
    {"text": "with", "dep": "prep", "pos": "ADP", "head": "coexist"},
    {"text": "rapidly", "dep": "advmod", "pos": "ADV", "head": "evolving"},
    {"text": "evolving", "dep": "pcomp", "pos": "VERB", "head": "with"},
    {"text": "urban", "dep": "amod", "pos": "ADJ", "head": "lifestyles"},
    {"text": "lifestyles", "dep": "dobj", "pos": "NOUN", "head": "evolving"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "characterized"},
    {"text": "\n\n", "dep": "dep", "pos": "SPACE", "head": "."},
    {"text": "Geographically", "dep": "advmod", "pos": "PROPN", "head": "boasts"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "boasts"},
    {"text": "India", "dep": "nsubj", "pos": "PROPN", "head": "boasts"},
    {"text": "boasts", "dep": "ROOT", "pos": "VERB", "head": "boasts"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "range"},
    {"text": "wide", "dep": "amod", "pos": "ADJ", "head": "range"},
    {"text": "range", "dep": "dobj", "pos": "NOUN", "head": "boasts"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "range"},
    {"text": "terrains", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "range"},
    {"text": "from", "dep": "prep", "pos": "ADP", "head": "range"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "mountains"},
    {"text": "snow", "dep": "npadvmod", "pos": "NOUN", "head": "capped"},
    {"text": "-", "dep": "punct", "pos": "PUNCT", "head": "capped"},
    {"text": "capped", "dep": "amod", "pos": "VERB", "head": "mountains"},
    {"text": "Himalayan", "dep": "amod", "pos": "ADJ", "head": "mountains"},
    {"text": "mountains", "dep": "pobj", "pos": "NOUN", "head": "from"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "mountains"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "north"},
    {"text": "north", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": "to", "dep": "prep", "pos": "ADP", "head": "from"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "beaches"},
    {"text": "tropical", "dep": "amod", "pos": "ADJ", "head": "beaches"},
    {"text": "beaches", "dep": "pobj", "pos": "NOUN", "head": "to"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "beaches"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "south"},
    {"text": "south", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "boasts"},
    {"text": "The", "dep": "det", "pos": "DET", "head": "country"},
    {"text": "country", "dep": "nsubj", "pos": "NOUN", "head": "is"},
    {"text": "is", "dep": "ROOT", "pos": "AUX", "head": "is"},
    {"text": "home", "dep": "advmod", "pos": "NOUN", "head": "is"},
    {"text": "to", "dep": "prep", "pos": "ADP", "head": "home"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "myriad"},
    {"text": "myriad", "dep": "pobj", "pos": "NOUN", "head": "to"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "myriad"},
    {"text": "ecosystems", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "is"},
    {"text": "supporting", "dep": "advcl", "pos": "VERB", "head": "is"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "array"},
    {"text": "diverse", "dep": "amod", "pos": "ADJ", "head": "array"},
    {"text": "array", "dep": "dobj", "pos": "NOUN", "head": "supporting"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "array"},
    {"text": "flora", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "flora"},
    {"text": "fauna", "dep": "conj", "pos": "NOUN", "head": "flora"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "is"},
    {"text": "The", "dep": "det", "pos": "DET", "head": "Ganges"},
    {"text": "Ganges", "dep": "nsubj", "pos": "PROPN", "head": "flows"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "Ganges"},
    {"text": "one", "dep": "appos", "pos": "NUM", "head": "Ganges"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "one"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "rivers"},
    {"text": "holiest", "dep": "amod", "pos": "ADJ", "head": "rivers"},
    {"text": "rivers", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "rivers"},
    {"text": "Hinduism", "dep": "pobj", "pos": "PROPN", "head": "in"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "Ganges"},
    {"text": "flows", "dep": "ROOT", "pos": "VERB", "head": "flows"},
    {"text": "through", "dep": "prep", "pos": "ADP", "head": "flows"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "heart"},
    {"text": "heart", "dep": "pobj", "pos": "NOUN", "head": "through"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "heart"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "country"},
    {"text": "country", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "flows"},
    {"text": "playing", "dep": "advcl", "pos": "VERB", "head": "flows"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "role"},
    {"text": "vital", "dep": "amod", "pos": "ADJ", "head": "role"},
    {"text": "role", "dep": "dobj", "pos": "NOUN", "head": "playing"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "playing"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "fabric"},
    {"text": "cultural", "dep": "amod", "pos": "ADJ", "head": "fabric"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "cultural"},
    {"text": "spiritual", "dep": "conj", "pos": "ADJ", "head": "cultural"},
    {"text": "fabric", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "fabric"},
    {"text": "India", "dep": "pobj", "pos": "PROPN", "head": "of"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "flows"},
    {"text": "\n\n", "dep": "dep", "pos": "SPACE", "head": "."},
    {"text": "India", "dep": "poss", "pos": "PROPN", "head": "heritage"},
    {"text": "'s", "dep": "case", "pos": "PART", "head": "India"},
    {"text": "rich", "dep": "amod", "pos": "ADJ", "head": "heritage"},
    {"text": "cultural", "dep": "amod", "pos": "ADJ", "head": "heritage"},
    {"text": "heritage", "dep": "nsubjpass", "pos": "NOUN", "head": "reflected"},
    {"text": "is", "dep": "auxpass", "pos": "AUX", "head": "reflected"},
    {"text": "reflected", "dep": "ROOT", "pos": "VERB", "head": "reflected"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "reflected"},
    {"text": "its", "dep": "poss", "pos": "PRON", "head": "festivals"},
    {"text": "numerous", "dep": "amod", "pos": "ADJ", "head": "festivals"},
    {"text": "festivals", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "festivals"},
    {"text": "art", "dep": "compound", "pos": "NOUN", "head": "forms"},
    {"text": "forms", "dep": "conj", "pos": "NOUN", "head": "festivals"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "forms"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "forms"},
    {"text": "classical", "dep": "amod", "pos": "ADJ", "head": "dance"},
    {"text": "dance", "dep": "nmod", "pos": "NOUN", "head": "traditions"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "dance"},
    {"text": "music", "dep": "conj", "pos": "NOUN", "head": "dance"},
    {"text": "traditions", "dep": "conj", "pos": "NOUN", "head": "forms"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "reflected"},
    {"text": "The", "dep": "det", "pos": "DET", "head": "country"},
    {"text": "country", "dep": "nsubj", "pos": "NOUN", "head": "has"},
    {"text": "has", "dep": "ROOT", "pos": "VERB", "head": "has"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "history"},
    {"text": "long", "dep": "amod", "pos": "ADJ", "head": "history"},
    {"text": "history", "dep": "dobj", "pos": "NOUN", "head": "has"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "history"},
    {"text": "contributions", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": "to", "dep": "prep", "pos": "ADP", "head": "contributions"},
    {"text": "science", "dep": "pobj", "pos": "NOUN", "head": "to"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "science"},
    {"text": "mathematics", "dep": "conj", "pos": "NOUN", "head": "science"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "mathematics"},
    {"text": "literature", "dep": "conj", "pos": "NOUN", "head": "mathematics"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "literature"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "literature"},
    {"text": "philosophy", "dep": "conj", "pos": "NOUN", "head": "literature"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "has"},
    {"text": "Ancient", "dep": "amod", "pos": "ADJ", "head": "texts"},
    {"text": "texts", "dep": "nsubj", "pos": "NOUN", "head": "left"},
    {"text": "such", "dep": "amod", "pos": "ADJ", "head": "as"},
    {"text": "as", "dep": "prep", "pos": "ADP", "head": "texts"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "Vedas"},
    {"text": "Vedas", "dep": "pobj", "pos": "PROPN", "head": "as"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "Vedas"},
    {"text": "Upanishads", "dep": "conj", "pos": "PROPN", "head": "Vedas"},
    {"text": "have", "dep": "aux", "pos": "AUX", "head": "left"},
    {"text": "left", "dep": "ROOT", "pos": "VERB", "head": "left"},
    {"text": "an", "dep": "det", "pos": "DET", "head": "mark"},
    {"text": "indelible", "dep": "amod", "pos": "ADJ", "head": "mark"},
    {"text": "mark", "dep": "dobj", "pos": "NOUN", "head": "left"},
    {"text": "on", "dep": "prep", "pos": "ADP", "head": "left"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "landscape"},
    {"text": "intellectual", "dep": "amod", "pos": "ADJ", "head": "landscape"},
    {"text": "landscape", "dep": "pobj", "pos": "NOUN", "head": "on"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "landscape"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "world"},
    {"text": "world", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "left"},
    {"text": "\n\n", "dep": "dep", "pos": "SPACE", "head": "."},
    {"text": "The", "dep": "det", "pos": "DET", "head": "economy"},
    {"text": "Indian", "dep": "amod", "pos": "ADJ", "head": "economy"},
    {"text": "economy", "dep": "nsubj", "pos": "NOUN", "head": "undergone"},
    {"text": "has", "dep": "aux", "pos": "AUX", "head": "undergone"},
    {"text": "undergone", "dep": "ROOT", "pos": "VERB", "head": "undergone"},
    {"text": "significant", "dep": "amod", "pos": "ADJ", "head": "transformation"},
    {"text": "transformation", "dep": "dobj", "pos": "NOUN", "head": "undergone"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "undergone"},
    {"text": "recent", "dep": "amod", "pos": "ADJ", "head": "decades"},
    {"text": "decades", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "undergone"},
    {"text": "emerging", "dep": "advcl", "pos": "VERB", "head": "undergone"},
    {"text": "as", "dep": "prep", "pos": "ADP", "head": "emerging"},
    {"text": "one", "dep": "pobj", "pos": "NUM", "head": "as"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "one"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "world"},
    {"text": "world", "dep": "poss", "pos": "NOUN", "head": "economies"},
    {"text": "'s", "dep": "case", "pos": "PART", "head": "world"},
    {"text": "fastest", "dep": "advmod", "pos": "ADV", "head": "growing"},
    {"text": "-", "dep": "punct", "pos": "PUNCT", "head": "growing"},
    {"text": "growing", "dep": "amod", "pos": "VERB", "head": "economies"},
    {"text": "major", "dep": "amod", "pos": "ADJ", "head": "economies"},
    {"text": "economies", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "undergone"},
    {"text": "Information", "dep": "compound", "pos": "NOUN", "head": "technology"},
    {"text": "technology", "dep": "nsubj", "pos": "NOUN", "head": "contributed"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "technology"},
    {"text": "software", "dep": "compound", "pos": "NOUN", "head": "services"},
    {"text": "services", "dep": "conj", "pos": "NOUN", "head": "technology"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "services"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "services"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "ecosystem"},
    {"text": "burgeoning", "dep": "amod", "pos": "VERB", "head": "ecosystem"},
    {"text": "startup", "dep": "compound", "pos": "NOUN", "head": "ecosystem"},
    {"text": "ecosystem", "dep": "conj", "pos": "NOUN", "head": "services"},
    {"text": "have", "dep": "aux", "pos": "AUX", "head": "contributed"},
    {"text": "contributed", "dep": "ROOT", "pos": "VERB", "head": "contributed"},
    {"text": "to", "dep": "prep", "pos": "ADP", "head": "contributed"},
    {"text": "India", "dep": "poss", "pos": "PROPN", "head": "position"},
    {"text": "'s", "dep": "case", "pos": "PART", "head": "India"},
    {"text": "position", "dep": "pobj", "pos": "NOUN", "head": "to"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "position"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "economy"},
    {"text": "global", "dep": "amod", "pos": "ADJ", "head": "economy"},
    {"text": "economy", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "contributed"},
    {"text": "Despite", "dep": "prep", "pos": "SCONJ", "head": "faces"},
    {"text": "these", "dep": "det", "pos": "DET", "head": "advancements"},
    {"text": "advancements", "dep": "pobj", "pos": "NOUN", "head": "Despite"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "faces"},
    {"text": "India", "dep": "nsubj", "pos": "PROPN", "head": "faces"},
    {"text": "faces", "dep": "ROOT", "pos": "VERB", "head": "faces"},
    {"text": "challenges", "dep": "dobj", "pos": "NOUN", "head": "faces"},
    {"text": "related", "dep": "acl", "pos": "VERB", "head": "challenges"},
    {"text": "to", "dep": "prep", "pos": "ADP", "head": "related"},
    {"text": "poverty", "dep": "pobj", "pos": "NOUN", "head": "to"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "poverty"},
    {"text": "healthcare", "dep": "conj", "pos": "NOUN", "head": "poverty"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "healthcare"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "healthcare"},
    {"text": "environmental", "dep": "amod", "pos": "ADJ", "head": "sustainability"},
    {"text": "sustainability", "dep": "conj", "pos": "NOUN", "head": "healthcare"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "faces"},
    {"text": "prompting", "dep": "advcl", "pos": "VERB", "head": "faces"},
    {"text": "ongoing", "dep": "amod", "pos": "ADJ", "head": "efforts"},
    {"text": "efforts", "dep": "dobj", "pos": "NOUN", "head": "prompting"},
    {"text": "for", "dep": "prep", "pos": "ADP", "head": "efforts"},
    {"text": "inclusive", "dep": "amod", "pos": "ADJ", "head": "development"},
    {"text": "development", "dep": "pobj", "pos": "NOUN", "head": "for"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "faces"},
    {"text": "\n\n", "dep": "dep", "pos": "SPACE", "head": "."},
    {"text": "India", "dep": "poss", "pos": "PROPN", "head": "landscape"},
    {"text": "'s", "dep": "case", "pos": "PART", "head": "India"},
    {"text": "political", "dep": "amod", "pos": "ADJ", "head": "landscape"},
    {"text": "landscape", "dep": "nsubjpass", "pos": "NOUN", "head": "characterized"},
    {"text": "is", "dep": "auxpass", "pos": "AUX", "head": "characterized"},
    {"text": "characterized", "dep": "ROOT", "pos": "VERB", "head": "characterized"},
    {"text": "by", "dep": "agent", "pos": "ADP", "head": "characterized"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "system"},
    {"text": "robust", "dep": "amod", "pos": "ADJ", "head": "system"},
    {"text": "democratic", "dep": "amod", "pos": "ADJ", "head": "system"},
    {"text": "system", "dep": "pobj", "pos": "NOUN", "head": "by"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "characterized"},
    {"text": "with", "dep": "prep", "pos": "ADP", "head": "characterized"},
    {"text": "a", "dep": "det", "pos": "DET", "head": "array"},
    {"text": "diverse", "dep": "amod", "pos": "ADJ", "head": "array"},
    {"text": "array", "dep": "pobj", "pos": "NOUN", "head": "with"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "array"},
    {"text": "political", "dep": "amod", "pos": "ADJ", "head": "parties"},
    {"text": "parties", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "characterized"},
    {"text": "The", "dep": "det", "pos": "DET", "head": "country"},
    {"text": "country", "dep": "nsubj", "pos": "NOUN", "head": "gained"},
    {"text": "gained", "dep": "ROOT", "pos": "VERB", "head": "gained"},
    {"text": "independence", "dep": "dobj", "pos": "NOUN", "head": "gained"},
    {"text": "from", "dep": "prep", "pos": "ADP", "head": "gained"},
    {"text": "British", "dep": "amod", "pos": "ADJ", "head": "rule"},
    {"text": "rule", "dep": "pobj", "pos": "NOUN", "head": "from"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "gained"},
    {"text": "1947", "dep": "pobj", "pos": "NUM", "head": "in"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "gained"},
    {"text": "led", "dep": "advcl", "pos": "VERB", "head": "gained"},
    {"text": "by", "dep": "agent", "pos": "ADP", "head": "led"},
    {"text": "Mahatma", "dep": "compound", "pos": "PROPN", "head": "Gandhi"},
    {"text": "Gandhi", "dep": "pobj", "pos": "PROPN", "head": "by"},
    {"text": "and", "dep": "cc", "pos": "CCONJ", "head": "Gandhi"},
    {"text": "other", "dep": "amod", "pos": "ADJ", "head": "leaders"},
    {"text": "prominent", "dep": "amod", "pos": "ADJ", "head": "leaders"},
    {"text": "leaders", "dep": "conj", "pos": "NOUN", "head": "Gandhi"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "gained"},
    {"text": "India", "dep": "poss", "pos": "PROPN", "head": "commitment"},
    {"text": "'s", "dep": "case", "pos": "PART", "head": "India"},
    {"text": "commitment", "dep": "nsubj", "pos": "NOUN", "head": "is"},
    {"text": "to", "dep": "prep", "pos": "ADP", "head": "commitment"},
    {"text": "democracy", "dep": "pobj", "pos": "NOUN", "head": "to"},
    {"text": "is", "dep": "ROOT", "pos": "AUX", "head": "is"},
    {"text": "evident", "dep": "acomp", "pos": "ADJ", "head": "is"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "is"},
    {"text": "its", "dep": "poss", "pos": "PRON", "head": "elections"},
    {"text": "vibrant", "dep": "amod", "pos": "ADJ", "head": "elections"},
    {"text": "elections", "dep": "pobj", "pos": "NOUN", "head": "in"},
    {"text": ",", "dep": "punct", "pos": "PUNCT", "head": "elections"},
    {"text": "where", "dep": "advmod", "pos": "SCONJ", "head": "participate"},
    {"text": "millions", "dep": "nsubj", "pos": "NOUN", "head": "participate"},
    {"text": "of", "dep": "prep", "pos": "ADP", "head": "millions"},
    {"text": "citizens", "dep": "pobj", "pos": "NOUN", "head": "of"},
    {"text": "participate", "dep": "relcl", "pos": "VERB", "head": "elections"},
    {"text": "in", "dep": "prep", "pos": "ADP", "head": "participate"},
    {"text": "shaping", "dep": "pcomp", "pos": "VERB", "head": "in"},
    {"text": "the", "dep": "det", "pos": "DET", "head": "nation"},
    {"text": "nation", "dep": "poss", "pos": "NOUN", "head": "future"},
    {"text": "'s", "dep": "case", "pos": "PART", "head": "nation"},
    {"text": "future", "dep": "dobj", "pos": "NOUN", "head": "shaping"},
    {"text": ".", "dep": "punct", "pos": "PUNCT", "head": "is"},
}
```

-----

### Extract part of speech tags from the text

```python
print(enalsis.get_POS_tag(text_para))
```

Output - The output format is a list of dictionaries, where each dictionary contains information about a token, including the word (`word`) and its part of speech (`pos`).

```python
[
    {"word": "India", "pos": "PROPN"},
    {"word": "is", "pos": "AUX"},
    {"word": "a", "pos": "DET"},
    {"word": "vast", "pos": "ADJ"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "diverse", "pos": "ADJ"},
    {"word": "country", "pos": "NOUN"},
    {"word": "located", "pos": "VERB"},
    {"word": "in", "pos": "ADP"},
    {"word": "South", "pos": "PROPN"},
    {"word": "Asia", "pos": "PROPN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "known", "pos": "VERB"},
    {"word": "for", "pos": "ADP"},
    {"word": "its", "pos": "PRON"},
    {"word": "rich", "pos": "ADJ"},
    {"word": "history", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "diverse", "pos": "ADJ"},
    {"word": "cultures", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "varied", "pos": "ADJ"},
    {"word": "landscapes", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "With", "pos": "ADP"},
    {"word": "a", "pos": "DET"},
    {"word": "population", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "over", "pos": "ADP"},
    {"word": "$", "pos": "SYM"},
    {"word": "1.3", "pos": "NUM"},
    {"word": "billion", "pos": "NUM"},
    {"word": "people", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "India", "pos": "PROPN"},
    {"word": "is", "pos": "AUX"},
    {"word": "the", "pos": "DET"},
    {"word": "second", "pos": "ADV"},
    {"word": "-", "pos": "PUNCT"},
    {"word": "most", "pos": "ADV"},
    {"word": "populous", "pos": "ADJ"},
    {"word": "country", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "world", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "The", "pos": "DET"},
    {"word": "country", "pos": "NOUN"},
    {"word": "is", "pos": "AUX"},
    {"word": "characterized", "pos": "VERB"},
    {"word": "by", "pos": "ADP"},
    {"word": "a", "pos": "DET"},
    {"word": "harmonious", "pos": "ADJ"},
    {"word": "blend", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "tradition", "pos": "NOUN"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "modernity", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "where", "pos": "SCONJ"},
    {"word": "ancient", "pos": "ADJ"},
    {"word": "customs", "pos": "NOUN"},
    {"word": "coexist", "pos": "VERB"},
    {"word": "with", "pos": "ADP"},
    {"word": "rapidly", "pos": "ADV"},
    {"word": "evolving", "pos": "VERB"},
    {"word": "urban", "pos": "ADJ"},
    {"word": "lifestyles", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "\n\n", "pos": "SPACE"},
    {"word": "Geographically", "pos": "PROPN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "India", "pos": "PROPN"},
    {"word": "boasts", "pos": "VERB"},
    {"word": "a", "pos": "DET"},
    {"word": "wide", "pos": "ADJ"},
    {"word": "range", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "terrains", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "from", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "snow", "pos": "NOUN"},
    {"word": "-", "pos": "PUNCT"},
    {"word": "capped", "pos": "VERB"},
    {"word": "Himalayan", "pos": "ADJ"},
    {"word": "mountains", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "north", "pos": "NOUN"},
    {"word": "to", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "tropical", "pos": "ADJ"},
    {"word": "beaches", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "south", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "The", "pos": "DET"},
    {"word": "country", "pos": "NOUN"},
    {"word": "is", "pos": "AUX"},
    {"word": "home", "pos": "NOUN"},
    {"word": "to", "pos": "ADP"},
    {"word": "a", "pos": "DET"},
    {"word": "myriad", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "ecosystems", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "supporting", "pos": "VERB"},
    {"word": "a", "pos": "DET"},
    {"word": "diverse", "pos": "ADJ"},
    {"word": "array", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "flora", "pos": "NOUN"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "fauna", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "The", "pos": "DET"},
    {"word": "Ganges", "pos": "PROPN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "one", "pos": "NUM"},
    {"word": "of", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "holiest", "pos": "ADJ"},
    {"word": "rivers", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "Hinduism", "pos": "PROPN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "flows", "pos": "VERB"},
    {"word": "through", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "heart", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "country", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "playing", "pos": "VERB"},
    {"word": "a", "pos": "DET"},
    {"word": "vital", "pos": "ADJ"},
    {"word": "role", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "cultural", "pos": "ADJ"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "spiritual", "pos": "ADJ"},
    {"word": "fabric", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "India", "pos": "PROPN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "\n\n", "pos": "SPACE"},
    {"word": "India", "pos": "PROPN"},
    {"word": "'s", "pos": "PART"},
    {"word": "rich", "pos": "ADJ"},
    {"word": "cultural", "pos": "ADJ"},
    {"word": "heritage", "pos": "NOUN"},
    {"word": "is", "pos": "AUX"},
    {"word": "reflected", "pos": "VERB"},
    {"word": "in", "pos": "ADP"},
    {"word": "its", "pos": "PRON"},
    {"word": "numerous", "pos": "ADJ"},
    {"word": "festivals", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "art", "pos": "NOUN"},
    {"word": "forms", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "classical", "pos": "ADJ"},
    {"word": "dance", "pos": "NOUN"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "music", "pos": "NOUN"},
    {"word": "traditions", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "The", "pos": "DET"},
    {"word": "country", "pos": "NOUN"},
    {"word": "has", "pos": "VERB"},
    {"word": "a", "pos": "DET"},
    {"word": "long", "pos": "ADJ"},
    {"word": "history", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "contributions", "pos": "NOUN"},
    {"word": "to", "pos": "ADP"},
    {"word": "science", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "mathematics", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "literature", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "philosophy", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "Ancient", "pos": "ADJ"},
    {"word": "texts", "pos": "NOUN"},
    {"word": "such", "pos": "ADJ"},
    {"word": "as", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "Vedas", "pos": "PROPN"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "Upanishads", "pos": "PROPN"},
    {"word": "have", "pos": "AUX"},
    {"word": "left", "pos": "VERB"},
    {"word": "an", "pos": "DET"},
    {"word": "indelible", "pos": "ADJ"},
    {"word": "mark", "pos": "NOUN"},
    {"word": "on", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "intellectual", "pos": "ADJ"},
    {"word": "landscape", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "world", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "\n\n", "pos": "SPACE"},
    {"word": "The", "pos": "DET"},
    {"word": "Indian", "pos": "ADJ"},
    {"word": "economy", "pos": "NOUN"},
    {"word": "has", "pos": "AUX"},
    {"word": "undergone", "pos": "VERB"},
    {"word": "significant", "pos": "ADJ"},
    {"word": "transformation", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "recent", "pos": "ADJ"},
    {"word": "decades", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "emerging", "pos": "VERB"},
    {"word": "as", "pos": "ADP"},
    {"word": "one", "pos": "NUM"},
    {"word": "of", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "world", "pos": "NOUN"},
    {"word": "'s", "pos": "PART"},
    {"word": "fastest", "pos": "ADV"},
    {"word": "-", "pos": "PUNCT"},
    {"word": "growing", "pos": "VERB"},
    {"word": "major", "pos": "ADJ"},
    {"word": "economies", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "Information", "pos": "NOUN"},
    {"word": "technology", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "software", "pos": "NOUN"},
    {"word": "services", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "a", "pos": "DET"},
    {"word": "burgeoning", "pos": "VERB"},
    {"word": "startup", "pos": "NOUN"},
    {"word": "ecosystem", "pos": "NOUN"},
    {"word": "have", "pos": "AUX"},
    {"word": "contributed", "pos": "VERB"},
    {"word": "to", "pos": "ADP"},
    {"word": "India", "pos": "PROPN"},
    {"word": "'s", "pos": "PART"},
    {"word": "position", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "the", "pos": "DET"},
    {"word": "global", "pos": "ADJ"},
    {"word": "economy", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "Despite", "pos": "SCONJ"},
    {"word": "these", "pos": "DET"},
    {"word": "advancements", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "India", "pos": "PROPN"},
    {"word": "faces", "pos": "VERB"},
    {"word": "challenges", "pos": "NOUN"},
    {"word": "related", "pos": "VERB"},
    {"word": "to", "pos": "ADP"},
    {"word": "poverty", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "healthcare", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "environmental", "pos": "ADJ"},
    {"word": "sustainability", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "prompting", "pos": "VERB"},
    {"word": "ongoing", "pos": "ADJ"},
    {"word": "efforts", "pos": "NOUN"},
    {"word": "for", "pos": "ADP"},
    {"word": "inclusive", "pos": "ADJ"},
    {"word": "development", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "\n\n", "pos": "SPACE"},
    {"word": "India", "pos": "PROPN"},
    {"word": "'s", "pos": "PART"},
    {"word": "political", "pos": "ADJ"},
    {"word": "landscape", "pos": "NOUN"},
    {"word": "is", "pos": "AUX"},
    {"word": "characterized", "pos": "VERB"},
    {"word": "by", "pos": "ADP"},
    {"word": "a", "pos": "DET"},
    {"word": "robust", "pos": "ADJ"},
    {"word": "democratic", "pos": "ADJ"},
    {"word": "system", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "with", "pos": "ADP"},
    {"word": "a", "pos": "DET"},
    {"word": "diverse", "pos": "ADJ"},
    {"word": "array", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "political", "pos": "ADJ"},
    {"word": "parties", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "The", "pos": "DET"},
    {"word": "country", "pos": "NOUN"},
    {"word": "gained", "pos": "VERB"},
    {"word": "independence", "pos": "NOUN"},
    {"word": "from", "pos": "ADP"},
    {"word": "British", "pos": "ADJ"},
    {"word": "rule", "pos": "NOUN"},
    {"word": "in", "pos": "ADP"},
    {"word": "1947", "pos": "NUM"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "led", "pos": "VERB"},
    {"word": "by", "pos": "ADP"},
    {"word": "Mahatma", "pos": "PROPN"},
    {"word": "Gandhi", "pos": "PROPN"},
    {"word": "and", "pos": "CCONJ"},
    {"word": "other", "pos": "ADJ"},
    {"word": "prominent", "pos": "ADJ"},
    {"word": "leaders", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
    {"word": "India", "pos": "PROPN"},
    {"word": "'s", "pos": "PART"},
    {"word": "commitment", "pos": "NOUN"},
    {"word": "to", "pos": "ADP"},
    {"word": "democracy", "pos": "NOUN"},
    {"word": "is", "pos": "AUX"},
    {"word": "evident", "pos": "ADJ"},
    {"word": "in", "pos": "ADP"},
    {"word": "its", "pos": "PRON"},
    {"word": "vibrant", "pos": "ADJ"},
    {"word": "elections", "pos": "NOUN"},
    {"word": ",", "pos": "PUNCT"},
    {"word": "where", "pos": "SCONJ"},
    {"word": "millions", "pos": "NOUN"},
    {"word": "of", "pos": "ADP"},
    {"word": "citizens", "pos": "NOUN"},
    {"word": "participate", "pos": "VERB"},
    {"word": "in", "pos": "ADP"},
    {"word": "shaping", "pos": "VERB"},
    {"word": "the", "pos": "DET"},
    {"word": "nation", "pos": "NOUN"},
    {"word": "'s", "pos": "PART"},
    {"word": "future", "pos": "NOUN"},
    {"word": ".", "pos": "PUNCT"},
]
```

-----

### Extract misspelled words and the corrected text

```python
print(enalsis.spell_check_text(text_para))
```


Output - The output format is a tuple containing a list of strings representing misspelled words in the text and the corrected text.

```python
(
    [
        "landscapes",
        "evolving",
        "lifestyles",
        "boasts",
        "terrains",
        "snow-capped",
        "beaches",
        "myriad",
        "fauna",
        "Ganges",
        "holiest",
        "festivals",
        "Vedas",
        "fastest-growing",
        "burgeoning",
        "startup",
        "advancements",
        "ongoing",
        "vibrant",
    ],
    "India is a vast and diverse country located in South Asia, known for its rich history, diverse cultures, and varied landscape. With a population of over $ 1.3 billion people, India is the second-most populous country in the world. The country is characterized by a harmonious blend of tradition and modernity, where ancient customs coexist with rapidly revolving urban lifestyle.\n\nGeographically, India boats a wide range of terrain, from the snow-tapped Himalayan mountains in the north to the tropical reaches in the south. The country is home to a myriads of ecosystems, supporting a diverse array of flora and found. The Ranges, one of the holies rivers in Hinduism, flows through the heart of the country, playing a vital role in the cultural and spiritual fabric of India.\n\nIndia's rich cultural heritage is reflected in its numerous festival, art forms, and classical dance and music traditions. The country has a long history of contributions to science, mathematics, literature, and philosophy. Ancient texts such as the Heads and Upanishads have left an indelible mark on the intellectual landscape of the world.\n\nThe Indian economy has undergone significant transformation in recent decades, emerging as one of the world's fattest-growing major economies. Information technology, software services, and a burdening started ecosystem have contributed to India's position in the global economy. Despite these advancement, India faces challenges related to poverty, healthcare, and environmental sustainability, prompting going efforts for inclusive development.\n\nIndia's political landscape is characterized by a robust democratic system, with a diverse array of political parties. The country gained independence from British rule in 1947, led by Mahatma Gandhi and other prominent leaders. India's commitment to democracy is evident in its vagrant elections, where millions of citizens participate in shaping the nation's future.",
)
```

-----

### Find misspelled words and its respective corrected words

```python
print(enalsis.find_spell_corrections(text_para))
```

Output - The provided dictionary maps each misspelled words to its corrected form.

```python
{
    "landscapes": "landscape",
    "evolving": "revolving",
    "lifestyles": "lifestyle",
    "boasts": "boats",
    "terrains": "terrain",
    "snow-capped": "snow-tapped",
    "beaches": "reaches",
    "myriad": "myriads",
    "fauna": "found",
    "Ganges": "Ranges",
    "holiest": "holies",
    "festivals": "festival",
    "Vedas": "Heads",
    "fastest-growing": "fattest-growing",
    "burgeoning": "burdening",
    "startup": "started",
    "advancements": "advancement",
    "ongoing": "going",
    "vibrant": "vagrant",
}
```

-----

### Perform the Profanity and Obscene Language Analysis on the text

```python
print(enalsis.profanity_analysis(text_para))
```

Output - The output format is a tuple containing a boolean value indicating whether the text is considered profane (True) or not (False), a numerical score representing the degree of profanity detected in the text and the probability of the text containing offensive language, ranging from 0 to 1.

```python
(False, 0, 0.003242810221774097)
```

-----

### Perform Sentiment Analysis on the text

```python
print(enalsis.sentiment_analysis(text_para))
```

Output - The output is in the format of a dictionary containing sentiment analysis results for a given text. It includes the sentiment label, sentiment polarity, and a list of sentiment-bearing words with their associated scores and frequencies.

```python
{
    "sentiment_label": "Positive",
    "sentiment_polarity": 0.09238505747126437,
    "sentiment_words": [
        {"word": "diverse", "score": 0.09238505747126437, "frequency": 4},
        {"word": "rich", "score": 0.09238505747126437, "frequency": 2},
        {"word": "cultural", "score": 0.09238505747126437, "frequency": 2},
        {"word": "ancient", "score": 0.09238505747126437, "frequency": 1},
        {"word": "political", "score": 0.09238505747126437, "frequency": 2},
    ],
}
```

-----

### Get the Semantic Similarity between the two texts

```python
print(enalsis.semantic_similarity(text_para, text_para))
```

Output - The output is a number representing the Semantic Similarity between the two texts.

```python
0.9999999
```

-----

### Extract the text summary

```python
print(enalsis.text_summarization(text_para, 10))
```

Output - The output is in the format of a paragraph representing the summary of the text provided.

```python
The Ganges, one of the holiest rivers in Hinduism, flows through the heart of the country, playing a vital role in the cultural and spiritual fabric of India. Geographically, India boasts a wide range of terrains, from the snow-capped Himalayan mountains in the north to the tropical beaches in the south. India is a vast and diverse country located in South Asia, known for its rich history, diverse cultures, and varied landscapes. Despite these advancements, India faces challenges related to poverty, healthcare, and environmental sustainability, prompting ongoing efforts for inclusive development. The country has a long history of contributions to science, mathematics, literature, and philosophy. Information technology, software services, and a burgeoning startup ecosystem have contributed to India's position in the global economy. With a population of over $ 1.3 billion people, India is the second-most populous country in the world. India's commitment to democracy is evident in its vibrant elections, where millions of citizens participate in shaping the nation's future. The country is home to a myriad of ecosystems, supporting a diverse array of flora and fauna. India's rich cultural heritage is reflected in its numerous festivals, art forms, and classical dance and music traditions.
```

-----

### Perform Readability Analysis on the text

```python
print(enalsis.calculate_readability_metrics(text_para))
```

Output - The provided data is a dictionary containing various readability scores for a text. These scores include Flesch Reading Ease, Flesch-Kincaid Grade Level, SMOG Index, Coleman-Liau Index, Automated Readability Index, Dale-Chall Readability Score, Difficult Words count, Linsear Write Formula, Gunning Fog Index, Text Standard, Fernandez Huerta Index, Szigriszt Pazos Index, Gutierrez Polini Index, Crawford Index, Gulpease Index, Osman Index and Average Readability.

```python
{
    "Flesch Reading Ease": 36.18,
    "Flesch-Kincaid Grade Level": 12.7,
    "SMOG Index": 14.3,
    "Coleman-Liau Index": 14.61,
    "Automated Readability Index": 14.6,
    "Dale-Chall Readability Score": 11.53,
    "Difficult Words": 105,
    "Linsear Write Formula": 10.666666666666666,
    "Gunning Fog Index": 14.44,
    "Text Standard": "14th and 15th grade",
    "Fernandez Huerta": 80.38,
    "Szigriszt Pazos": 77.75,
    "Gutierrez Polini": 35.08,
    "Crawford": 4.2,
    "Gulpease Index": 48.3,
    "Osman": 36.45,
    "Average Readability": 29.370476190476186,
}
```

-----

### Perform paragraph-wise sentiment analysis on the text

```python
print(enalsis.paragraph_sentiment_analysis(text_para))
```


Output - The output format is in the form of a list containing the sentiments of the paragraphs present in the text.

```python
[0.125, 0.06999999999999999, 0.090625, 0.0875, 0.09895833333333333]
```

-----

### Perform sentence-wise sentiment analysis on the text

```python
print(enalsis.sentence_sentiment_analysis(text_para))
```

Output - The output format is in the form of a list containing the sentiments of the sentences present in the text.

```python
[0.1875, 0.0, 0.0, -0.1, 0.25, 0.06666666666666667, 0.11875, -0.05, 0.09999999999999999, 0.14583333333333334, 0.0, 0.0, 0.0, 0.125, 0.13888888888888887]
```

-----

### Extract words and their word meanings from the text

```python
print(enalsis.extract_word_meanings(text_para))
```

Output - The outuput format is in the form of a dictionary containing a string representing the word and A list of strings representing the meanings or definitions of the word.

```python
{
    {
        "word": "India",
        "meanings": [
            "a republic in the Asian subcontinent in southern Asia; second most populous country in the world; achieved independence from the United Kingdom in 1947"
        ],
    },
    {
        "word": "is",
        "meanings": [
            "have the quality of being; (copula, used with an adjective or a predicate noun)",
            "be identical to; be someone or something",
            "occupy a certain position or area; be somewhere",
            "have an existence, be extant",
            "happen, occur, take place",
            "be identical or equivalent to",
            "form or compose",
            "work in a specific place, with a specific subject, or in a specific function",
            "represent, as of a character on stage",
            "spend or use time",
            "have life, be alive",
            "to remain unmolested, undisturbed, or uninterrupted -- used only in infinitive form",
            "be priced at",
        ],
    },
    {
        "word": "a",
        "meanings": [
            "a metric unit of length equal to one ten billionth of a meter (or 0.0001 micron); used to specify wavelengths of electromagnetic radiation",
            "any of several fat-soluble vitamins essential for normal vision; prevents night blindness or inflammation or dryness of the eyes",
            "one of the four nucleotides used in building DNA; all four nucleotides have a common phosphate group and a sugar (ribose)",
            "(biochemistry) purine base found in DNA and RNA; pairs with thymine in DNA and with uracil in RNA",
            "the basic unit of electric current adopted under the Systeme International d'Unites",
            "the 1st letter of the Roman alphabet",
            "the blood group whose red cells carry the A antigen",
        ],
    },
    {
        "word": "vast",
        "meanings": [
            "unusually great in size or amount or degree or especially extent or scope; ; ; ; ; ; ; ; ; - W.R.Inge"
        ],
    },
    {"word": "and", "meanings": []},
    {
        "word": "diverse",
        "meanings": ["many and different", "distinctly dissimilar or unlike"],
    },
    {
        "word": "country",
        "meanings": [
            "a politically organized body of people under a single government",
            "the territory occupied by a nation",
            "the people who live in a nation or country",
            "an area outside of cities and towns",
            "a particular geographical region of indefinite boundary (usually serving some special purpose or distinguished by its people or culture or geography)",
        ],
    },
    {
        "word": "located",
        "meanings": [
            "discover the location of; determine the place of; find by searching or examining",
            "determine or indicate the place, site, or limits of, as if by an instrument or by a survey",
            "assign a location to",
            "take up residence and become established",
            "situated in a particular spot or position",
        ],
    },
    {
        "word": "in",
        "meanings": [
            "a unit of length equal to one twelfth of a foot",
            "a rare soft silvery metallic element; occurs in small quantities in sphalerite",
            "a state in midwestern United States",
            "holding office",
            "directed or bound inward",
            "currently fashionable",
            "to or toward the inside of",
        ],
    },
    {
        "word": "South",
        "meanings": [
            "the region of the United States lying to the south of the Mason-Dixon line",
            "the southern states that seceded from the United States in 1861",
            "the cardinal compass point that is at 180 degrees",
            "a location in the southern part of a country, region, or city",
            "the direction corresponding to the southward cardinal compass point",
            "situated in or facing or moving toward or coming from the south",
            "in a southern direction",
        ],
    },
    {
        "word": "Asia",
        "meanings": [
            "the largest continent with 60% of the earth's population; it is joined to Europe on the west to form Eurasia; it is the site of some of the world's earliest civilizations",
            "the nations of the Asian continent collectively",
        ],
    },
    {"word": ",", "meanings": []},
    {
        "word": "known",
        "meanings": [
            "be cognizant or aware of a fact or a specific piece of information; possess knowledge or information about",
            "know how to do or perform something",
            "be aware of the truth of something; have a belief or faith in something; regard as true beyond any doubt",
            "be familiar or acquainted with a person or an object",
            "have firsthand knowledge of states, situations, emotions, or sensations",
            "accept (someone) to be what is claimed or accept his power and authority",
            "have fixed in the mind",
            "have sexual intercourse with",
            "know the nature or character of",
            "be able to distinguish, recognize as being different",
            "perceive as familiar",
            "apprehended with certainty",
        ],
    },
    {"word": "for", "meanings": []},
    {
        "word": "its",
        "meanings": [
            "the branch of engineering that deals with the use of computers and telecommunications to retrieve and store and transmit information"
        ],
    },
    {
        "word": "rich",
        "meanings": [
            "people who have possessions and wealth (considered as a group)",
            "possessing material wealth",
            "having an abundant supply of desirable qualities or substances (especially natural resources)",
            "of great worth or quality",
            "marked by great fruitfulness",
            "strong; intense",
            "very productive",
            "high in mineral content; having a high proportion of fuel to air; ,",
            "suggestive of or characterized by great expense",
            "containing plenty of fat, or eggs, or sugar",
            "marked by richness and fullness of flavor",
            "pleasantly full and mellow",
            "affording an abundant supply",
        ],
    },
    {
        "word": "history",
        "meanings": [
            "the aggregate of past events",
            "a record or narrative description of past events",
            "the discipline that records and interprets past events involving human beings",
            "the continuum of events occurring in succession leading from the past to the present and even into the future",
            "all that is remembered of the past as preserved in writing; a body of knowledge",
        ],
    },
    {
        "word": "cultures",
        "meanings": [
            "a particular society at a particular time and place",
            "the tastes in art and manners that are favored by a social group",
            "all the knowledge and values shared by a society",
            "(biology) the growing of microorganisms in a nutrient medium (such as gelatin or agar)",
            "a highly developed state of perfection; having a flawless or impeccable quality; ; ; --Joseph Conrad",
            "the attitudes and behavior that are characteristic of a particular social group or organization",
            "the raising of plants or animals",
            "grow in a special preparation",
        ],
    },
    {
        "word": "varied",
        "meanings": [
            "become different in some particular way, without permanently losing one's or its former characteristics or essence",
            "be at variance with; be out of line with",
            "be subject to change in accordance with a variable",
            "make something more diverse and varied",
            "characterized by variety",
            "widely different",
            "broken away from sameness or identity or duplication",
        ],
    },
    {
        "word": "landscapes",
        "meanings": [
            "an expanse of scenery that can be seen in a single view",
            "painting depicting an expanse of natural scenery",
            "a genre of art dealing with the depiction of natural scenery",
            "an extensive mental viewpoint",
            "embellish with plants",
            "do landscape gardening",
        ],
    },
    {"word": ".", "meanings": []},
    {"word": "With", "meanings": []},
    {
        "word": "population",
        "meanings": [
            "the people who inhabit a territory or state",
            "a group of organisms of the same species inhabiting a given area",
            "(statistics) the entire aggregation of items from which samples can be drawn",
            "the number of inhabitants (either the total number or the number of a particular race or class) in a given place (country or city etc.)",
            "the act of populating (causing to live in a place)",
        ],
    },
    {"word": "of", "meanings": []},
    {
        "word": "over",
        "meanings": [
            "(cricket) the division of play during which six balls are bowled at the batsman by one player from the other team from the same end of the pitch",
            "having come or been brought to a conclusion",
            "at or to a point across intervening space etc.",
            "throughout an area",
            "throughout a period of time",
            "beyond the top or upper surface or edge; forward from an upright position",
            "over the entire area",
        ],
    },
    {"word": "$", "meanings": []},
    {"word": "1.3", "meanings": []},
    {
        "word": "billion",
        "meanings": [
            "the number that is represented as a one followed by 12 zeros; in the United Kingdom the usage followed in the United States is frequently seen",
            "a very large indefinite number (usually hyperbole)",
            "the number that is represented as a one followed by 9 zeros",
            "denoting a quantity consisting of one thousand million items or units in the United States",
            "denoting a quantity consisting of one million million items or units in Great Britain",
        ],
    },
    {
        "word": "people",
        "meanings": [
            "(plural) any group of human beings (men or women or children) collectively",
            "the body of citizens of a state or country",
            "members of a family line",
            "the common people generally",
            "fill with people",
            "furnish with people",
        ],
    },
    {"word": "the", "meanings": []},
    {"word": "second-most", "meanings": []},
    {"word": "populous", "meanings": ["densely populated"]},
    {
        "word": "world",
        "meanings": [
            "everything that exists anywhere",
            "people in general; especially a distinctive group of people with some shared interest",
            "all of your experiences that determine how things appear to you",
            "the 3rd planet from the sun; the planet we live on",
            "people in general considered as a whole",
            "a part of the earth that can be considered separately",
            "the concerns of this life as distinguished from heaven and the afterlife",
            "all of the living human inhabitants of the earth",
            "involving the entire earth; not limited or provincial in scope",
        ],
    },
    {"word": "The", "meanings": []},
    {
        "word": "characterized",
        "meanings": [
            "describe or portray the character or the qualities or peculiarities of",
            "be characteristic of",
        ],
    },
    {
        "word": "by",
        "meanings": [
            "so as to pass a given point",
            "in reserve; not for immediate use",
        ],
    },
    {
        "word": "harmonious",
        "meanings": [
            "musically pleasing",
            "exhibiting equivalence or correspondence among constituents of an entity or between different entities",
            "suitable and fitting",
            "existing together in harmony",
        ],
    },
    {
        "word": "blend",
        "meanings": [
            "an occurrence of thorough mixing",
            "a new word formed by joining two others and combining their meanings",
            "the act of blending components together thoroughly",
            "combine into one",
            "blend or harmonize",
            "mix together different elements",
        ],
    },
    {
        "word": "tradition",
        "meanings": [
            "an inherited pattern of thought or action",
            "a specific practice of long standing",
        ],
    },
    {
        "word": "modernity",
        "meanings": ["the quality of being current or of the present"],
    },
    {"word": "where", "meanings": []},
    {
        "word": "ancient",
        "meanings": [
            "a very old person",
            "a person who lived in ancient times",
            "belonging to times long past especially of the historical period before the fall of the Western Roman Empire",
            "very old",
        ],
    },
    {
        "word": "customs",
        "meanings": [
            "money collected under a tariff",
            "accepted or habitual practice",
            "a specific practice of long standing",
            "money collected under a tariff",
            "habitual patronage",
        ],
    },
    {
        "word": "coexist",
        "meanings": ["coexist peacefully, as of nations", "exist together"],
    },
    {"word": "with", "meanings": []},
    {"word": "rapidly", "meanings": ["with rapid movements"]},
    {
        "word": "evolving",
        "meanings": [
            "work out",
            "undergo development or evolution",
            "gain through experience",
        ],
    },
    {
        "word": "urban",
        "meanings": [
            "relating to or concerned with a city or densely populated area",
            "located in or characteristic of a city or city life",
        ],
    },
    {
        "word": "lifestyles",
        "meanings": [
            "a manner of living that reflects the person's values and attitudes"
        ],
    },
    {"word": "Geographically", "meanings": ["with respect to geography"]},
    {
        "word": "boasts",
        "meanings": [
            "speaking of yourself in superlatives",
            "show off",
            "wear or display in an ostentatious or proud manner",
        ],
    },
    {
        "word": "wide",
        "meanings": [
            "having great (or a certain) extent from one side to the other",
            "broad in scope or content; ; ; ; ; - T.G.Winner",
            "(used of eyes) fully open or extended",
            "very large in expanse or scope",
            "great in degree",
            "having ample fabric",
            "not on target",
            "with or by a broad space",
            "to the fullest extent possible",
            "far from the intended target",
            "to or over a great extent or range; far",
        ],
    },
    {
        "word": "range",
        "meanings": [
            "an area in which something acts or operates or has power or control:",
            "the limits within which something can be effective",
            "a large tract of grassy open land on which livestock can graze",
            "a series of hills or mountains",
            "a place for shooting (firing or driving) projectiles of various kinds",
            "a variety of different things or activities",
            "(mathematics) the set of values of the dependent variable for which a function is defined",
            "the limit of capability",
            "a kitchen appliance used for cooking food",
            "change or be different within limits",
            "move about aimlessly or without any destination, often in search of food or employment",
            "have a range; be capable of projecting over a certain distance, as of a gun",
            "range or extend over; occupy a certain area",
            "lay out orderly or logically in a line or as if in a line",
            "feed as in a meadow or pasture",
            "let eat",
            "assign a rank or rating to",
        ],
    },
    {
        "word": "terrains",
        "meanings": [
            "a piece of ground having specific characteristics or military potential"
        ],
    },
    {"word": "from", "meanings": []},
    {
        "word": "snow-capped",
        "meanings": ["(of mountains) capped with a covering of snow"],
    },
    {"word": "Himalayan", "meanings": ["of or relating to the Himalayas"]},
    {
        "word": "mountains",
        "meanings": [
            "a land mass that projects well above its surroundings; higher than a hill",
            "(often followed by `of') a large number or amount or extent",
        ],
    },
    {
        "word": "north",
        "meanings": [
            "the region of the United States lying to the north of the Mason-Dixon line",
            "the United States (especially the northern states during the American Civil War)",
            "the cardinal compass point that is at 0 or 360 degrees",
            "a location in the northern part of a country, region, or city",
            "the direction corresponding to the northward cardinal compass point",
            "the direction in which a compass needle points",
            "British statesman under George III whose policies led to rebellion in the American colonies (1732-1792)",
            "situated in or facing or moving toward or coming from the north",
            "in a northern direction",
        ],
    },
    {"word": "to", "meanings": []},
    {
        "word": "tropical",
        "meanings": [
            "relating to or situated in or characteristic of the tropics (the region on either side of the equator)",
            "of or relating to the tropics, or either tropic",
            "characterized by or of the nature of a trope or tropes; changed from its literal sense",
            "of weather or climate; hot and humid as in the tropics",
        ],
    },
    {
        "word": "beaches",
        "meanings": [
            "an area of sand sloping down to the water of a sea or lake",
            "land on a beach",
        ],
    },
    {
        "word": "south",
        "meanings": [
            "the region of the United States lying to the south of the Mason-Dixon line",
            "the southern states that seceded from the United States in 1861",
            "the cardinal compass point that is at 180 degrees",
            "a location in the southern part of a country, region, or city",
            "the direction corresponding to the southward cardinal compass point",
            "situated in or facing or moving toward or coming from the south",
            "in a southern direction",
        ],
    },
    {
        "word": "home",
        "meanings": [
            "where you live at a particular time",
            "housing that someone is living in",
            "the country or state or city where you live",
            "(baseball) base consisting of a rubber slab where the batter stands; it must be touched by a base runner in order to score",
            "the place where you are stationed and from which missions start and end",
            "place where something began and flourished",
            "an environment offering affection and security",
            "a social unit living together",
            "an institution where people are cared for",
            "provide with, or send to, a home",
            "return home accurately from a long distance",
            "used of your own ground",
            "relating to or being where one lives or where one's roots are",
            "inside the country",
            "at or to or in the direction of one's home or family",
            "on or to the point aimed at",
            "to the fullest extent; to the heart",
        ],
    },
    {
        "word": "myriad",
        "meanings": [
            "a large indefinite number",
            "the cardinal number that is the product of ten and one thousand",
            "too numerous to be counted",
        ],
    },
    {
        "word": "ecosystems",
        "meanings": [
            "a system formed by the interaction of a community of organisms with their physical environment"
        ],
    },
    {
        "word": "supporting",
        "meanings": [
            "the act of bearing the weight of or strengthening",
            "give moral or psychological support, aid, or courage to",
            "support materially or financially",
            "be behind; approve of",
            "be the physical support of; carry the weight of",
            "establish or strengthen as with new evidence or facts",
            "adopt as a belief",
            "support with evidence or authority or make more certain or confirm",
            "argue or speak in defense of",
            "play a subordinate role to (another performer)",
            "be a regular customer or client of",
            "put up with something or somebody unpleasant",
            "furnishing support and encouragement",
            "capable of bearing a structural load",
        ],
    },
    {
        "word": "array",
        "meanings": [
            "an orderly arrangement",
            "an impressive display",
            "especially fine or decorative clothing",
            "an arrangement of aerials spaced to give desired directional characteristics",
            "lay out orderly or logically in a line or as if in a line",
            "align oneself with a group or a way of thinking",
        ],
    },
    {
        "word": "flora",
        "meanings": [
            "all the plant life in a particular region or period",
            "(botany) a living organism lacking the power of locomotion",
        ],
    },
    {
        "word": "fauna",
        "meanings": [
            "all the animal life in a particular region or period",
            "a living organism characterized by voluntary movement",
        ],
    },
    {
        "word": "Ganges",
        "meanings": [
            "an Asian river; rises in the Himalayas and flows east into the Bay of Bengal; a sacred river of the Hindus",
            "act as an organized group",
        ],
    },
    {
        "word": "one",
        "meanings": [
            "the smallest whole number or a numeral representing this number",
            "a single person or thing",
            "used of a single unit or thing; not two or more",
            "having the indivisible character of a unit",
            "of the same kind or quality",
            "used informally as an intensifier",
            "indefinite in time or position",
            "being a single entity made by combining separate components",
            "eminent beyond or above comparison",
        ],
    },
    {
        "word": "holiest",
        "meanings": ["belonging to or derived from or associated with a divine power"],
    },
    {
        "word": "rivers",
        "meanings": ["a large natural stream of water (larger than a creek)"],
    },
    {
        "word": "Hinduism",
        "meanings": [
            "the religion of most people in India, Bangladesh, Sri Lanka, and Nepal",
            "a body of religious and philosophical beliefs and cultural practices native to India and based on a caste system; it is characterized by a belief in reincarnation, by a belief in a supreme being of many forms and natures, by the view that opposing theories are aspects of one eternal truth, and by a desire for liberation from earthly evils",
        ],
    },
    {
        "word": "flows",
        "meanings": [
            "the motion characteristic of fluids (liquids or gases)",
            "the amount of fluid that flows in a given time",
            "the act of flowing or streaming; continuous progression",
            "any uninterrupted stream or discharge",
            "something that resembles a flowing stream in moving continuously",
            "dominant course (suggestive of running water) of successive events or ideas",
            "the monthly discharge of blood from the uterus of nonpregnant women from puberty to menopause; ; --Hippocrates; --Aristotle",
            "move or progress freely as if in a stream",
            "move along, of liquids",
            "cause to flow",
            "be abundantly present",
            "fall or flow in a certain way",
            "cover or swamp with water",
            "undergo menstruation",
        ],
    },
    {
        "word": "through",
        "meanings": [
            "having finished or arrived at completion",
            "(of a route or journey etc.) continuing without requiring stops or changes",
            "from beginning to end",
            "over the whole distance",
            "to completion",
            "in diameter",
            "throughout the entire extent",
        ],
    },
    {
        "word": "heart",
        "meanings": [
            "the locus of feelings and intuitions",
            "the hollow muscular organ located behind the sternum and between the lungs; its rhythmic contractions move the blood through the body",
            "the courage to carry on",
            "an area that is approximately central within some larger region",
            "the choicest or most essential or most vital part of some idea or experience",
            "an inclination or tendency of a certain kind",
            "a plane figure with rounded sides curving inward at the top and intersecting at the bottom; conventionally used on playing cards and valentines",
            "a firm rather dry variety meat (usually beef or veal)",
            "a positive feeling of liking",
            "a playing card in the major suit that has one or more red hearts on it",
        ],
    },
    {
        "word": "playing",
        "meanings": [
            "the act of playing a musical instrument",
            "the action of taking part in a game or sport or other recreation",
            "the performance of a part or role in a drama",
            "participate in games or sport",
            "act or have an effect in a specified way or with a specific effect or outcome",
            "play on an instrument",
            "play a role or part",
            "be at play; be engaged in playful activity; amuse oneself in a way characteristic of children",
            "replay (as a melody)",
            "perform music on (a musical instrument)",
            "pretend to have certain qualities or state of mind",
            "move or seem to move quickly, lightly, or irregularly",
            "bet or wager (money)",
            "engage in recreational activities rather than work; occupy oneself in a diversion",
            "pretend to be somebody in the framework of a game or playful activity",
            "emit recorded sound",
            "perform on a certain location",
            "put (a card or piece) into play during a game, or act strategically as if in a card game",
            "engage in an activity as if it were a game rather than take it seriously",
            "behave in a certain way",
            "cause to emit recorded audio or video",
            "manipulate manually or in one's mind or imagination",
            "use to one's advantage",
            "consider not very seriously",
            "be received or accepted or interpreted in a specific way",
            "behave carelessly or indifferently",
            "cause to move or operate freely within a bounded space",
            "perform on a stage or theater",
            "be performed or presented for public viewing",
            "cause to happen or to occur as a consequence",
            "discharge or direct or be discharged or directed as if in a continuous stream",
            "make bets",
            "stake on the outcome of an issue",
            "shoot or hit in a particular manner",
            "use or move",
            "employ in a game or in a specific position",
            "contend against an opponent in a sport, game, or battle",
            "exhaust by allowing to pull on the line",
        ],
    },
    {
        "word": "vital",
        "meanings": [
            "urgently needed; absolutely necessary",
            "performing an essential function in the living body",
            "full of spirit",
            "manifesting or characteristic of life",
        ],
    },
    {
        "word": "role",
        "meanings": [
            "the actions and activities assigned to or required or expected of a person or group",
            "an actor's portrayal of someone in a play",
            "what something is used for",
            "normal or customary activity of a person in a particular social setting",
        ],
    },
    {
        "word": "cultural",
        "meanings": [
            "of or relating to the arts and manners that a group favors",
            "denoting or deriving from or distinctive of the ways of living built up by a group of people; - J.F.Kennedy",
            "of or relating to the shared knowledge and values of a society",
            "relating to the raising of plants or animals",
        ],
    },
    {
        "word": "spiritual",
        "meanings": [
            "a kind of religious song originated by Blacks in the southern United States",
            "concerned with sacred matters or religion or the church",
            "concerned with or affecting the spirit or soul",
            "lacking material body or form or substance; ; -Lewis Mumford",
            "resembling or characteristic of a phantom",
        ],
    },
    {
        "word": "fabric",
        "meanings": [
            "artifact made by weaving or felting or knitting or crocheting natural or synthetic fibers",
            "the underlying structure",
        ],
    },
    {"word": "'s", "meanings": []},
    {
        "word": "heritage",
        "meanings": [
            "practices that are handed down from the past by tradition",
            "any attribute or immaterial possession that is inherited from ancestors",
            "that which is inherited; a title or property or estate that passes by law to the heir on the death of the owner",
            "hereditary succession to a title or an office or property",
        ],
    },
    {
        "word": "reflected",
        "meanings": [
            "manifest or bring back",
            "reflect deeply on a subject",
            "to throw or bend back (from a surface)",
            "be bright by reflecting or casting light",
            "show an image of",
            "give evidence of a certain behavior",
            "give evidence of the quality of",
            "(especially of incident sound or light) bent or sent back",
        ],
    },
    {"word": "numerous", "meanings": ["amounting to a large indefinite number"]},
    {
        "word": "festivals",
        "meanings": [
            "a day or period of time set aside for feasting and celebration",
            "an organized series of acts and performances (usually in one place)",
        ],
    },
    {
        "word": "art",
        "meanings": [
            "the products of human creativity; works of art collectively",
            "the creation of beautiful or significant things",
            "a superior skill that you can learn by study and practice and observation",
            "photographs or other visual representations in a printed publication",
        ],
    },
    {
        "word": "forms",
        "meanings": [
            "the phonological or orthographic sound or appearance of a word that can be used to describe or identify something",
            "a category of things distinguished by some common characteristic or quality",
            "a perceptual structure",
            "any spatial attributes (especially as defined by outline)",
            "alternative names for the body of a human being",
            "the spatial arrangement of something as distinct from its substance",
            "the visual appearance of something or someone",
            "a printed document with spaces in which to write",
            "(biology) a group of organisms within a species that differ in trivial ways from similar groups",
            "an arrangement of the elements in a composition or discourse",
            "a particular mode in which something is manifested",
            "(physical chemistry) a distinct state of matter in a system; matter that is identical in chemical composition and physical state and separated from other material by the phase boundary",
            "a body of students who are taught together",
            "an ability to perform well",
            "a life-size dummy used to display clothes",
            "a mold for setting concrete",
            "create (as an entity)",
            "to compose or represent:",
            "develop into a distinctive entity",
            "give shape or form to",
            "make something, usually for a specific function",
            "establish or impress firmly in the mind",
            "assume a form or shape",
        ],
    },
    {
        "word": "classical",
        "meanings": [
            "traditional genre of music conforming to an established form and appealing to critical interest and developed musical taste",
            "of or relating to the most highly developed stage of an earlier civilisation and its culture",
            "of recognized authority or excellence",
            "of or relating to the study of the literary works of ancient Greece and Rome",
            '(language) having the form used by ancient standard authors; "classical Greek',
            'of or pertaining to or characteristic of the ancient Greek and Roman cultures; ; "classical',
        ],
    },
    {
        "word": "dance",
        "meanings": [
            "an artistic form of nonverbal communication",
            "a party of people assembled for dancing",
            "taking a series of rhythmical steps (and movements) in time to music",
            "a party for social dancing",
            "move in a graceful and rhythmical way",
            "move in a pattern; usually to musical accompaniment; do or perform a dance",
            "skip, leap, or move up and down or sideways",
        ],
    },
    {
        "word": "music",
        "meanings": [
            "an artistic form of auditory communication incorporating instrumental or vocal tones in a structured and continuous manner",
            "any agreeable (pleasing and harmonious) sounds",
            "musical activity (singing or whistling etc.)",
            "(music) the sounds produced by singers or musical instruments (or reproductions of such sounds)",
            "punishment for one's actions",
        ],
    },
    {
        "word": "traditions",
        "meanings": [
            "an inherited pattern of thought or action",
            "a specific practice of long standing",
        ],
    },
    {
        "word": "has",
        "meanings": [
            "(astronomy) the angular distance of a celestial point measured westward along the celestial equator from the zenith crossing; the right ascension for an observer at a particular location and time of day",
            "have or possess, either in a concrete or an abstract sense",
            "have as a feature",
            "go through (mental or physical states or experiences)",
            "have ownership or possession of",
            "cause to move; cause to be in a certain position or condition",
            "serve oneself to, or consume regularly",
            "have a personal or business relationship with someone",
            "organize or be responsible for",
            "have left",
            "be confronted with",
            "undergo",
            "suffer from; be ill with",
            "cause to do; cause to act in a specified manner",
            "receive willingly something given or offered",
            "get something; come into possession of",
            "undergo (as of injuries and illnesses)",
            "achieve a point or goal",
            "cause to be born",
            "have sex with; archaic use",
        ],
    },
    {
        "word": "long",
        "meanings": [
            "desire strongly or persistently",
            "primarily temporal sense; being or indicating a relatively great or greater than average duration or passage of time or a duration as specified",
            "primarily spatial sense; of relatively great or greater than average spatial extension or extension as specified",
            "of relatively great height; - Sherwood Anderson",
            "good at remembering",
            "holding securities or commodities in expectation of a rise in prices",
            "(of speech sounds or syllables) of relatively long duration",
            "involving substantial risk",
            "planning prudently for the future",
            "having or being more than normal or necessary:",
            "for an extended time or at a distant time",
            "for an extended distance",
        ],
    },
    {
        "word": "contributions",
        "meanings": [
            "the part played by a person in bringing about a result",
            "a voluntary gift (as of money or service or ideas) made to some worthwhile cause",
            "act of giving in common with others for a common purpose especially to a charity",
            "an amount of money contributed",
            "a writing for publication especially one of a collection of writings as an article or story",
        ],
    },
    {
        "word": "science",
        "meanings": [
            "a particular branch of scientific knowledge",
            "ability to produce solutions in some problem domain",
        ],
    },
    {
        "word": "mathematics",
        "meanings": [
            "a science (or group of related sciences) dealing with the logic of quantity and shape and arrangement"
        ],
    },
    {
        "word": "literature",
        "meanings": [
            "creative writing of recognized artistic value",
            "the humanistic study of a body of literature",
            "published writings in a particular style on a particular subject",
            "the profession or art of a writer",
        ],
    },
    {
        "word": "philosophy",
        "meanings": [
            "a belief (or system of beliefs) accepted as authoritative by some group or school",
            "the rational investigation of questions about existence and knowledge and ethics",
            "any personal belief about how to live or how to deal with a situation",
        ],
    },
    {
        "word": "Ancient",
        "meanings": [
            "a very old person",
            "a person who lived in ancient times",
            "belonging to times long past especially of the historical period before the fall of the Western Roman Empire",
            "very old",
        ],
    },
    {
        "word": "texts",
        "meanings": [
            "the words of something written",
            "a passage from the Bible that is used as the subject of a sermon",
            "a book prepared for use in schools or colleges",
            "the main body of a written work (as distinct from illustrations or footnotes etc.)",
        ],
    },
    {
        "word": "such",
        "meanings": ["of so extreme a degree or extent", "to so extreme a degree"],
    },
    {
        "word": "as",
        "meanings": [
            "a very poisonous metallic element that has three allotropic forms; arsenic and arsenic compounds are used as herbicides and insecticides and various alloys; found in arsenopyrite and orpiment and realgar",
            "a United States territory on the eastern part of the island of Samoa",
            "a metric unit of length equal to one ten billionth of a meter (or 0.0001 micron); used to specify wavelengths of electromagnetic radiation",
            "any of several fat-soluble vitamins essential for normal vision; prevents night blindness or inflammation or dryness of the eyes",
            "one of the four nucleotides used in building DNA; all four nucleotides have a common phosphate group and a sugar (ribose)",
            "(biochemistry) purine base found in DNA and RNA; pairs with thymine in DNA and with uracil in RNA",
            "the basic unit of electric current adopted under the Systeme International d'Unites",
            "the 1st letter of the Roman alphabet",
            "the blood group whose red cells carry the A antigen",
            "to the same degree (often followed by `as')",
        ],
    },
    {
        "word": "Vedas",
        "meanings": [
            "(from the Sanskrit word for `knowledge') any of the most ancient sacred writings of Hinduism written in early Sanskrit; traditionally believed to comprise the Samhitas, the Brahmanas, the Aranyakas, and the Upanishads"
        ],
    },
    {
        "word": "Upanishads",
        "meanings": [
            "a later sacred text of Hinduism of a mystical nature dealing with metaphysical questions"
        ],
    },
    {
        "word": "have",
        "meanings": [
            "a person who possesses great material wealth",
            "have or possess, either in a concrete or an abstract sense",
            "have as a feature",
            "go through (mental or physical states or experiences)",
            "have ownership or possession of",
            "cause to move; cause to be in a certain position or condition",
            "serve oneself to, or consume regularly",
            "have a personal or business relationship with someone",
            "organize or be responsible for",
            "have left",
            "be confronted with",
            "undergo",
            "suffer from; be ill with",
            "cause to do; cause to act in a specified manner",
            "receive willingly something given or offered",
            "get something; come into possession of",
            "undergo (as of injuries and illnesses)",
            "achieve a point or goal",
            "cause to be born",
            "have sex with; archaic use",
        ],
    },
    {
        "word": "left",
        "meanings": [
            "location near or direction toward the left side; i.e. the side to the north when a person or object faces east",
            "those who support varying degrees of social or political or economic change designed to promote the public welfare",
            "the hand that is on the left side of the body",
            "the piece of ground in the outfield on the catcher's left",
            "a turn toward the side of the body that is on the north when the person is facing east",
            "go away from a place",
            "go and leave behind, either intentionally or by neglect or forgetfulness",
            "act or be so as to become in a specified state",
            "leave unchanged or undisturbed or refrain from taking",
            "move out of or depart from",
            "make a possibility or provide opportunity for; permit to be attainable or cause to remain",
            "have as a result or residue",
            "remove oneself from an association with or participation in",
            "put into the care or protection of someone",
            "leave or give by will after one's death",
            "have left or have as a remainder",
            "be survived by after one's death",
            "transmit (knowledge or skills)",
            "leave behind unintentionally",
            "being or located on or directed toward the side of the body to the west when facing north",
            "not used up",
            "intended for the left hand",
            "of or belonging to the political or intellectual left",
            "toward or on the left; also used figuratively",
        ],
    },
    {"word": "an", "meanings": ["an associate degree in nursing"]},
    {"word": "indelible", "meanings": ["cannot be removed or erased"]},
    {
        "word": "mark",
        "meanings": [
            "a number or letter indicating quality (especially of a student's performance)",
            "a distinguishing symbol",
            "a reference point to shoot at",
            "a visible indication made on a surface",
            "the impression created by doing something unusual or extraordinary that people notice and remember",
            "a symbol of disgrace or infamy; --Genesis",
            "formerly the basic unit of money in Germany",
            "Apostle and companion of Saint Peter; assumed to be the author of the second Gospel",
            "a person who is gullible and easy to take advantage of",
            "a written or printed symbol (as for punctuation)",
            "a perceptible indication of something not immediately apparent (as a visible clue that something has happened)",
            "the shortest of the four Gospels in the New Testament",
            "an indication of damage",
            "a marking that consists of lines that cross each other",
            "something that exactly succeeds in achieving its goal",
            "attach a tag or label to",
            "designate as if by a mark",
            "be a distinctive feature, attribute, or trait; sometimes in a very positive sense",
            "mark by some ceremony or observation",
            "make or leave a mark on",
            "to accuse or condemn or openly or formally or brand as disgraceful",
            "notice or perceive",
            "mark with a scar",
            "make small marks into the surface of",
            "establish as the highest level or best performance",
            "make underscoring marks",
            "remove from a list",
            "put a check mark on or near or next to",
            "assign a grade or rank to, according to one's evaluation",
            "insert punctuation marks into",
        ],
    },
    {
        "word": "on",
        "meanings": [
            "in operation or operational",
            "(of events) planned or scheduled",
            "with a forward motion",
            "indicates continuity or persistence or concentration",
            "in a state required for something to function or be effective",
        ],
    },
    {
        "word": "intellectual",
        "meanings": [
            "a person who uses the mind creatively",
            "of or associated with or requiring the use of the mind",
            "appealing to or using the intellect",
            "involving intelligence rather than emotions or instinct",
        ],
    },
    {
        "word": "landscape",
        "meanings": [
            "an expanse of scenery that can be seen in a single view",
            "painting depicting an expanse of natural scenery",
            "a genre of art dealing with the depiction of natural scenery",
            "an extensive mental viewpoint",
            "embellish with plants",
            "do landscape gardening",
        ],
    },
    {
        "word": "Indian",
        "meanings": [
            "a member of the race of people living in America when Europeans arrived",
            "a native or inhabitant of India",
            "any of the languages spoken by Amerindians",
            "of or relating to or characteristic of India or the East Indies or their peoples or languages or cultures",
            "of or pertaining to American Indians or their culture or languages",
        ],
    },
    {
        "word": "economy",
        "meanings": [
            "the system of production and distribution and consumption",
            "the efficient use of resources",
            "frugality in the expenditure of money or resources",
            "an act of economizing; reduction in cost",
        ],
    },
    {"word": "undergone", "meanings": ["pass through"]},
    {
        "word": "significant",
        "meanings": [
            "important in effect or meaning",
            "fairly large",
            "too closely correlated to be attributed to chance and therefore indicating a systematic relation",
            "rich in significance or implication",
        ],
    },
    {
        "word": "transformation",
        "meanings": [
            "a qualitative change",
            "(mathematics) a function that changes the position or direction of the axes of a coordinate system",
            "a rule describing the conversion of one syntactic structure into another related syntactic structure",
            "(genetics) modification of a cell or bacterium by the uptake and incorporation of exogenous DNA",
            "the act of changing in form or shape or appearance",
        ],
    },
    {
        "word": "recent",
        "meanings": [
            "approximately the last 10,000 years",
            "new",
            "of the immediate past or just previous to the present time",
        ],
    },
    {
        "word": "decades",
        "meanings": [
            "a period of 10 years",
            "the cardinal number that is the sum of nine and one; the base of the decimal system",
        ],
    },
    {
        "word": "emerging",
        "meanings": [
            "come out into view, as from concealment",
            "come out of",
            "become known or apparent",
            "come up to the surface of or rise",
            "happen or occur as a result of something",
            "coming to maturity",
            "coming into existence",
        ],
    },
    {"word": "fastest-growing", "meanings": []},
    {
        "word": "major",
        "meanings": [
            "a commissioned military officer in the United States Army or Air Force or Marines; below lieutenant colonel and above captain",
            "British statesman who was prime minister from 1990 until 1997 (born in 1943)",
            "a university student who is studying a particular field as the principal subject",
            "the principal field of study of a student at a university",
            "have as one's principal field of study",
            "of greater importance or stature or rank",
            "greater in scope or effect",
            "greater in number or size or amount",
            "of the field of academic study in which one concentrates or specializes",
            "of a scale or mode",
            "of greater seriousness or danger",
            "of full legal age",
            "of the elder of two boys with the same family name",
        ],
    },
    {
        "word": "economies",
        "meanings": [
            "the system of production and distribution and consumption",
            "the efficient use of resources",
            "frugality in the expenditure of money or resources",
            "an act of economizing; reduction in cost",
        ],
    },
    {
        "word": "Information",
        "meanings": [
            "a message received and understood",
            "knowledge acquired through study or experience or instruction",
            "formal accusation of a crime",
            "a collection of facts from which conclusions may be drawn",
            "(communication theory) a numerical measure of the uncertainty of an outcome",
        ],
    },
    {
        "word": "technology",
        "meanings": [
            "the practical application of science to commerce or industry",
            "the discipline dealing with the art or science of applying scientific knowledge to practical problems",
        ],
    },
    {
        "word": "software",
        "meanings": [
            "(computer science) written programs or procedures or rules and associated documentation pertaining to the operation of a computer system and that are stored in read/write memory"
        ],
    },
    {
        "word": "services",
        "meanings": [
            "performance of duties or provision of space and equipment helpful to others",
            "work done by one person or group that benefits another",
            "an act of help or assistance",
            "the act of public worship following prescribed rules",
            "a company or agency that performs a public service; subject to government regulation",
            "employment in or work for another",
            "a force that is a branch of the armed forces",
            "Canadian writer (born in England) who wrote about life in the Yukon Territory (1874-1958)",
            "a means of serving",
            "tableware consisting of a complete set of articles (silver or dishware) for use at table",
            "the act of mating by male animals",
            "(law) the acts performed by an English feudal tenant for the benefit of his lord which formed the consideration for the property granted to him",
            "(sports) a stroke that puts the ball in play",
            "the act of delivering a writ or summons upon someone",
            "periodic maintenance on a car or machine",
            "the performance of duties by a waiter or servant",
            "be used by; as of a utility",
            "make fit for use",
            "mate with",
        ],
    },
    {"word": "burgeoning", "meanings": ["grow and flourish"]},
    {
        "word": "startup",
        "meanings": [
            "the act of setting in operation",
            "the act of starting a new operation or practice",
        ],
    },
    {
        "word": "ecosystem",
        "meanings": [
            "a system formed by the interaction of a community of organisms with their physical environment"
        ],
    },
    {
        "word": "contributed",
        "meanings": [
            "bestow a quality on",
            "contribute to some cause",
            "be conducive to",
            "provide",
        ],
    },
    {
        "word": "position",
        "meanings": [
            "the particular portion of space occupied by something",
            "a point occupied by troops for tactical reasons",
            "a way of regarding situations or topics etc.",
            "the arrangement of the body and its limbs",
            "the relative position or standing of things or especially persons in a society",
            "a job in an organization",
            "the spatial property of a place where or way in which something is situated",
            "the appropriate or customary location",
            "(in team sports) the role assigned to an individual player",
            "the act of putting something in a certain place",
            "a condition or position in which you find yourself",
            "a rationalized mental attitude",
            "an opinion that is held in opposition to another in an argument or dispute",
            "an item on a list or in a sequence",
            "the post or function properly or customarily occupied or served by another",
            "the act of positing; an assumption taken as a postulate or axiom",
            "cause to be in an appropriate place, state, or relation",
            "put into a certain place or abstract location",
        ],
    },
    {
        "word": "global",
        "meanings": [
            "involving the entire earth; not limited or provincial in scope",
            "having the shape of a sphere or ball; ; ; - Zane Grey",
        ],
    },
    {
        "word": "Despite",
        "meanings": [
            "lack of respect accompanied by a feeling of intense dislike",
            "contemptuous disregard",
        ],
    },
    {"word": "these", "meanings": []},
    {
        "word": "advancements",
        "meanings": [
            "encouragement of the progress or growth or acceptance of something",
            "the act of moving forward (as toward a goal)",
            "gradual improvement or growth or development",
        ],
    },
    {
        "word": "faces",
        "meanings": [
            "the front of the human head from the forehead to the chin and ear to ear",
            "the feelings expressed on a person's face",
            "the general outward appearance of something",
            "the striking or working surface of an implement",
            "a part of a person that is used to refer to a person",
            "a surface forming part of the outside of an object",
            "the part of an animal corresponding to the human face",
            "the side upon which the use of a thing depends (usually the most prominent surface of an object)",
            "a contorted facial expression",
            "a specific size and style of type within a type family",
            "status in the eyes of others",
            "impudent aggressiveness",
            "a vertical surface of a building or cliff",
            "deal with (something unpleasant) head on",
            "oppose, as in hostility or a competition",
            "be oriented in a certain direction, often with respect to another reference point; be opposite to",
            "be opposite",
            "turn so as to face; turn the face in a certain direction",
            "present somebody with something, usually to accuse or criticize",
            "turn so as to expose the face",
            "line the edge (of a garment) with a different material",
            "cover the front or surface of",
        ],
    },
    {
        "word": "challenges",
        "meanings": [
            "a demanding or stimulating situation",
            "a call to engage in a contest or fight",
            "questioning a statement and demanding an explanation",
            "a formal objection to the selection of a particular person as a juror",
            "a demand by a sentry for a password or identification",
            "take exception to",
            "issue a challenge to",
            "ask for identification",
            "raise a formal objection in a court of law",
        ],
    },
    {
        "word": "related",
        "meanings": [
            "make a logical or causal connection",
            "be relevant to",
            "give an account of",
            "be in a relationship with",
            "have or establish a relationship to",
            "being connected either logically or causally or by shared characteristics",
            "connected by kinship, common origin, or marriage",
        ],
    },
    {
        "word": "poverty",
        "meanings": [
            "the state of having little or no money and few or no material possessions"
        ],
    },
    {
        "word": "healthcare",
        "meanings": [
            "the preservation of mental and physical health by preventing or treating illness through services offered by the health profession"
        ],
    },
    {
        "word": "environmental",
        "meanings": [
            "of or relating to the external conditions or surroundings",
            "concerned with the ecological effects of altering the environment",
        ],
    },
    {"word": "sustainability", "meanings": ["the property of being sustainable"]},
    {
        "word": "prompting",
        "meanings": [
            "persuasion formulated as a suggestion",
            "a cue given to a performer (usually the beginning of the next line to be spoken)",
            "give an incentive for action",
            "serve as the inciting cause of",
            "assist (somebody acting or reciting) by suggesting the next words of something forgotten or imperfectly learned",
        ],
    },
    {"word": "ongoing", "meanings": ["currently happening"]},
    {
        "word": "efforts",
        "meanings": [
            "earnest and conscientious activity intended to do or accomplish something",
            "use of physical or mental energy; hard work",
            "a notable achievement",
            "a series of actions advancing a principle or tending toward a particular end",
        ],
    },
    {
        "word": "inclusive",
        "meanings": [
            "including much or everything; and especially including stated limits"
        ],
    },
    {
        "word": "development",
        "meanings": [
            "act of improving by expanding or enlarging or refining",
            "a process in which something passes by degrees to a different stage (especially a more advanced or mature stage)",
            "(biology) the process of an individual organism growing organically; a purely biological unfolding of events involved in an organism changing gradually from a simple to a more complex level",
            "a recent event that has some relevance for the present situation",
            "the act of making some area of land or water more profitable or productive or useful",
            "a district that has been developed to serve some purpose",
            "a state in which things are improving; the result of developing (as in the early part of a game of chess)",
            "processing a photosensitive material in order to make an image visible",
            "(music) the section of a composition or movement (especially in sonata form) where the major musical themes are developed and elaborated",
        ],
    },
    {
        "word": "political",
        "meanings": [
            "involving or characteristic of politics or parties or politicians; - Daniel Goleman",
            "of or relating to your views about social relationships involving authority or power",
            "of or relating to the profession of governing",
        ],
    },
    {
        "word": "robust",
        "meanings": [
            "sturdy and strong in form, constitution, or construction",
            "marked by richness and fullness of flavor",
            "strong enough to withstand or overcome intellectual challenges or adversity",
            "rough and crude",
        ],
    },
    {
        "word": "democratic",
        "meanings": [
            "characterized by or advocating or based upon the principles of democracy or social equality; ; ; - George du Maurier",
            "belong to or relating to the Democratic Party",
            "representing or appealing to or adapted for the benefit of the people at large",
        ],
    },
    {
        "word": "system",
        "meanings": [
            "instrumentality that combines interrelated interacting artifacts designed to work as a coherent entity",
            "a group of independent but interrelated elements comprising a unified whole",
            "(physical chemistry) a sample of matter in which substances in different phases are in equilibrium",
            "a complex of methods or rules governing behavior",
            "an organized structure for arranging or classifying",
            "a group of physiologically or anatomically related organs or parts",
            "a procedure or process for obtaining an objective",
            "the living body considered as made up of interdependent components forming a unified whole",
            "an ordered manner; orderliness by virtue of being methodical and well organized",
        ],
    },
    {
        "word": "parties",
        "meanings": [
            "an organization to gain political power",
            "a group of people gathered together for pleasure",
            "a band of people associated temporarily in some activity",
            "an occasion on which people can assemble for social interaction and entertainment",
            "a person involved in legal proceedings",
            "have or participate in a party",
        ],
    },
    {
        "word": "gained",
        "meanings": [
            "obtain",
            "win something through one's efforts",
            "derive a benefit from",
            "reach a destination, either real or abstract",
            "obtain advantages, such as points, etc.",
            "rise in rate or price",
            "increase or develop",
            "earn on some commercial or business transaction; earn as salary or wages",
            "increase (one's body weight)",
        ],
    },
    {
        "word": "independence",
        "meanings": [
            "freedom from control or influence of another or others",
            "the successful ending of the American Revolution",
            "a city in western Missouri; the beginning of the Santa Fe Trail",
        ],
    },
    {
        "word": "British",
        "meanings": [
            "the people of Great Britain",
            "of or relating to or characteristic of Great Britain or its people or culture",
        ],
    },
    {
        "word": "rule",
        "meanings": [
            "a principle or condition that customarily governs behavior",
            "something regarded as a normative example",
            "prescribed guide for conduct or action",
            "(linguistics) a rule describing (or prescribing) a linguistic practice",
            "a basic generalization that is accepted as true and that can be used as a basis for reasoning or conduct",
            "the duration of a monarch's or government's power",
            "dominance or power through legal authority",
            "directions that define the way a game or sport is to be conducted",
            "any one of a systematic body of regulations defining the way of life of members of a religious order",
            "a rule or law concerning a natural phenomenon or the function of a complex system",
            "(mathematics) a standard procedure for solving a class of mathematical problems",
            "measuring stick consisting of a strip of wood or metal or plastic with a straight edge that is used for drawing straight lines and measuring lengths",
            "exercise authority over; as of nations",
            "decide with authority",
            "be larger in number, quantity, power, status or importance",
            "decide on and make a declaration about",
            "have an affinity with; of signs of the zodiac",
            "mark or draw with a ruler",
            "keep in check",
        ],
    },
    {"word": "1947", "meanings": []},
    {
        "word": "led",
        "meanings": [
            "diode such that light emitted at a p-n junction is proportional to the bias current; color depends on the material used",
            "take somebody somewhere",
            "have as a result or residue",
            "tend to or result in",
            "travel in front of; go in advance of others",
            "cause to undertake a certain action",
            "stretch out over a distance, space, time, or scope; run or extend between two points or beyond a certain point",
            "be in charge of",
            "be ahead of others; be the first",
            "be conducive to",
            "lead, as in the performance of a composition",
            "lead, extend, or afford access",
            "move ahead (of others) in time or space",
            "cause something to pass or lead somewhere",
            "preside over",
        ],
    },
    {"word": "Mahatma", "meanings": ["(Hinduism) term of respect for a brahmin sage"]},
    {
        "word": "Gandhi",
        "meanings": [
            "daughter of Nehru who served as prime minister of India from 1966 to 1977 (1917-1984)",
            "political and spiritual leader during India's struggle with Great Britain for home rule; an advocate of passive resistance (1869-1948)",
        ],
    },
    {
        "word": "other",
        "meanings": [
            "not the same one or ones already mentioned or implied; - the White Queen",
            "recently past",
            "belonging to the distant past",
            "very unusual; different in character or quality from the normal or expected; - Lance Morrow",
        ],
    },
    {
        "word": "prominent",
        "meanings": [
            "having a quality that thrusts itself into attention",
            "conspicuous in position or importance",
        ],
    },
    {
        "word": "leaders",
        "meanings": [
            "the body of people who lead a group",
            "a person who rules or guides or inspires others",
            "a featured article of merchandise sold at a loss in order to draw customers",
        ],
    },
    {
        "word": "commitment",
        "meanings": [
            "the trait of sincere and steadfast fixity of purpose",
            "the act of binding yourself (intellectually or emotionally) to a course of action",
            "an engagement by contract involving financial obligation",
            "a message that makes a pledge",
            "the official act of consigning a person to confinement (as in a prison or mental hospital)",
        ],
    },
    {
        "word": "democracy",
        "meanings": [
            "the political orientation of those who favor government by the people or by their elected representatives",
            "a political system in which the supreme power lies in a body of citizens who can elect people to represent them",
            "the doctrine that the numerical majority of an organized group can make decisions binding on the whole group",
        ],
    },
    {
        "word": "evident",
        "meanings": [
            "clearly revealed to the mind or the senses or judgment",
            "capable of being seen or noticed",
        ],
    },
    {
        "word": "vibrant",
        "meanings": [
            "vigorous and animated",
            "of sounds that are strong and resonating",
            "of colors that are bright and striking",
        ],
    },
    {
        "word": "elections",
        "meanings": [
            "a vote to select the winner of a position or political office",
            "the act of selecting someone or something; the exercise of deliberate choice",
            "the status or fact of being elected",
            "the predestination of some individuals as objects of divine mercy (especially as conceived by Calvinists)",
        ],
    },
    {
        "word": "millions",
        "meanings": [
            "the number that is represented as a one followed by 6 zeros",
            "a very large indefinite number (usually hyperbole)",
        ],
    },
    {
        "word": "citizens",
        "meanings": [
            "a native or naturalized member of a state or other political community"
        ],
    },
    {
        "word": "participate",
        "meanings": ["share in something", "become a participant; be involved in"],
    },
    {
        "word": "shaping",
        "meanings": [
            "any process serving to define the shape of something",
            "the act of fabricating something in a particular shape",
            "shape or influence; give direction to",
            "make something, usually for a specific function",
            "give shape or form to",
            "forming or capable of forming or molding or fashioning",
        ],
    },
    {
        "word": "nation",
        "meanings": [
            "a politically organized body of people under a single government",
            "the people who live in a nation or country",
            "United States prohibitionist who raided saloons and destroyed bottles of liquor with a hatchet (1846-1911)",
            "a federation of tribes (especially Native American tribes)",
        ],
    },
    {
        "word": "future",
        "meanings": [
            "the time yet to come",
            "a verb tense that expresses actions or states in the future",
            "bulk commodities bought or sold at an agreed price for delivery at a specified future date",
            "yet to be or coming",
            "effective in or looking toward the future",
            "(of elected officers) elected but not yet serving",
            "a verb tense or other formation referring to events or states that have not yet happened",
        ],
    },
}
```

-----

### Extract words and their respective frequencies from the text

```python
print(enalsis.count_words(text_para))
```

Output - The provided data is a list of tuples, where each tuple contains an element that is a string representing a word and the second element is an integer representing the frequency or count of occurrences of that word.

```python
[
    ("india", 9),
    ("is", 7),
    ("a", 11),
    ("vast", 1),
    ("and", 12),
    ("diverse", 4),
    ("country", 7),
    ("located", 1),
    ("in", 12),
    ("south", 2),
    ("asia", 1),
    ("known", 1),
    ("for", 2),
    ("its", 3),
    ("rich", 2),
    ("history", 2),
    ("cultures", 1),
    ("varied", 1),
    ("landscapes", 1),
    ("with", 3),
    ("population", 1),
    ("of", 13),
    ("over", 1),
    ("1", 1),
    ("3", 1),
    ("billion", 1),
    ("people", 1),
    ("the", 22),
    ("second", 1),
    ("most", 1),
    ("populous", 1),
    ("world", 3),
    ("characterized", 2),
    ("by", 3),
    ("harmonious", 1),
    ("blend", 1),
    ("tradition", 1),
    ("modernity", 1),
    ("where", 2),
    ("ancient", 2),
    ("customs", 1),
    ("coexist", 1),
    ("rapidly", 1),
    ("evolving", 1),
    ("urban", 1),
    ("lifestyles", 1),
    ("geographically", 1),
    ("boasts", 1),
    ("wide", 1),
    ("range", 1),
    ("terrains", 1),
    ("from", 2),
    ("snow", 1),
    ("capped", 1),
    ("himalayan", 1),
    ("mountains", 1),
    ("north", 1),
    ("to", 6),
    ("tropical", 1),
    ("beaches", 1),
    ("home", 1),
    ("myriad", 1),
    ("ecosystems", 1),
    ("supporting", 1),
    ("array", 2),
    ("flora", 1),
    ("fauna", 1),
    ("ganges", 1),
    ("one", 2),
    ("holiest", 1),
    ("rivers", 1),
    ("hinduism", 1),
    ("flows", 1),
    ("through", 1),
    ("heart", 1),
    ("playing", 1),
    ("vital", 1),
    ("role", 1),
    ("cultural", 2),
    ("spiritual", 1),
    ("fabric", 1),
    ("s", 6),
    ("heritage", 1),
    ("reflected", 1),
    ("numerous", 1),
    ("festivals", 1),
    ("art", 1),
    ("forms", 1),
    ("classical", 1),
    ("dance", 1),
    ("music", 1),
    ("traditions", 1),
    ("has", 2),
    ("long", 1),
    ("contributions", 1),
    ("science", 1),
    ("mathematics", 1),
    ("literature", 1),
    ("philosophy", 1),
    ("texts", 1),
    ("such", 1),
    ("as", 2),
    ("vedas", 1),
    ("upanishads", 1),
    ("have", 2),
    ("left", 1),
    ("an", 1),
    ("indelible", 1),
    ("mark", 1),
    ("on", 1),
    ("intellectual", 1),
    ("landscape", 2),
    ("indian", 1),
    ("economy", 2),
    ("undergone", 1),
    ("significant", 1),
    ("transformation", 1),
    ("recent", 1),
    ("decades", 1),
    ("emerging", 1),
    ("fastest", 1),
    ("growing", 1),
    ("major", 1),
    ("economies", 1),
    ("information", 1),
    ("technology", 1),
    ("software", 1),
    ("services", 1),
    ("burgeoning", 1),
    ("startup", 1),
    ("ecosystem", 1),
    ("contributed", 1),
    ("position", 1),
    ("global", 1),
    ("despite", 1),
    ("these", 1),
    ("advancements", 1),
    ("faces", 1),
    ("challenges", 1),
    ("related", 1),
    ("poverty", 1),
    ("healthcare", 1),
    ("environmental", 1),
    ("sustainability", 1),
    ("prompting", 1),
    ("ongoing", 1),
    ("efforts", 1),
    ("inclusive", 1),
    ("development", 1),
    ("political", 2),
    ("robust", 1),
    ("democratic", 1),
    ("system", 1),
    ("parties", 1),
    ("gained", 1),
    ("independence", 1),
    ("british", 1),
    ("rule", 1),
    ("1947", 1),
    ("led", 1),
    ("mahatma", 1),
    ("gandhi", 1),
    ("other", 1),
    ("prominent", 1),
    ("leaders", 1),
    ("commitment", 1),
    ("democracy", 1),
    ("evident", 1),
    ("vibrant", 1),
    ("elections", 1),
    ("millions", 1),
    ("citizens", 1),
    ("participate", 1),
    ("shaping", 1),
    ("nation", 1),
    ("future", 1),
]
```

-----

### Extract alphabetical and numerical percentage from the text

```python
print(enalsis.calculate_alphabetical_and_numberical_percentages(text_para))
```

Output - The output is in the format of numbers represnting the percentage of alphabets, numbers and white space present in the text.

```python
(84.65092402464066, 0.3080082135523614, 15.041067761806982)
```

-----