+++
author = "Ted Chen"
date = '2025-08-13'
draft = false
title = "Full Walkthrough: Bear Theme Syntax Guide"
description = "A comprehensive guide showcasing Markdown syntax and theme features including basic elements, code blocks, tables, and audio player functionality."
tags = ['hugo', 'markdown', 'syntax', 'theme', 'guide']
audio = ["/audio/sample.aac"]
+++

This comprehensive guide demonstrates the full range of Markdown syntax and theme features available in this Hugo blog theme. It showcases how basic HTML elements are styled and introduces special features like the audio player.

<!--more-->

## Text Formatting & Headings

The following sections demonstrate the six levels of section headings available. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Paragraphs & Text Flow

Standard paragraph text flows naturally within the theme. Here's an example with Lorem Ipsum-style content:

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Blockquotes & Citations

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

#### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables & Data Display

Tables aren't part of the core Markdown spec, but Hugo supports them out-of-the-box. Here are examples of different table formatting options:

   Name | Age
--------|------
    Bob | 27
  Alice | 23

#### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

## Code Blocks & Syntax Highlighting

This theme supports multiple ways to display code, each with its own styling and use cases.

#### Code block with backticks

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## Lists & Organization

Different list types help organize content hierarchically and provide clear structure for information.

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## Special HTML Elements

The theme properly styles various HTML elements for enhanced typography and user experience.

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>Command + Shift + D</kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

## Audio Player Features

This theme includes a custom audio player that integrates seamlessly with blog posts. The audio player features:

- Play/pause button with hover effects
- Progress bar that matches the theme colors
- Current time display
- Volume control and mute button
- Keyboard accessibility
- Responsive design that works on all devices

### How to Add Audio to Posts

To include an audio player in any blog post, simply add the `audio` parameter to your front matter:

```toml
title = "My Blog Post"
audio = "/audio/my-audio-file.aac"
```

The audio player supports common audio formats:
- AAC (.aac)
- MP3 (.mp3)
- WAV (.wav)

### Audio Player Styling

The audio player automatically adapts to the theme's color scheme, including dark mode support. It uses the same design language as the rest of the blog for a cohesive experience.

The player is positioned right after the post metadata (author, read time, date) and before the main content, making it easily discoverable for readers who want to listen to the audio version of your post.

This guide demonstrates how the theme handles various content types and provides a reference for creating rich, well-formatted blog posts with both visual and audio elements.
