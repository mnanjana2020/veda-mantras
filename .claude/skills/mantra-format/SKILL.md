---
name: mantra-format
description: Format and add new Vedic mantras to the website. Use when adding mantras, formatting Sanskrit text, or creating mantra pages.
---

# Mantra Formatting Skill

When adding new mantras to the Veda Mantras website, follow this structure:

## HTML Structure for Each Mantra

```html
<section>
    <h2>Mantra Name</h2>
    <p><strong>Source Reference</strong> — Brief description</p>

    <div class="mantra">
        Sanskrit text here (Devanagari script)
    </div>

    <div class="translation">
        <strong>Transliteration:</strong><br>
        IAST Roman script version<br><br>

        <strong>Word-by-Word:</strong><br>
        Sanskrit (transliteration) — meaning<br>
        Sanskrit (transliteration) — meaning<br>
        ... (continue for each word/term)<br><br>

        <strong>Translation:</strong><br>
        Complete English meaning
    </div>

    <div class="analysis">
        <h3>Commentary</h3>
        <p>Explanation and significance</p>
    </div>
</section>
```

## Style Guidelines

1. **Sanskrit text**: Use Devanagari Unicode characters
2. **Transliteration**: Use IAST (International Alphabet of Sanskrit Transliteration)
3. **Word-by-Word**: REQUIRED - Break down each significant word with:
   - Devanagari form
   - IAST transliteration in parentheses
   - English meaning after em-dash (—)
4. **Translation**: Clear, accessible English summary
5. **Commentary**: Include historical context, word meanings, and spiritual significance

## Word-by-Word Format Example

```html
<strong>Word-by-Word:</strong><br>
ॐ (Om) — the primordial sound, representing the divine<br>
भूर् (Bhūr) — earth, the physical plane<br>
भुवः (Bhuvaḥ) — atmosphere, the mental plane<br>
स्वः (Svaḥ) — heaven, the spiritual plane<br>
```

## CSS Classes Available

- `.mantra` - Styled box for Sanskrit text
- `.translation` - Italicized translation block (includes word-by-word)
- `.analysis` - Commentary section
- `.blessing` - Featured quote box
- `.divider` - Decorative separator

## Important Notes

- Every mantra MUST include word-by-word translation
- Group compound words together when appropriate
- Include grammatical notes where helpful (e.g., "dative plural", "vocative")
- For long mantras, translate all key terms; minor particles (ca, vai) can be grouped
