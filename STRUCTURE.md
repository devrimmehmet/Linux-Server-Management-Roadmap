# Repository Structure and Naming Standards

## 1. Folder Naming
- Use **PascalCase** for main sections (e.g., `01-Basics`, `02-Docker`).
- Each main section contains:
  - `en/` folder → English content
  - `tr/` folder → Turkish content
  - `media/` folder → Related images and videos

## 2. File Naming
- Use **kebab-case** for file names (e.g., `docker-intro.md`, `ag-yonetimi.md`).
- File names in `en/` should be in English, in `tr/` should be in Turkish.
- Avoid spaces or special characters in file names.

## 3. Media Files
- Store all section-specific images/videos in the `media/` folder inside that section.
- Use descriptive kebab-case names for media (e.g., `docker-architecture.png`).

## 4. Language Files
- The main README should have two versions:
  - `README.md` → English
  - `README.tr.md` → Turkish
- Links between translations should be included at the top of each file.

## 5. Versioning
- Major content updates should be committed with clear commit messages:
  - Example: `docs(en): added docker compose guide`
  - Example: `docs(tr): güncellendi kubernetes giriş notları`

## 6. Contribution
- Any new content must be added to both `en/` and `tr/` when possible.
- Media should be optimized for web (compressed without losing quality).

---
