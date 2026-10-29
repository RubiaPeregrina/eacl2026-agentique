# Ancient Greek lemmatization and POS tagging

Intended for linguists specializing in Ancient Greek, the project has created a database containing Ancient Greek words along with their lemmas and associated part-of-speech (POS) tags in .tsv format, and now needs help tagging new, previously unpublished Ancient Greek texts.


One input token = one output row
Only tags from data/tagsets/GRC_tagset.txt (see skill annotation-grc).


Send the text to the “tagger” subagent (task tool). This subagent generates the output/annotation.tsv file.
Send the text to the “proofreader” subagent. This subagent returns a report in text format.
If the report contains errors or suggestions, send it back to the “tagger” for an initial round of corrections.
Copy the result to the output/final.tsv file and summarize: number of tokens, corrections made, and unresolved issues.

