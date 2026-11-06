# Zabaykalsky Krai: catalogue of laws in git

Part of [lexifina/global-law](https://github.com/lexifina/global-law), one git history for every country's law: this is the law of Zabaykalsky Krai, Russia, which global-law reads at `russia/zabaykalsky/acts/`.

**Facts only: no law text.**

A catalogue of the laws of Zabaykalsky Krai (Забайкальский край), a federal subject of the Russian Federation, as a git history: one file per law, holding the facts the Official Internet Portal of Legal Information gives for it, added on the day the portal published it. `git log` lists the laws in the order they were published; checking out a date shows which laws had been published by then.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law). The federal law of Russia is in [lexifina/russia-law](https://github.com/lexifina/russia-law).

## What this repository holds

1,638 laws published from 2014-12-03 to 2026-10-28 (281 publication days): every document of a law type the portal lists for Zabaykalsky Krai (laws, charter or constitutional laws, the charter or constitution and the laws amending it). Decrees, resolutions and orders are not included.

Each file, `zakony-<year>/<number>.md` (the year of publication, the law's number in Latin letters), holds:

- the official title;
- the document type and number;
- the date signed and the publication date;
- the electronic publication number;
- the signing body the portal names;
- the link to the law's official publication page on the portal, where its text can be read.

No text of any law is copied.

## Source

The [Official Internet Portal of Legal Information](http://publication.pravo.gov.ru/documents/block/region75) (Официальный интернет-портал правовой информации, publication.pravo.gov.ru), section Забайкальский край: its metadata API (`/api/Documents`), read on 2026-10-30. The portal's open data may be reused freely, keeping a link to the source (http://publication.pravo.gov.ru/OpenData).

## Dates

Each law is added on the day the portal published it, at noon Asia/Chita time, and credited to the portal. Publication on the portal is official publication, but a law may take effect on another day: read its own text.

## How it is checked

- Every version is read back from git on its day and on the day before, and must match the corpus.
- Every file's facts are compared, field by field, with the portal's API records, read by a second, independent reader.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future.

## Limits

This is not an official publication. The catalogue lists what the portal holds; its sections for the federal subjects start in the 2010s, so older laws are missing. It does not say whether a law is in force, has been amended or has lapsed.

---

# Забайкальский край: каталог законов в git

**Только сведения: без текстов законов.**

Каталог законов субъекта Российской Федерации по данным Официального интернет-портала правовой информации (publication.pravo.gov.ru): один файл на закон (наименование, вид, номер, дата подписания, дата опубликования, номер электронного опубликования, принявший орган и ссылка на страницу опубликования), один коммит на день опубликования. Это не официальное опубликование.
