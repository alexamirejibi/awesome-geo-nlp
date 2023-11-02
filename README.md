# NLP resources for the Georgian language
(Stuff I've encountered so far)

## Models
- [Davit6174/georgian-distilbert-mlm · Hugging Face](https://huggingface.co/Davit6174/georgian-distilbert-mlm)
- [jnz/electra-ka · Hugging Face](https://huggingface.co/jnz/electra-ka)
	- More on jnz's profile

## Tools
Some projects working on Georgian NLP tools:
- [ანბანი ჻ Anbani Georgia · GitHub](https://github.com/anbani)
	- "Collection of Web and AI tools designed to equip Georgian Language and Alphabet with the challenges of digital age ჻ ᲐᲜᲑᲐᲜᲘ"
	- [nano](https://github.com/Anbani/nano) - bare-bones Georgian script converter
	- [anbani.py](https://github.com/Anbani/anbani.py) - Georgian Python toolkit for NLP, Transliteration and more
	- [TextArt](https://github.com/Anbani/TextArt) - Georgian Text Art Generator
	- [anbani.js](https://github.com/Anbani/anbani.js) - Multifunctional javascript toolkit for Georgian Alphabet - Anbani
	- [word-embeddings](https://github.com/Anbani/word-embeddings)
	- [anbani.db](https://github.com/Anbani/anbani.db) - Various Georgian datasets
- https://qartnlp.iliauni.edu.ge/ s
- [screeve · GitHub](https://github.com/screeve)
	- [lemmatizer](https://github.com/screeve/lemmatizer) - Lemmatization functionality for Georgian language.
	- [postagger](https://github.com/screeve/postagger) - Part-of-speech tagging functionality for Georgian language.
	- [embeddings](https://github.com/screeve/embeddings) - pre-trained embeddings for Georgian language

## Datasets
- [WikiANN](https://huggingface.co/datasets/wikiann/viewer/ka) - NER dataset

## Linguistic resources
- [[Sparklis] Kartu-Verbs: A Semantic Web Base of Inflected Georgian Verb Forms to Bypass Georgian Verb Lemmatization Issues](http://www.irisa.fr/LIS/ferre/sparklis/osparklis.html?title=Kartu-Verbs%3A%20Georgian%20Verb%20Forms%26lt%3Bbr%26gt%3B&endpoint=http%3A//servolis.irisa.fr%3A3737/kartuverbs/sparql&sparklis-query=%5BVId%5DReturn%28Det%28An%281%2CModif%28Select%2CUnordered%29%2CClass%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/verb%22%29%29%2CSome%28And%28Rel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/Georgian_form%22%2CFwd%2CDet%28An%2838%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/person%22%2CFwd%2CDet%28An%2842%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/number%22%2CFwd%2CDet%28An%2846%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/tense%22%2CFwd%2CDet%28An%2850%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/preverb%22%2CFwd%2CDet%28An%2854%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/preradical%22%2CFwd%2CDet%28An%2858%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/root%22%2CFwd%2CDet%28An%2862%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/postradical%22%2CFwd%2CDet%28An%2866%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/pFSF%22%2CFwd%2CDet%28An%2870%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/ending%22%2CFwd%2CDet%28An%2874%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/English_infinitive%22%2CFwd%2CDet%28An%2878%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/French_infinitive%22%2CFwd%2CDet%28An%2882%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%2CRel%28%22file%3A///home/ferre/data/ontologies/Kartu-verbs/Georgian_infinitive%22%2CFwd%2CDet%28An%2886%2CModif%28Select%2CUnordered%29%2CThing%29%2CNone%29%29%29%29%29%29&sparklis-path=D&regexp_hidden_URIs=&entity_lexicon_select=http%3A//www.w3.org/2000/01/rdf-schema%23label&concept_lexicons_select=http%3A//www.w3.org/2000/01/rdf-schema%23label&short-permalink=false)
	- [Paper](https://hal.science/hal-02924019)
## Research notes and questions
- Georgia is a highly inflectional language (a lot of word forms, see the Sparklis link above), which has notable implications. FastText is probably the best non-transformer embedding model for inflectional languages thanks to subword embeddings - see [Comprehensive Evaluation of Word Embeddings for Highly Inflectional Language](https://link.springer.com/chapter/10.1007/978-3-030-88113-9_48). Transformer alternatives are "more powerful" but inefficient and costly.
 
## Contributions
- I'm seeking input from other researchers and practitioners on best practices and useful resources for doing NLP in Georgian. Please contribute what you can, especially general wisdom.
