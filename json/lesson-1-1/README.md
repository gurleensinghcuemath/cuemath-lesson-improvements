# Lesson 1.1 — Place Value JSON Files

Course: `mk-foundations-grade-3-4`
Route: `/lesson/mk-foundations-grade-3-4/0/0`
Repo: `cuemath-academy-next`

## Files

| File | Slug | Status |
|------|------|--------|
| `lesson-1-1-place-value-v4.json` | `mk-f-place-value-v4` | Archived |
| `lesson-1-1-place-value-v5.json` | `mk-f-place-value-v5` | Archived |
| `lesson-1-1-place-value-v6.json` | `mk-f-place-value-v6` | **Live** |

## How to integrate into cuemath-academy-next

### 1. Copy JSON file

```
src/data/content/mk-foundations-grade-3-4/unit-1/lesson-1-1-place-value-v6.json
```

### 2. Register in `src/data/content/v2-loader.ts`

```typescript
import mkFoundationsLesson11v6 from "./mk-foundations-grade-3-4/unit-1/lesson-1-1-place-value-v6.json";

// In AUTHORED_LESSONS["mk-foundations-grade-3-4"]:
"mk-f-place-value-v6": mkFoundationsLesson11v6 as unknown as LessonV2,
```

### 3. Update `src/data/content/mk-foundations-grade-3-4/index.json`

In `units[0].lessons[0]`, set:
```json
"id": "mk-f-place-value-v6",
"slug": "mk-f-place-value-v6"
```

### 4. Run dev server

```bash
npm run dev
```

Open: http://localhost:3000/lesson/mk-foundations-grade-3-4/0/0

## Version history

| Version | Key changes |
|---------|-------------|
| v4 | First full authored lesson. CF×2, IL×11, WE×2, PL×8, MC×4, CE×1 |
| v5 | P4 replaced (place-value direction), MC4 replaced (zero-placeholder), 14 hint fixes |
| v6 | UI fixes: predict prompt, amber hint box, CF onWrong, WE1 vocabulary, `figuresInOptions` removed |
