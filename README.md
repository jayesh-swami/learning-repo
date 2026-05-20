# learning-repo
Repository to store all my notes, resources etc. As an ambition to best keep track of my learning, each course directory contains a `course_metadata.yaml` file that serves as the single source of truth for the course's progress, context, and academic connections. The format is as follows - 

### **Schema Definition**

| Field | Type | Description |
| :--- | :--- | :--- |
| `name` | `string` | The full, official name of the course. |
| `status` | `string` | Current state: `in-progress`, `completed`, or `paused`. |
| `start_date` | `date` | The date study commenced (`YYYY-MM-DD`). |
| `end_date` | `date` \| `null` | The date study concluded (`YYYY-MM-DD`) or `null` if ongoing. |
| `last_revision_date` | `date` | The last time I did a revision of this course (`YYYY-MM-DD`). |
| `labels` | `array[string]` | Tags for categorization (e.g., `mathematics`, `machine-learning`). |
| `links` | `array[object]` | A collection of resource links. |
| ↳ `type` | `string` | The source type (e.g., `youtube`, `mit_ocw`, `coursera`). |
| ↳ `url` | `string` \| `null` | The direct URL to the course or resource. |
| `context` | `object` | The academic and professional context of the learning. |
| ↳ `type` | `string` | Learning mode: `self-study`, `university`, `summer-school`, etc. |
| ↳ `institution` | `string` \| `null` | The institution or platform providing the course. |
| ↳ `program` | `string` \| `null` | The specific degree or program name (if applicable) the course is associated with. |
| ↳ `credential_earned`| `boolean` | `true` if a certificate or degree was obtained. |
| ↳ `related_papers` | `array[string]`| List of academic papers read or planned to read during this course. |
| `event_log` | `array[object]` | A chronological log of significant milestones. |
| ↳ `type` | `string` | Type of event: `creation`, `revision`, `resource_added`, `personal_notes`, or `completion`. |
| ↳ `date` | `date` | When the event occurred (`YYYY-MM-DD`). |
| ↳ `description` | `_string_` | A brief note describing the event or milestone. |
