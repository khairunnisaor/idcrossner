# IDCrossNER: An Indonesian specific-domain NER dataset
This dataset is an adapted cross-domain NER dataset in the Indonesian language that covers five different domains: science, politics, music, literature, and artificial intelligence (AI). We translated and projected an English cross-domain NER dataset, CrossNER (https://github.com/zliucr/CrossNER), to the Indonesian language and performed manual corrections to ensure the dataset consistency and reliability.

Entity list of each domain and the number of sentences in each split (train/dev/test) are described below.
- Politics (9): country, election, event, location, organization, person, political party, politician, and misc. (200/541/651)
- Science (16): academic journal, astronomical object, award, chemical compound, country, discipline, enzyme, event, location, organization, person, protein, scientist, theory, university, and misc. (200/450/543)
- Music (12): album, award, band, event, location, musical artist, musical instrument, music genre, organization, person, song, and misc. (100/380/456)
- Literature (12): award, book, country, event, literary genre, location, magazine, organization, person, poem, writer, and misc. (100/400/416)
- AI (14): algorithm, conference, country, field, location, metrics, organization, person, product, program lang, researcher, task, university, and misc. (100/350/431)

The format is following CoNLL dataset which split each token into one line and each sentence is separated by one empty line. For the NER tag, we use the IOB format as illustrated in the example below.

Example:
```
Tahun	O
berikutnya	O
mereka	O
berkolaborasi	O
dalam	O
versi	O
film	O
musikal	O
Si	B-book
Pangeran	I-book
Kecil	I-book
,	O
berdasarkan	O
klasik	O
anak-anak	O
karya	O
Antoine	B-writer
de	I-writer
Saint-Exupéry	I-writer
.	O

Dalam	O
majalah	O
The	B-magazine
Crisis	I-magazine
pada	O
1943	O
,	O
Harold	B-writer
Preece	I-writer
mengkritik	O
Hurston	B-writer
karena	O
melestarikan	O
primitivisme	B-literarygenre
Negro	I-literarygenre
untuk	O
memajukan	O
karir	O
sastranya	O
sendiri	O
.	O
```

# Research Paper
(TBA)
