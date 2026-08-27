# Book 1 spec v3: The Machine, 5 parts, Marathi-English Devanagari

## Decision history
- v2 (Hinglish, 5 parts) archived at book/archive/book1-v2-hinglish-*.
- v3 after user saw Part 2 Hinglish + Part 3 Devanagari: wants ALL
  parts in Marathi-English Devanagari, analogy-heavy. 30 MCQs answered
  2026-08-27; encoded below.

## Language
1. Marathi-English mix, Devanagari script, all 5 parts.
2. Spoken simple Marathi (boli-bhasha). Clarity > shuddha-lekhan.
3. Technical nouns ALWAYS English in Roman: server, packet, DNS, code.
4. Short-medium sentences; emphasis via **bold** (no caps in Devanagari).
5. Numbers: million/billion first, lakh/crore in brackets when helpful.
6. No em-dashes, no emojis.

## Analogies (core upgrade)
7. One desi analogy per section of each chapter.
8. Rotate 4 worlds: vehicles/traffic, dhaba/kitchen, gaon/bazaar,
   post/bank/sarkar-office.
9. Company examples 50-50 India/global.

## Chapter shape
10. Body: problem-first; term names (bold) and company example WOVEN
    INTO body. No separate NAAV / EXAMPLE sections.
11. Sections after body, in order:
    - इथे लोक काय चुकीचं समजतात
    - MAP वर (concise; 85% tech / 15% paisa overall)
    - स्वतः बघा (5 minute)
    - विचार करा (1 derivation Q, answer below in > quote)
12. NO Madhav-Kabir dialogue anywhere.
13. ~3 pages/chapter. [SPINE]/[DEPTH] kept. Diagrams only where needed.
14. Geopolitics windows kept where natural. No user-personal business
    references.

## Part shape
15. Front matter: 5-part naksha + "तुम्ही इथे आहात"; Part 2+ starts
    with 5-question recap of previous part (answers below).
16. Section openers: 3-4 lines business-decision relevance.
17. Part end: naksha-table + 4-question self-test + next-part preview
    + mini-glossary. Part 5 additionally: master glossary + full map.
18. PDF: --cover, NO --toc. Each part its own PDF (separate binding).

## Process
19. One part at a time; user OK gates the next.
20. Delivery: PDF + auto-verify report (shingle 0-missing, structure,
    font, stray-script scan, spot render).

## Layout
Folders book/book1/part{1..5}/; files: 000 front matter, x00 section
openers, x01+ chapters, 900 part-end; BOOK.md assembled with blank-line
joins; H1 = page break (generator CSS).
Titles: "The Machine, Part N: <Marathi name>".
Parts: 1 पैसा आणि Machine (16ch: cur. 0,1,2) | 2 Machine शी बोलणं
(12ch: cur. 3,4) | 3 Machines चं जाळं (8ch: cur. 5) | 4 Data आणि आठवणी
(7ch: cur. 6) | 5 जगाला Serve करणं (15ch: cur. 7,8).
