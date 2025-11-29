# Active Staff Repository — Clark Hyundai

A lightweight, Git-ready repository to store and publish **active staff** data for Clark Hyundai. Includes:

* Normalized JSON under `data/`
* Simple static site under `web/` to browse/search staff
* Validation script under `scripts/`

> Address: **2955 US 93 South, Kalispell, MT 59901**

---

## Repo Structure

```
clark-hyundai-staff/
├─ README.md
├─ data/
│  ├─ staff.json
│  ├─ departments.json
│  └─ org.json
├─ scripts/
│  └─ validate.mjs
└─ web/
   └─ index.html
```

---

## README.md

```markdown
# Clark Hyundai — Active Staff

This repository contains the **active staff directory** for Clark Hyundai. Data lives in `data/` and a simple static UI exists in `web/` for quick browsing.

## Quick Start

- View locally: open `web/index.html` in a browser (or serve with any static server).
- Validate data: `node scripts/validate.mjs`

## Files

- `data/staff.json` — canonical staff list (source of truth)
- `data/departments.json` — department registry (names + IDs)
- `data/org.json` — organization metadata (location, name)
- `web/index.html` — simple searchable directory
- `scripts/validate.mjs` — schema & referential checks

## Updating

1. Edit `data/staff.json`.
2. Run `node scripts/validate.mjs`.
3. Commit changes.

```

---

## data/departments.json

```json
[
  { "id": "ID_ccae9c", "name": "Management" },
  { "id": "ID_038374", "name": "Finance" },
  { "id": "ID_ef4f64", "name": "Sales" },
  { "id": "ID_521a50", "name": "Inventory" },
  { "id": "ID_c2ba20", "name": "Service" },
  { "id": "ID_afb5b2", "name": "Parts" },
  { "id": "ID_dd7c17", "name": "Office" },
  { "id": "ID_reception", "name": "Reception" }
]
```

---

## data/org.json

```json
{
  "org_id": "clark-hyundai",
  "name": "Clark Hyundai",
  "address": {
    "line1": "2955 US 93 South",
    "city": "Kalispell",
    "state": "MT",
    "postal_code": "59901",
    "country": "US"
  },
  "last_updated": "2025-11-29"
}
```

---

## data/staff.json

> Note: `title_original` preserves source text; `title` is a lightly normalized version (spelling/casing).

