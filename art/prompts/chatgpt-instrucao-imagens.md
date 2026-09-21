# Instrução para o ChatGPT (anexar os arquivos)

Anexe ao chat estes 5 arquivos:
- `art/style-bible.md`
- `art/prompts/concept/char-aquiles.v1.md`
- `art/prompts/concept/char-agamemnon.v1.md`
- `art/prompts/concept/char-odisseu.v1.md`
- `art/prompts/concept/char-heitor.v1.md`

Depois cole o texto abaixo.

```
I attached five Markdown files for my game's character concept art.

1. style-bible.md: contains the STYLE BLOCK and the NEGATIVES BLOCK (each inside a code block).
2. char-aquiles.v1.md, char-agamemnon.v1.md, char-odisseu.v1.md, char-heitor.v1.md: each contains the CHARACTER BLOCK for one character (inside a code block).

Task: generate four images, ONE per reply, in this order: Achilles, Agamemnon, Odysseus, Hector. After each image, stop and wait for me to say "next".
- For each character, build the image prompt by joining, in this order and without changing any word: STYLE BLOCK, then that character's CHARACTER BLOCK, then NEGATIVES BLOCK.
- Ignore the Portuguese text outside the code blocks; it is documentation.
- Where a CHARACTER BLOCK conflicts with the STYLE BLOCK (for example a character holding a sceptre or spear), the CHARACTER BLOCK wins.
- Keep exactly the same painterly art style, lighting, palette, framing and plain light-gray background in all four images, so they look like one set. From the second image on, use the previous images as style reference.
- Follow every detail literally. Do not add elements that are not in the files.
- Return only the image, then one line listing anything you could not follow.
```
