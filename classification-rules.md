# 🔖 EnergizeOS File Classification Rules

These are the fixed rules used to automatically group files by category in the document portal:

| Category             | Keywords (must be present in file name, case-insensitive) |
|----------------------|------------------------------------------------------------|
| **Product Specs**      | `spec`, `datasheet`, `technical`                            |
| **Standard Contracts** | `contract`, `agreement`, `terms`, `msa`                    |
| **Product Images**     | `.png`, `.jpg`, `.jpeg`, `image`, `photo`, `picture`       |
| **Certifications**     | `cert`, `ul`, `iec`, `en`, `compliance`, `certificate`     |
| **Other Files**        | Default fallback when no keywords are matched              |

## 🛠 Notes

- All file names are matched in lowercase.
- Matching is done purely via file name substring, no need for structured prefixes.
- These rules are implemented in the `index.html` frontend JavaScript.

📁 If you want a file to appear under a specific category, just make sure its name includes the correct keyword.
