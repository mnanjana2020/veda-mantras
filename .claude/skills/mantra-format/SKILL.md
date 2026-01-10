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
        Roman script version<br><br>

        <strong>Translation:</strong><br>
        English meaning
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
3. **Translation**: Clear, accessible English
4. **Commentary**: Include historical context, word meanings, and spiritual significance

## CSS Classes Available

- `.mantra` - Styled box for Sanskrit text
- `.translation` - Italicized translation block
- `.analysis` - Commentary section
- `.blessing` - Featured quote box
- `.divider` - Decorative separator
