# Editing Guide — Genesis Academic Site

## 1. Main file

Edit this file:

```text
index.html
```

## 2. Make the picture smaller or larger

In `index.html`, search for:

```css
--photo-size: 310px;
```

Change only the number.

Examples:

```css
--photo-size: 260px;
```

smaller picture

```css
--photo-size: 340px;
```

larger picture

## 3. Replace the photo

The current photo is:

```text
assets/profile.jpg
```

To replace it:

1. Upload a new photo into the `assets` folder.
2. Rename the new photo exactly:

```text
profile.jpg
```

Do not change the code if the file name is the same.

## 4. Change the main description

Search for:

```html
<p class="intro">
```

Edit the text inside that paragraph.

## 5. Change research cards

Search for:

```html
Current research
Highlights
Interests
```

Edit the text below each title.

## 6. Add or edit experience

Search for:

```html
<section id="experience">
```

Each experience item has this structure:

```html
<article class="timeline-item">
  <div class="date">Present</div>
  <div>
    <div class="role">PhD Research Student</div>
    <div class="place">University of Antwerp</div>
    <p class="description">
      Description here.
    </p>
  </div>
</article>
```

Copy and paste that block to add another experience.

## 7. Publications

The publications section is removed.

When you have publications, add a new section where this comment appears:

```html
<!-- Publications section intentionally removed for now. -->
```

## 8. Remove Teaching or Awards

To remove Teaching:

1. Delete this menu link:

```html
<a href="#teaching">Teaching</a>
```

2. Delete the full section that starts with:

```html
<section id="teaching">
```

To remove Awards, do the same with:

```html
<a href="#awards">Awards</a>
<section id="awards">
```

## 9. Change colors

Search for:

```css
:root {
```

The most important values are:

```css
--background: #f8f8f6;
--text: #111111;
--muted: #666666;
```

For blacker text, keep:

```css
--text: #111111;
```

## 10. Avoid breaking the page

Be careful not to delete:

```text
< > / " = ; { }
```

Most errors come from deleting one of those symbols.
