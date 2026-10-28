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

The MATH 1070 page lists slides and homework in a topic table (`<table class="resource-table">`, one row per
topic, light-green "Week N" rows from `<tr class="week-row">`). The same CSS classes are described under
"Instructor Resources" below; reuse them for new course pages.

The URL to put on a syllabus is `dionmann.github.io/courses/<folder>/`.

`math1070.html` in the top folder is only a redirect: the Summer 2026 syllabus and slides
point to `dionmann.github.io/math1070`, so keep that file.

## Instructor Resources

The "Instructor Resources" tab (`resources.html`) collects course materials for other instructors,
organized by course (not by semester):

```
resources.html          <- hub page: one "course-card" per course + license / request policy
resources/
  math1070/
    index.html          <- topic-by-topic table (Topic | Text § | Slides | Homework | Worksheet)
    notes/  slides/  homework/  worksheets/
  math1131/             <- same layout ("In progress"; table is a commented-out template)
  math1020/             <- same layout ("Coming soon")
```

Rules:

- **Don't copy files that are already on a course page.** Link them in place, e.g.
  `../../courses/2026-summer-math1070/materials/Su2026_Topic3.pdf`.
- **Anything new** (lecture notes, worksheets, activities, slides never posted to students) goes in
  the matching subfolder of `resources/<course>/`, named `<course>_<type><NN>.pdf`,
  e.g. `resources/math1070/worksheets/math1070_worksheet05.pdf`.
- In a course table, an empty cell is `<td class="empty">&mdash;</td>`; replace it with
  `<td><a href="worksheets/math1070_worksheet05.pdf" target="_blank">Worksheet</a></td>`.
- **Do not post** quizzes, exams, or answer keys here. The pages say they are available by email.
- When a course gets its first materials, change its label on `resources.html` from
  `<span class="status soon">Coming soon</span>` to `<span class="status">Available</span>`
  and update the "Posted:" line on its card.

### Adding a course to Instructor Resources

1. Copy `resources/math1131/` to `resources/<course>/` and edit the new `index.html`.
2. In `resources.html`, copy a `course-card` block and point it to `resources/<course>/index.html`.
