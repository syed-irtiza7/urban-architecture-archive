# 🌆 Urban Architecture Archive  
### A Digital Curation Project by **Syed Irtiza**  
INFO 4730 – Digital Curation & Preservation  

Welcome to the **Urban Architecture Archive**, a digital collection created to preserve and share essential information about five significant works of mid-century modern architecture. This site is designed for students, researchers, architects, and anyone who wants to explore how modernist design shaped the built environment. Every item includes descriptive documentation, curated metadata, and clear organization to support learning and long-term accessibility.

---

# 🔎 Site Search

Type to search for any architect, building name, year, or keyword.

<input type="text" id="searchBox" placeholder="Search the archive…" style="width:100%; padding:8px; font-size:14px; margin-bottom:15px;">

<ul id="searchResults"></ul>

<script>
const pages = [
  { name: "Case Study House No. 22 (Stahl House)", link: "items/case_study_house_22.md", keywords: "stahl pierre koenig 1960 los angeles modern" },
  { name: "Farnsworth House", link: "items/farnsworth_house.md", keywords: "farnsworth mies van der rohe 1951 illinois glass pavilion" },
  { name: "Eames House", link: "items/eames_house.md", keywords: "charles ray eames case study modular 1949 california" },
  { name: "Glass House", link: "items/glass_house.md", keywords: "philip johnson 1949 connecticut transparent pavilion" },
  { name: "Villa Savoye", link: "items/villa_savoye.md", keywords: "le corbusier international style 1931 france modernism" }
];

document.getElementById("searchBox").addEventListener("keyup", function() {
  let q = this.value.toLowerCase();
  let list = document.getElementById("searchResults");
  list.innerHTML = "";
  if (q.length < 2) return;

  let results = pages.filter(p => p.name.toLowerCase().includes(q) || p.keywords.includes(q));
  
  results.forEach(r => {
    let item = document.createElement("li");
    item.innerHTML = `<a href="${r.link}">${r.name}</a>`;
    list.appendChild(item);
  });
});
</script>

---

# 🧭 Navigation

This archive was created with user-friendly access in mind. Items are grouped clearly, metadata is linked directly, and users can browse in multiple ways:

### **Ways to Navigate**
- Use the **search bar** above to look for architects, dates, or buildings  
- Browse the building list below  
- Open metadata for detailed technical information  
- Use your browser’s built-in navigation to move between pages  

This structure supports students, architecture enthusiasts, and researchers who need quick, reliable access to curated information.

---

# 🏛️ Curated Buildings  
### *Five Works of Mid-Century Modern Architecture*

Each item includes a written description of the building’s background, design features, and historical importance.

---

## 1. **Case Study House No. 22 (Stahl House)**  
📄 [Description File](items/case_study_house_22.md)  
🗂️ [Metadata](metadata/metadata_case_study_house_22.md)

---

## 2. **Farnsworth House**  
📄 [Description File](items/farnsworth_house.md)  
🗂️ [Metadata](metadata/metadata_farnsworth_house.md)

---

## 3. **Eames House (Case Study House No. 8)**  
📄 [Description File](items/eames_house.md)  
🗂️ [Metadata](metadata/metadata_eames_house.md)

---

## 4. **Glass House**  
📄 [Description File](items/glass_house.md)  
🗂️ [Metadata](metadata/metadata_glass_house.md)

---

## 5. **Villa Savoye**  
📄 [Description File](items/villa_savoye.md)  
🗂️ [Metadata](metadata/metadata_villa_savoye.md)

---

# 📁 Metadata Overview

Metadata helps ensure long-term preservation and discoverability.  
Each record includes:

- Item ID  
- Title  
- Architect/Creator  
- Date  
- Location  
- Description  
- Format & Type  
- Keywords  
- Provenance/Source  
- Rights & Use  
- Recommended Citation  

This structure supports preservation planning and academic reuse.

---

# ⚖️ Copyright & Rights Information

This archive avoids the use of copyrighted images that require permission.

- Only public-domain or openly licensed materials were used  
- Text descriptions were written by **Syed Irtiza**  
- Items are provided for **educational and non-commercial use**  
- Users should cite the creator and the archive when reusing material  
- Metadata includes recommended citations for each record  

This ensures compliance with the assignment’s requirement to avoid copyrighted material.

---

# 🧩 Usability Features

To support user needs, this website includes:

### ✔ Simple search functionality  
Allows users to locate items quickly by architect, building name, year, or keywords.

### ✔ Clear navigation structure  
Users can move easily between documentation, metadata, and categories.

### ✔ Predictable layout  
Each section is formatted consistently for readability.

### ✔ Web-friendly formats  
All files use formats that preserve well over time (Markdown, plain text, open standards).

These enhancements align with digital curation principles of accessibility, sustainability, and usability.

---

# 🗂️ Repository Structure
urban-architecture-archive/
│
├── items/ → Description files
├── metadata/ → Metadata records
├── images/ → Supporting images
└── index.md → Website homepage
