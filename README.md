# DionMann.github.io
Dion Mann Mathematics Webpage

## Course webpages

Each course offering gets its own folder under `courses/`, named `<year>-<term>-<course>`:

```
courses/
  2026-summer-math1070/
    index.html      <- course page  (dionmann.github.io/courses/2026-summer-math1070/)
    materials/      <- syllabus, homework, slides, schedule image
  2026-fall-math1131/
    index.html
    materials/
```

Course folders never move, so links to a course page keep working after the course ends.
When a semester ends, only `teaching.html` changes: move the course's line from
"Currently Teaching" to the top of "Previous Courses".

### Adding a new course

1. Copy the most recent course folder (e.g. `courses/2026-fall-math1131/`) and rename it,
   e.g. `courses/2027-spring-math1131/`. Delete the old files in its `materials/`.
2. Edit the new `index.html` (title, term, times, rooms, links). Inside `courses/<folder>/`,
   site pages are linked as `../../teaching.html` and the stylesheet as `../../style.css`.
3. In `teaching.html`, add the course under "Currently Teaching" with a link to
   `courses/<folder>/index.html`.

The URL to put on a syllabus is `dionmann.github.io/courses/<folder>/`.

`math1070.html` in the top folder is only a redirect: the Summer 2026 syllabus and slides
point to `dionmann.github.io/math1070`, so keep that file.
