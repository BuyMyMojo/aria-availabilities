# aria-availabilities

A static page of aria's free/busy, and the days she can travel.

- `index.html` is **generated**. Editing it here is pointless — it is overwritten on the next build.
- Days are cut in **Australia/Melbourne**, because "a free Monday" is a fact about her week, not the reader's.
  Rendering the same instants in the viewer's clock would slide a Monday into a Sunday somewhere else.
- **Busy means her calendar marks it busy** (`TRANSP:OPAQUE`). An event marked *free* is not a claim on her
  time and does not make a day unavailable. Cancelled events never count.
- **Travel days**: Mondays and Wednesdays with no busy event at all.
- No event titles, locations, attendees or descriptions ever reach this file. The generator reads start, end,
  all-day, transparency and status only — and it scans the finished HTML for every title in the window before
  writing, refusing to publish if one appears.

Generated: see the timestamp in the page footer.
