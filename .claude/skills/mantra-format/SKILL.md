---
name: mantra-format
description: Format and analyze Vedic mantras with multi-language support (English, Devanagari, Kannada). Use when adding mantras, formatting Sanskrit text, or creating mantra pages.
---

# Mantra Analysis Skill

When adding new mantras to the Veda Mantras website, follow this comprehensive structure based on the CHATGPT GURU format.

## Output Structure

### 1. Mantra Header
```html
<article class="mantra-entry">
    <header>
        <h2>Sanskrit Name / English Name</h2>
        <p class="source"><strong>Source:</strong> [Veda Name], [Mandala/Book], [Sukta], Verse [Number]</p>
        <p class="description">Brief description of the mantra's significance</p>
    </header>
```

### 2. Multi-Language Text Block
Present the mantra in ALL THREE scripts (required):

```html
    <section class="mantra-text">
        <h3>Mantra Text</h3>
        <div class="script kannada">
            <h4>ಕನ್ನಡ</h4>
            ಕನ್ನಡ ಲಿಪಿಯಲ್ಲಿ ಮಂತ್ರ
        </div>
        <div class="script devanagari">
            <h4>देवनागरी</h4>
            देवनागरी में मन्त्र
        </div>
        <div class="script transliteration">
            <h4>IAST Transliteration</h4>
            Romanized transliteration with diacritics
        </div>
    </section>
```

### 3. Word-by-Word Analysis (Table Format - REQUIRED)
Break down EVERY significant word in a table:

```html
    <section class="word-analysis">
        <h3>Word-by-Word Analysis</h3>
        <table class="analysis-table">
            <thead>
                <tr>
                    <th>Sanskrit (देवनागरी)</th>
                    <th>Transliteration</th>
                    <th>English Meaning</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>संस्कृत शब्द</td>
                    <td>saṃskṛta śabda</td>
                    <td>meaning (grammatical note if helpful)</td>
                </tr>
                <!-- Continue for each word/compound -->
            </tbody>
        </table>
    </section>
```

**Guidelines for Word-by-Word:**
- Include grammatical notes where helpful (e.g., "nominative plural", "vocative", "3rd person imperative")
- Group compound words (samasa) together when appropriate
- For long mantras, translate all key terms; minor particles (ca, vai, hi) can be grouped

### 4. Full Translations (REQUIRED: Both Languages)

```html
    <section class="translations">
        <h3>Translations</h3>
        <div class="translation english">
            <h4>English Translation</h4>
            <p>Clear, accessible English rendering of the complete mantra.</p>
        </div>
        <div class="translation kannada">
            <h4>ಕನ್ನಡ ಅನುವಾದ</h4>
            <p>ಸಂಪೂರ್ಣ ಮಂತ್ರದ ಕನ್ನಡ ಅನುವಾದ.</p>
        </div>
    </section>
```

### 5. Meaning (Simple + Deep) - REQUIRED

```html
    <section class="meaning">
        <h3>Meaning</h3>
        <div class="simple">
            <h4>Simple Meaning</h4>
            <p>
                Straightforward interpretation accessible to all readers.
                What does this mantra say in plain terms?
            </p>
        </div>
        <div class="deep">
            <h4>Deep Meaning</h4>
            <p>
                Philosophical, spiritual, and esoteric significance.
                What are the hidden layers of meaning?
                How does this connect to broader Vedantic concepts?
            </p>
        </div>
    </section>
```

### 6. Commentary

```html
    <section class="commentary">
        <h3>Commentary</h3>
        <p>
            Historical context, traditional interpretations,
            connection to other texts, and practical application.
        </p>
    </section>
</article>
```

---

## Complete Example