```json
[
  {
    "staff_id": "babak-mohammadi",
    "name": "Babak Mohammadi",
    "title": "General Manager",
    "title_original": "Genaral Manager",
    "department": "Management",
    "department_id": "ID_ccae9c",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "joshua-brandenburg",
    "name": "Joshua Brandenburg",
    "title": "General Sales Manager",
    "title_original": "General Sales Manager",
    "department": "Management",
    "department_id": "ID_ccae9c",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "brian-cook",
    "name": "Brian Cook",
    "title": "Finance Manager",
    "title_original": "Finance Manager",
    "department": "Finance",
    "department_id": "ID_038374",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "ellie-brustkern",
    "name": "Ellie Brustkern",
    "title": "Finance Manager",
    "title_original": "Finance Manager",
    "department": "Finance",
    "department_id": "ID_038374",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "veronica-nekrassoff",
    "name": "Veronica Nekrassoff",
    "title": "Sales Advisor",
    "title_original": "Sales Advisor",
    "department": "Sales",
    "department_id": "ID_ef4f64",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "brock-cross",
    "name": "Brock Cross",
    "title": "Sales Advisor",
    "title_original": "Sales Advisor",
    "department": "Sales",
    "department_id": "ID_ef4f64",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "eric-shirley",
    "name": "Eric Shirley",
    "title": "Sales Advisor",
    "title_original": "Sales Advisor",
    "department": "Sales",
    "department_id": "ID_ef4f64",
    "phone": "+1-406-740-6631",
    "display_phone": "(406) 740-6631",
    "status": "active"
  },
  {
    "staff_id": "parker-mcwhirter",
    "name": "Parker McWhirter",
    "title": "Sales Advisor",
    "title_original": "Sales Advisor",
    "department": "Sales",
    "department_id": "ID_ef4f64",
    "phone": "+1-406-505-7872",
    "display_phone": "(406) 505-7872",
    "status": "active"
  },
  {
    "staff_id": "brandon-ullom",
    "name": "Brandon Ullom",
    "title": "Sales Advisor",
    "title_original": "Sales Advisor",
    "department": "Sales",
    "department_id": "ID_ef4f64",
    "phone": "+1-406-780-5108",
    "display_phone": "(406) 780-5108",
    "status": "active"
  },
  {
    "staff_id": "john-squire",
    "name": "John Squire",
    "title": "Sales Advisor",
    "title_original": "Sales Advisor",
    "department": "Sales",
    "department_id": "ID_ef4f64",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "reception-unlisted",
    "name": "Reception",
    "title": "—",
    "title_original": "—",
    "department": "Reception",
    "department_id": "ID_reception",
    "phone": null,
    "display_phone": null,
    "status": "no-listings"
  },
  {
    "staff_id": "rob-vanderbeek",
    "name": "Rob Vanderbeek",
    "title": "Used Car Manager",
    "title_original": "Used car Manager",
    "department": "Inventory",
    "department_id": "ID_521a50",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "sarah-weed",
    "name": "Sarah Weed",
    "title": "Assistant Service Manager",
    "title_original": "Assistant Service Manager",
    "department": "Service",
    "department_id": "ID_c2ba20",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "lauren-bell",
    "name": "Lauren Bell",
    "title": "Service Adviser",
    "title_original": "Service Adviser",
    "department": "Service",
    "department_id": "ID_c2ba20",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "colton-schroeder",
    "name": "Colton Schroeder",
    "title": "Parts Advisor",
    "title_original": "Parts Advisor",
    "department": "Parts",
    "department_id": "ID_afb5b2",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "tyler-james-pace",
    "name": "Tyler James Pace",
    "title": "Controller",
    "title_original": "Controller",
    "department": "Office",
    "department_id": "ID_dd7c17",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "haliee-tipton",
    "name": "Haliee Tipton",
    "title": "Payroll & Benefits",
    "title_original": "Payroll & Benefits",
    "department": "Office",
    "department_id": "ID_dd7c17",
    "phone": null,
    "display_phone": null,
    "status": "active"
  },
  {
    "staff_id": "melinda-s-boggess",
    "name": "Melinda S. Boggess",
    "title": "Title Clerk",
    "title_original": "Title Clerk",
    "department": "Office",
    "department_id": "ID_dd7c17",
    "phone": null,
    "display_phone": null,
    "status": "active"
  }
]
```

---

## scripts/validate.mjs

Simple data checks: schema, department ID references, phone format.

```js
import fs from 'node:fs/promises';
import path from 'node:path';

const root = path.resolve(process.cwd(), 'data');
const load = p => fs.readFile(path.join(root, p), 'utf8').then(JSON.parse);

function die(msg){ console.error('\u274c', msg); process.exit(1); }
function ok(msg){ console.log('\u2705', msg); }

function isTel(s){ return s==null || /^\+1-\d{3}-\d{3}-\d{4}$/.test(s); }

const required = ['staff_id','name','title','department','department_id','status'];

const depts = await load('departments.json');
const deptIds = new Set(depts.map(d=>d.id));

const staff = await load('staff.json');

// Basic schema
for (const p of staff){
  for (const k of required){ if (!(k in p)) die(`Missing ${k} on ${p.name}`); }
  if (!deptIds.has(p.department_id)) die(`Unknown department_id ${p.department_id} on ${p.name}`);
  if (!isTel(p.phone)) die(`Bad phone format for ${p.name}: ${p.phone}`);
}

ok(`Validated ${staff.length} staff records.`);

// Duplicate IDs
const ids = new Set();
for (const p of staff){
  if (ids.has(p.staff_id)) die(`Duplicate staff_id: ${p.staff_id}`);
  ids.add(p.staff_id);
}
ok('No duplicate staff_id values.');

// Optional: warn on empty Reception listing
const hasReception = staff.some(s=>s.department==='Reception' && s.status==='active');
if (!hasReception) console.warn('\u26A0\uFE0F', 'Reception has no active listings.');
```

---

## web/index.html

A tiny static directory with search + department filters. It fetches `../data/staff.json` & `../data/departments.json`.

