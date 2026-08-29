# Anki Card Template

A responsive Anki card template for learning vocabulary on desktop, iPhone,
and Android. It includes configurable speech, recorded MP3 audio, study
sequences, images, hints, themes, accents, and compact settings controls.

> Want to generate local MP3 audio and add it to cards automatically? Use the
> companion [Anki Voice Studio](https://github.com/RemyGremory/anki-voice-studio).

## Features

- Automatic speech for the front and back of a card.
- Choice of language, system voice, and speech speed for the word and
  translation.
- Optional recorded MP3 audio for the word, translation, and examples.
- Study mode with configurable cycles and audio sequences.
- Random Front/Back swapping for the next card.
- Show or hide hints, typed answers, details, comments, and images.
- A choice of dark/light theme and accent colours.
- Settings designed for both phones and Anki Desktop.

## Installation

Before changing a note type, make an Anki backup.

1. In Anki Desktop, open **Tools → Manage Note Types**.
2. Select the note type you want to use and click **Fields…**.
3. Create the fields below if they do not already exist. Their order is not
   important, but the names must match exactly:

   `Front`, `Back`, `Description`, `Example`, `verb`, `Comment`, `Image`,
   `AudioWord`, `AudioTranslation`, `AudioExample`

4. Click **Cards…**.
5. Copy the contents of `Front.html` into the **Front Template**.
6. Copy the contents of `Back.html` into the **Back Template**.
7. Copy the contents of `Styleng.css` into the **Styling** section.
8. Save, then use **Preview** to test a card.
9. Sync Anki after the template looks correct on the computer. The template
   will then appear on the phone as well.

## How to use the fields

| Field | Purpose |
| --- | --- |
| `Front` | Word or phrase to learn. |
| `Back` | Translation or answer. |
| `Description` | Explanation, transcription, or extra context. |
| `Example` | Example sentences. Separate lines are kept as separate lines. |
| `verb` | Optional verb forms. |
| `Comment` | Optional note or usage tip. |
| `Image` | An optional picture shown under the translation on the back and under the hint on the front. |
| `AudioWord` | Optional MP3 audio for the word. |
| `AudioTranslation` | Optional MP3 audio for the translation. |
| `AudioExample` | Optional MP3 audio for examples. |

To add an image, drag it into the `Image` field in Anki Desktop. Anki stores it
in its media collection and syncs it to mobile devices with the rest of the
collection.

## Settings

Open the gear button on a card to change its behaviour. The selected options
are saved locally on that device.

Main settings include:

- automatic speech and skipping text in parentheses;
- study mode, sequence, repeat count, and random swapping;
- hints, type-answer mode, details, comments, and image visibility;
- theme and accent colour;
- languages, voices, and speech speed;
- whether to prefer recorded MP3 audio when it is present.

## Recorded audio

The easiest way to create audio is with the companion
[Anki Voice Studio](https://github.com/RemyGremory/anki-voice-studio). It can
create a CSV with MP3 files for new cards or write audio directly to selected
existing cards. After that, sync Anki normally for iPhone or Android.

You can also add an MP3 file manually in Anki Desktop by dragging it into one
of the `Audio…` fields.

## Notes

- The template works without recorded MP3 files; it can use the device’s own
  speech voices instead.
- Some system voices are available only on a particular device. Downloaded iOS
  voices may not always be exposed to Anki’s browser engine, so recorded MP3
  audio is the most reliable way to get the same voice everywhere.
- The template does not include cards, images, personal audio, or voice data.

Created by Remy.