```html
<article class="mantra-entry">
    <header>
        <h2>गायत्री मन्त्र / Gayatri Mantra</h2>
        <p class="source"><strong>Source:</strong> Rig Veda, Mandala 3, Sukta 62, Verse 10</p>
        <p class="description">The most sacred mantra of the Vedas, a prayer to the divine light of consciousness</p>
    </header>

    <section class="mantra-text">
        <h3>Mantra Text</h3>
        <div class="script kannada">
            <h4>ಕನ್ನಡ</h4>
            ಓಂ ಭೂರ್ಭುವಃ ಸ್ವಃ<br>
            ತತ್ಸವಿತುರ್ವರೇಣ್ಯಂ<br>
            ಭರ್ಗೋ ದೇವಸ್ಯ ಧೀಮಹಿ<br>
            ಧಿಯೋ ಯೋ ನಃ ಪ್ರಚೋದಯಾತ್
        </div>
        <div class="script devanagari">
            <h4>देवनागरी</h4>
            ॐ भूर्भुवः स्वः<br>
            तत्सवितुर्वरेण्यं<br>
            भर्गो देवस्य धीमहि<br>
            धियो यो नः प्रचोदयात्
        </div>
        <div class="script transliteration">
            <h4>IAST Transliteration</h4>
            Oṃ bhūr bhuvaḥ svaḥ<br>
            Tat savitur vareṇyaṃ<br>
            Bhargo devasya dhīmahi<br>
            Dhiyo yo naḥ pracodayāt
        </div>
    </section>

    <section class="word-analysis">
        <h3>Word-by-Word Analysis</h3>
        <table class="analysis-table">
            <thead>
                <tr>
                    <th>Sanskrit (देवनागरी)</th>
                    <th>Transliteration</th>
                    <th>English Meaning</th>
                </tr>
            </thead>
            <tbody>
                <tr><td>ॐ</td><td>Oṃ</td><td>The primordial sound, representing the divine</td></tr>
                <tr><td>भूः</td><td>Bhūḥ</td><td>Earth, the physical plane</td></tr>
                <tr><td>भुवः</td><td>Bhuvaḥ</td><td>Atmosphere, the mental plane</td></tr>
                <tr><td>स्वः</td><td>Svaḥ</td><td>Heaven, the spiritual plane</td></tr>
                <tr><td>तत्</td><td>Tat</td><td>That (referring to the Divine)</td></tr>
                <tr><td>सवितुः</td><td>Savituḥ</td><td>Of Savitr/the Sun (genitive)</td></tr>
                <tr><td>वरेण्यम्</td><td>Vareṇyam</td><td>Most excellent, worthy of worship</td></tr>
                <tr><td>भर्गः</td><td>Bhargaḥ</td><td>Radiance, divine light, splendor</td></tr>
                <tr><td>देवस्य</td><td>Devasya</td><td>Of the divine being (genitive)</td></tr>
                <tr><td>धीमहि</td><td>Dhīmahi</td><td>We meditate upon (1st person plural)</td></tr>
                <tr><td>धियः</td><td>Dhiyaḥ</td><td>Intellects, understanding (accusative plural)</td></tr>
                <tr><td>यः</td><td>Yaḥ</td><td>Who (relative pronoun)</td></tr>
                <tr><td>नः</td><td>Naḥ</td><td>Our (genitive/accusative)</td></tr>
                <tr><td>प्रचोदयात्</td><td>Pracodayāt</td><td>May inspire, may illumine (3rd person optative)</td></tr>
            </tbody>
        </table>
    </section>

    <section class="translations">
        <h3>Translations</h3>
        <div class="translation english">
            <h4>English Translation</h4>
            <p>Om. We meditate upon the most excellent radiance of the divine Sun (Savitr). May that divine light illumine our intellects and inspire our understanding.</p>
        </div>
        <div class="translation kannada">
            <h4>ಕನ್ನಡ ಅನುವಾದ</h4>
            <p>ಓಂ. ಭೂಮಿ, ಅಂತರಿಕ್ಷ ಮತ್ತು ಸ್ವರ್ಗಲೋಕಗಳಲ್ಲಿ ವ್ಯಾಪಿಸಿರುವ ಆ ಸವಿತೃ ದೇವನ ಶ್ರೇಷ್ಠವಾದ ತೇಜಸ್ಸನ್ನು ನಾವು ಧ್ಯಾನಿಸುತ್ತೇವೆ. ಆ ದೈವಿಕ ಬೆಳಕು ನಮ್ಮ ಬುದ್ಧಿಯನ್ನು ಪ್ರೇರೇಪಿಸಲಿ.</p>
        </div>
    </section>

    <section class="meaning">
        <h3>Meaning</h3>
        <div class="simple">
            <h4>Simple Meaning</h4>
            <p>This is a prayer to the divine light of the Sun, asking for wisdom and clarity. The devotee meditates on the brilliant light that pervades all three worlds and asks for intellectual and spiritual guidance.</p>
        </div>
        <div class="deep">
            <h4>Deep Meaning</h4>
            <p>The Gayatri represents the journey from ignorance to enlightenment. Savitr is not merely the physical sun but the inner light of consciousness (Brahman) that illumines all existence. The three vyahrtis (bhur, bhuvah, svah) represent the gross, subtle, and causal bodies, indicating that this light pervades all levels of existence. "Dhimahi" suggests deep meditation, not mere intellectual understanding. The prayer is for the awakening of buddhi (discriminative wisdom) that allows one to perceive the Real beyond appearances.</p>
        </div>
    </section>

    <section class="commentary">
        <h3>Commentary</h3>
        <p>The Gayatri Mantra is considered the essence of all Vedic wisdom. Traditionally, it was revealed to Sage Vishwamitra and is chanted during the Sandhya Vandana (twilight prayers). The Chandogya Upanishad states that just as all leaves are held together by a stalk, all speech (Vedas) is held together by the Gayatri.</p>
    </section>
</article>
```

---

## CSS Classes Reference

| Class | Purpose |
|-------|---------|
| `.mantra-entry` | Container for complete mantra analysis |
| `.source` | Source reference styling |
| `.mantra-text` | Container for multi-language text |
| `.script.kannada` | Kannada script styling |
| `.script.devanagari` | Devanagari script styling |
| `.script.transliteration` | IAST transliteration styling |
| `.word-analysis` | Word-by-word section container |
| `.analysis-table` | Table styling for word breakdown |
| `.translations` | Translations section container |
| `.translation.english` | English translation block |
| `.translation.kannada` | Kannada translation block |
| `.meaning` | Meaning section container |
| `.meaning .simple` | Simple meaning block |
| `.meaning .deep` | Deep meaning block |
| `.commentary` | Commentary section |

---

## Checklist for Each Mantra

- [ ] Header with name in Sanskrit and English
- [ ] Source reference (Veda, Mandala, Sukta, Verse)
- [ ] Mantra text in Kannada script
- [ ] Mantra text in Devanagari script
- [ ] IAST transliteration
- [ ] Word-by-word analysis table (all significant words)
- [ ] English translation (complete)
- [ ] Kannada translation (complete)
- [ ] Simple meaning
- [ ] Deep meaning
- [ ] Commentary with context
