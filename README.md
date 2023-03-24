# Dictionaries data sources

This repository contains a different dictionaries in JSON format. The JSON structure is as follows:

```json
{
  "name": "dictionary_name",
  "url": "source_url",
  "expressionLanguageId": "lez",
  "definitionLanguageId": "rus",
  "dictionary": [
    {
      "spelling": "word_spelling",
      "definitions": [
        "definition_1",
        "definition_2",
        ...
      ]
    },
    ...
  ]
}
```

## Fields

- `name`: The name of the dictionary, e.g., "ЛЕЗГИНСКО-РУССКИЙ СЛОВАРЬ 2018 (Бабаханов М.Б)".
- `url`: The source URL of the dictionary (if available).
- `expressionLanguageId`: The language code for the words being defined, in this case, "lez" for Lezgian.
- `definitionLanguageId`: The language code for the definitions, in this case, "rus" for Russian.
- `dictionary`: An array of dictionary entries.

## Dictionary Entry

- `spelling`: The word being defined.
- `definitions`: An array of definitions for the word. Each definition is a string.

## Example

```json
{
  "name": "ЛЕЗГИНСКО-РУССКИЙ СЛОВАРЬ 2018 (Бабаханов М.Б)",
  "url": "",
  "expressionLanguageId": "lez",
  "definitionLanguageId": "rus",
  "dictionary": [
    {
      "spelling": "А",
      "definitions": [
        "I первая буква лезгинского алфавита"
      ]
    },
    {
      "spelling": "А",
      "definitions": [
        "II мест. указ. тот, та, то (о предмете, который находится вне поля зрения говорящего и о котором знает собеседник); <см.тж.> {абур}",
        ...
      ]
    },
    ...
  ]
}
```

The above example demonstrates the JSON structure for the Lezgian-Russian dictionary. Each entry contains the word spelling and an array of definitions for that word.