```html
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1"/>
<title>Clark Hyundai — Staff Directory</title>
<style>
  :root{ --bg:#0b1220; --panel:#101926; --text:#f8fafc; --muted:#93a4b8; --accent:#38bdf8; --border:#203045; }
  *{ box-sizing:border-box }
  body{ margin:0; background:var(--bg); color:var(--text); font:15px/1.5 system-ui,-apple-system,Segoe UI,Roboto }
  .wrap{ max-width:1100px; margin:24px auto; padding:0 16px }
  h1{ margin:0 0 8px; font-size:22px }
  .muted{ color:var(--muted) }
  .row{ display:flex; flex-wrap:wrap; gap:12px }
  .filters{ background:var(--panel); border:1px solid var(--border); border-radius:12px; padding:12px; margin:12px 0 }
  input[type="search"], .pill{ background:#0e1726; color:var(--text); border:1px solid var(--border); border-radius:8px; padding:10px }
  .grid{ display:grid; grid-template-columns: repeat(auto-fill, minmax(260px,1fr)); gap:12px }
  .card{ background:var(--panel); border:1px solid var(--border); border-radius:12px; padding:12px }
  .name{ font-weight:600; margin:0 0 2px }
  .title{ font-size:13px; color:var(--muted); margin-bottom:6px }
  a.tel{ color:var(--accent); text-decoration:none; font-size:13px }
  .dept{ font-size:12px; color:var(--muted) }
  .badge{ display:inline-block; padding:2px 8px; border-radius:999px; background:rgba(56,189,248,.15); color:var(--accent); border:1px solid var(--border); font-size:12px }
  label{ font-size:13px; display:inline-flex; align-items:center; gap:6px; margin:4px 8px 4px 0 }
  .footer{ margin:18px 0; font-size:12px; color:var(--muted) }
</style>
</head>
<body>
<div class="wrap">
  <h1>Clark Hyundai — Staff Directory</h1>
  <div class="muted">2955 US 93 South • Kalispell, MT 59901</div>

  <div class="filters">
    <div class="row">
      <input id="q" type="search" placeholder="Search name or title…" style="flex:1 1 260px"/>
      <span class="badge" id="count">0 staff</span>
    </div>
    <div id="deptFilters" style="margin-top:8px"></div>
  </div>

  <div id="grid" class="grid"></div>
  <div class="footer muted">Data source: <code>data/staff.json</code>. Last updated <span id="stamp"></span>.</div>
</div>
<script>
const $ = s => document.querySelector(s);
const grid = $('#grid');
const q = $('#q');
const count = $('#count');
const deptFilters = $('#deptFilters');

let STAFF=[], DEPTS=[];

async function load(){
  const [staff,depts] = await Promise.all([
    fetch('../data/staff.json').then(r=>r.json()),
    fetch('../data/departments.json').then(r=>r.json())
  ]);
  STAFF = staff.filter(p=>p.status==='active');
  DEPTS = depts;
  renderFilters();
  render();
  const d = new Date(); $('#stamp').textContent = d.toISOString().slice(0,10);
}

function renderFilters(){
  deptFilters.innerHTML = DEPTS.map(d=>
    `<label><input type="checkbox" value="${d.name}" checked> ${d.name}</label>`
  ).join('');
  deptFilters.addEventListener('change', render);
}

function activeDepartments(){
  return Array.from(deptFilters.querySelectorAll('input[type="checkbox"]'))
    .filter(x=>x.checked).map(x=>x.value);
}

function render(){
  const depts = new Set(activeDepartments());
  const term = q.value.trim().toLowerCase();
  let rows = STAFF.filter(p=> depts.has(p.department));
  if (term){
    rows = rows.filter(p=> p.name.toLowerCase().includes(term) || p.title.toLowerCase().includes(term));
  }
  count.textContent = `${rows.length} staff`;
  grid.innerHTML = rows.map(p=> card(p)).join('');
}

function card(p){
  const tel = p.display_phone ? `<a class="tel" href="tel:${(p.display_phone||'').replace(/[^\d]/g,'')}">${p.display_phone}</a>` : '';
  return `<div class="card">
    <div class="name">${p.name}</div>
    <div class="title">${p.title}</div>
    <div class="dept">${p.department}</div>
    ${tel}
  </div>`;
}

q.addEventListener('input', render);
load();
</script>
</body>
</html>
```

---

### Notes

* **Normalization**: Titles kept in `title_original`, normalized to `title` for display/spelling (e.g., “Genaral Manager” → “General Manager”).
* **Phones**: Stored as both `display_phone` (human-friendly) and `phone` (`+1-AAA-BBB-CCCC`).
* **Reception**: Included as a placeholder with status `no-listings` so the UI can remain consistent until listings exist.
* **Extensibility**: Add `email`, `photo_url`, or `start_date` fields later without breaking the UI.
# team
