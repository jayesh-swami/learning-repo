# Course-Specific Schema

In addition to the [common fields](../schema.md), courses use the following fields.

| Field | Type | Description |
| :--- | :--- | :--- |
| `context` | `object` | The academic and professional context of the learning. |
| ↳ `type` | `string` | Learning mode: `self-study`, `university`, `summer-school`, etc. |
| ↳ `institution` | `string` \| `null` | The institution or platform providing the study. |
| ↳ `program` | `string` \| `null` | The specific degree or program name (if applicable). |
| ↳ `credential_earned` | `boolean` | `true` if a certificate or degree was obtained. |
| ↳ `related_papers` | `array[string]` | List of academic papers read or planned to read during this course. |
