## Sarvajna Vachana Archives

In the 16th century Kannada speaking region in Southern India, a wave of rationalism and anti-caste philosophy started taking root. There were many eminent poets and composers whose work has been etched into the ethos of the Kannada society. Among them all, one wandering poet is reminisced more than others. He called himself "Sarvajna" (the all knowing) and his nuggets of wisdom were packaged into triplets following a certain metric rhythm. His empathy, rationalism, wit, and humour resonate to date in modern India.

Growing up, I was always fascinated by his triplets (or vachanas) and previously had tried archiving them with transliterations and translations. But it never came to fruition.

Now, with the help of recent AI models, I am embarking on a project of giving it another shot. I am first verifying the OCR'ed transcriptions of the vachanas from the authoritative book that was compiled based on extensive research work (Uttangi 1927), and use #LLMs to transliterate and translate while I do a final verification. This is an enjoyable hobby project that I hope to continue working on. There are more than 2000 vachanas in the book.

## Contribution

I have not really considered how to make this project open for collaborations. If you would like to contribute, raise a github issue. It could be to fix transliteration errors, or to provide alternative translations. I am primarily focused on using Uttangi 1927 as the source material. Perhaps, once this is done, I would like to look for other verified sources. 

## Language Model

I have tried using ChatGPT 5.2 and Gemini for the transliteration and translation tasks. After some basic playing around, a custom Gemini instance (gem) with a clear and detailed system instructions has been useful. And the _fast_ mode has proven to be better than the _thinking_ mode which has hallucinated more for this task.

### System instruction

This is the system instruction I have provided for the Gemini gem. 

```
You are helping with archiving sarvjna's tripadis. I will provide kannada text then you should make a json entry that follows structure like this:
{

    "id": 23,

    "theme": "invocation",

    "kannada": "ನಂದಿಯನು ಏರಿದನ ಚಂದಿರನ ಸೂಡಿಬದನ\nಕಂದನ ಬೇಡಿ ನಲಿದಾನು ನೆನೆವುತ್ತ\nಮುಂದಿ ಹೇಳುವೆನು ಸರ್ವಜ್ಞ",

    "transliteration": "Nandiyanu eeridana chandirana soodibadana\nkandana beedi nalidaanu nenevutta\nmundi heluvenu Sarvajna.",

    "translation": "Remembering the one who rides the bull Nandi, who wears the moon as an adornment, and who rejoiced when asked for a child, I shall henceforth recite, O Sarvajna."

  }

Abstract to one word theme. All transliterations should follow the Uppercase for Dheerga and Retroflex standard:

* Vowels: Upper case (A, I, U, E, O) represents Dheerga (long) sounds.
* Consonants: Upper case (T, D, N, L) represents Retroflex (hard) sounds.

Keep track of the ids and increment as we work through new vachanas. Respond to me in English.
```
