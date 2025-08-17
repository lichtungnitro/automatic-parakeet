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
> **Note** that you can use _Markdown syntax_ within a blockquote.

#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables & Data Display

Tables aren't part of the core Markdown spec, but Hugo supports them out-of-the-box. Here are examples of different table formatting options:

| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |

#### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------- | -------- | ------ |
| _italics_ | **bold** | `code` |

## Code Blocks & Syntax Highlighting

This theme supports multiple ways to display code, each with its own styling and use cases.

#### Code block with backticks

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
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

- List item
- Another item
- And another item

#### Nested list

- Fruit
  - Apple
  - Orange
  - Banana
- Dairy
  - Milk
  - Cheese

## Special HTML Elements

The theme properly styles various HTML elements for enhanced typography and user experience.

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>Command + Shift + D</kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

## Images & Media

This section demonstrates how to add images to your blog posts using Markdown syntax.

#### Basic image with alt text

```markdown
![Sample Image](https://via.placeholder.com/400x200/4A90E2/FFFFFF?text=Sample+Image)
```

_What you'll see: A blue placeholder image with the text "Sample Image" displayed inline with your content._

#### Image with link

```markdown
![Clickable Image](https://via.placeholder.com/300x150/50C878/FFFFFF?text=Click+Me)](https://example.com)
```

![Clickable Image](https://www.shutterstock.com/shutterstock/photos/2477913981/display_1500/stock-vector-line-shape-marker-underline-arrow-heart-brush-element-set-hand-drawn-sketch-marker-underline-2477913981.jpg)
_What you'll see: A green placeholder image that acts as a clickable link to the specified URL._

#### Image with custom styling

```markdown
<img src="https://via.placeholder.com/350x200/E74C3C/FFFFFF?text=Styled+Image" 
     alt="Styled image with border" 
     style="border: 3px solid #2C3E50; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" />
```

<img src="https://www.shutterstock.com/shutterstock/photos/2477913981/display_1500/stock-vector-line-shape-marker-underline-arrow-heart-brush-element-set-hand-drawn-sketch-marker-underline-2477913981.jpg" 
     alt="Styled image with border" 
     style="border: 3px solid #2C3E50; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" />

_What you'll see: A red placeholder image with a dark border, rounded corners, and a subtle shadow effect._

#### Image with caption

```markdown
<figure>
  <img src="https://via.placeholder.com/450x250/9B59B6/FFFFFF?text=Figure+Caption" alt="Image with figure caption" />
  <figcaption><em>Figure: An image with proper semantic captioning</em></figcaption>
</figure>
```

<figure>
  <img src="https://www.shutterstock.com/shutterstock/photos/2477913981/display_1500/stock-vector-line-shape-marker-underline-arrow-heart-brush-element-set-hand-drawn-sketch-marker-underline-2477913981.jpg" alt="Image with figure caption" />
  <figcaption><em>Figure: Line shaped marker with underline, arrow and heart</em></figcaption>
</figure>

_What you'll see: A purple placeholder image wrapped in a semantic figure element with an italicized caption below it._

The last but not the least, examples above use placeholder images for demonstration. In your actual posts, replace the URLs with real image paths from your Hugo static directory (e.g., `/images/your-image.jpg`) or external sources with proper attribution.

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
