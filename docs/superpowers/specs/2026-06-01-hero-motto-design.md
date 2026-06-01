# Hero Motto — Design Spec

## Goal
Add a witty, presence-filled motto to the hero section that conveys: "you focus on what makes you great, leave the tech to Little Development."

## Approach
**Approach A** — motto goes in the `text` field, emphasized with `<b>` tags, followed by the existing description. The `text` field supports HTML via `dangerouslySetInnerHTML`, so bold text and line breaks work natively.

## Copy

### English
> **Make your business great, leave the little developments to us!**
>
> Technology and consultancy solutions to boost your business. We transform ideas into custom digital solutions.

### Portuguese
> **Faça seu negócio decolar, deixe os pequenos desenvolvimentos conosco!**
>
> Soluções em tecnologia e consultoria para impulsionar o seu negócio. Transformamos ideias em soluções digitais sob medida.

## Implementation
- Edit `content/en/_index.md` — hero block `text` field: motto (bold) + line break + existing description
- Edit `content/pt/_index.md` — same structure with Portuguese copy

## Files Affected
- `content/en/_index.md`
- `content/pt/_index.md`
