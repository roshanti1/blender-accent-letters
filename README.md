# Accent Letters for Blender

A Blender 4.2+ extension. Adds an **Accent Letters** tab to the 3D viewport sidebar (press
<kbd>N</kbd>) holding the accented letters of 55 languages, plus a **Remove accents** operator for the
selected text objects.

## What it does

**Insert** — search by the letter, its Unicode name, the accent mark, a language or a code point, so
`two dots`, `spanish`, `00e9` and `é` all find **é**. Click it and:

- **in Edit Mode**, the letter goes in **at the text cursor** — `bpy.ops.font.text_insert()`, the same
  call Blender makes when you type;
- **out of Edit Mode**, there is no cursor, so it is appended to the object's text and the panel says
  so rather than pretending otherwise.

**Remove accents** rewrites the selected text objects: *Crème brûlée* becomes *Creme brulee*. The
letters Unicode does not decompose — `ø ł đ ß æ œ þ` and Turkish dotless `ı` — are converted too, with
options for those and for German-style `ä → ae`.

## Installing

Download `accent_letters-1.0.1.zip` from [Releases](https://github.com/roshanti1/blender-accent-letters/releases),
then in Blender: **Edit ▸ Preferences ▸ Add-ons ▸ Install from Disk**. Needs Blender **4.2 or newer**.

## Reporting a problem

[Open an issue](https://github.com/roshanti1/blender-accent-letters/issues/new/choose). Say which
Blender version and operating system you are on, what you did, and what happened instead — a
screenshot of the sidebar helps.

## Privacy

The add-on makes no network request and reads nothing outside its own folder. It requests no
permissions and collects nothing.

## Licence

GPL-3.0-or-later — see [LICENSE](LICENSE). The Blender Extensions Platform requires it of every
add-on, because Blender is GPL and treats an add-on as a derivative work.

More tools for typing accents on every device: <https://accentletters.wiki>
