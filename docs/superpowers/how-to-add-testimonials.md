# Adding Testimonials

Once you have real client testimonials, follow these steps to add them to the website.

## 1. Locate the right section

In both language files:

- `content/en/_index.md` — between the CTA section and the FAQ block
- `content/pt/_index.md` — same position

The testimonials block slot is reserved. Add it back with this structure:

```yaml
  - block: testimonials
    content:
      title: What Our Clients Say     # section heading
      subtitle: ""                    # optional subtitle below title
      items:
        - name: "Client Name"
          role: "Company / Position"
          text: "The testimonial text goes here. Keep it genuine and specific about the value delivered."
      # Optional: add a photo
      # avatar_asset: "media/testimonials/client-photo.jpg"
    design:
      spacing:
        padding: ["6rem", 0, "4rem", 0]
```

## 2. For each testimonial

| Field   | What to put                                              |
|---------|----------------------------------------------------------|
| `name`  | The person's full name (e.g. `"Maria Silva"`)            |
| `role`  | Company name or role (e.g. `"CEO, TechStart"`)           |
| `text`  | The testimonial quote. Use `<b>bold</b>` for emphasis if needed. |

### Optional: Add a photo

1. Place the photo in `assets/media/testimonials/` (e.g., `client-photo.jpg`)
2. Add `avatar_asset` to the testimonial item:
   ```yaml
   - name: "Maria Silva"
     avatar_asset: "media/testimonials/maria-silva.jpg"
     role: "CEO, TechStart"
     text: "Little Development delivered beyond our expectations..."
   ```

3. For dark/light mode photos, use a path like `media/testimonials/maria-silva-light.jpg` and `media/testimonials/maria-silva-dark.jpg`.

## 3. Multiple testimonials

Add more items under the `items:` list:

```yaml
items:
  - name: "First Client"
    role: "Company A"
    text: "Amazing work!"
  - name: "Second Client"
    role: "Company B"
    text: "Professional and on-time."
```

The component handles carousel/slider navigation automatically when there are multiple items.

## 4. Translation

Keep both language files in sync — add the same testimonials to PT with translated quotes:

```yaml
# content/pt/_index.md
items:
  - name: "Primeiro Cliente"
    role: "Empresa A"
    text: "Trabalho incrível!"
```

## Tips

- **Be honest** — only use real, authorized testimonials
- **Be specific** — concrete results ("increased sales by 30%") are more compelling than generic praise
- **Keep it concise** — 2-4 sentences per testimonial is ideal
- **Mix roles** — CEOs, CTOs, and project managers add different perspectives
- **Photo consent** — only add photos with explicit permission
- **Vary industries** — show breadth of expertise if applicable
