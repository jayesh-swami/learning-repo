# Common Schema

The following fields are shared across all resource types (`course`, `paper-reading`, `others`). Each directory may define additional fields in its own `schema.md`.

| Field | Type | Description |
| :--- | :--- | :--- |
| `name` | `string` | The full, official name of the course/paper-reading/others. |
| `type` | `string` | Type of the resource: `course`, `paper-reading`, or `others`. |
| `status` | `string` | Current state: `in-progress`, `completed`, or `paused`. |
| `end_date` | `date` \| `null` | The date study concluded (`YYYY-MM-DD`) or `null` if ongoing. |
| `last_revision_date` | `date` \| `null` | The last time I did a revision (`YYYY-MM-DD`) or `null` if never revised. |
| `labels` | `array[string]` | Tags for categorization (e.g., `mathematics`, `machine-learning`). |
| `links` | `array[object]` | A collection of resource links. |
| ↳ `type` | `string` | The source type (e.g., `youtube`, `mit_ocw`, `coursera`, `arxiv`). |
| ↳ `url` | `string` \| `null` | The direct URL to the resource. |
| `event_log` | `array[object]` | A chronological log of significant milestones. |
| ↳ `type` | `string` | Type of event: `start`, `revision`, `resource_added`, `personal_notes`, or `completion`. |
| ↳ `date` | `date` | When the event occurred (`YYYY-MM-DD`). |
| ↳ `description` | `string` | A brief note describing the event or milestone. |
