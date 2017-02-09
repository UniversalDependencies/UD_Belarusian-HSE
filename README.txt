The Belarusian UD treebank is based on a sample of the news texts included in the Belarusian-Russian parallel subcorpus of the Russian National Corpus.

=== Machine-readable metadata =================================================
Documentation status: stub
Data source: manual
Data available since: UD v2.0
License: CC BY-SA 4.0
Genre: news
Contributors: Lyashevskaya, Olga
Contact: olesar@yandex.ru
===============================================================================

The treebank is based on a sample of the news texts included in the Belarusian-Russian parallel subcorpus of the Russian National Corpus,
online search available at: http://ruscorpora.ru/search-para.html. 

TOKENIZATION

The tokenization is mostly straightforward based on whitespace and punctuation.

- Numerical expressions including non-integers (e.g. "245", "3,14") are treated as single tokens. 
- Time expressions like "20:55" are splitted into separate tokens (in this case, three {20, :, 55} ). 
- Dates like "20.04.2012" are splitted into separate tokens (in this case, five {20, ., 04, ., 2012} ). 
- Special symbols before and after numerical expressions (e.g. "$500", "2,67%") are tokenised separately.
- Numerical expressions with hyphen and cyrillic endings (e.g. "1-ый", "3-м") as well as adjectives and other non-numerals which contain digits (e.g. "18-летний", "500-летие") are treated as single tokens. 
- Other words with hyphen are treated as single tokens, except cases then the first part is inflected. Examples: {зелено-серый}, but {Ростове, -, на, -, Дону}. Words with пол- are treated as single tokens: {пол-яблока}. 
- Abbreviations are treated as single tokens, whitespaces split the abbreviations.
- Email addresses, URLs, and tweet-style names are treated as single tokens: {no@mail.ru}, {https://github.com}, {@anna_li}

The Belarusian UD treebank does not contain multiword tokens.

MORPHOLOGY

The morphological annotation is adopted from the Russian-Syntagrus UD guidelines and mostly compliant with the RNC morphological standard (exept for "second" cases, comp2, imper2, and transitivity tags). 
Lemmas and features were annotated manually.

SYNTAX
The data were labeled semi-automatically using the annotation projection from Russian. For that purpose, Russian data were annotated using UDpipe, converted into UD 2.0, and then checked manually.
Belarusian dependency relation tags were checked manually.

TEXTS

The source texts are short news articles originally written in Belarusian (and/)or Russian, published by telegraf.by online agency.

Document list: 
http://search2.ruscorpora.ru/search.xml?env=alpha&text=meta&sort=gr_tagging&lang=ru&doc_g_number_lang=&doc_te_author=&mode=para&doc_te_header=*&author=&doc_g_birthday=&doc_l_birthday=&doc_g_created=&doc_l_created=&doc_te_translator=&doc_lang=bel&doc_lang_trans=rus&doc_g_date_date_trans=&doc_l_date_date_trans=&doc_sphere=%EF%F3%E1%EB%E8%F6%E8%F1%F2%E8%EA%E0

Acknowledgments:

We thank Uladzimir Koshchanka (Уладзімір Кошчанка, koshul@gmail.com) for providing the source texts. 
