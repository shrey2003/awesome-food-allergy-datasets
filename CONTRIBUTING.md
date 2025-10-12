# Contributing to Awesome Food Allergy Datasets

Thank you for your interest in contributing to awesome-food-allergy-datasets! 🎉

This repository is a community-driven effort to promote and support the use of machine learning in food allergies research by centralizing a collection of relevant datasets.

## 📑 Table of Contents

- [Focus Areas](#focus-areas)
- [How to Contribute](#how-to-contribute)
- [Dataset Entry Requirements](#dataset-entry-requirements)
- [Key Points](#key-points)
- [Automated Workflows](#automated-workflows)
- [Submission Process](#submission-process)

---

## 🎯 Focus Areas

We currently focus on six main categories:

- 💊 **Drug & Immunotherapy Development**
- 🔬 **Computational Method Development**
- 🔄 **Cross-Reactivity Analysis**
- 🔍 **Allergen Identification & Prediction**
- 🏥 **Patient Management & Clinical Decision Support**
- 🍽️ **Food Product Development & Safety**

---

## 🚀 How to Contribute

Contribute datasets by adding them directly to the README.md in the proper format!

### Step 1: Fork and Clone
```bash
# Fork the repository on GitHub, then:
git clone https://github.com/<your-username>/awesome-food-allergy-datasets.git
cd awesome-food-allergy-datasets
```

### Step 2: Find the Right Category Section
In `README.md`, locate your target category and find the **manual entry marker**:

```markdown
<!-- CATEGORY_Your Category Name_START -->

[Existing datasets appear here]

<!-- TSV_END -->

👉 ADD YOUR DATASET HERE (after TSV_END marker)

<!-- CATEGORY_Your Category Name_END -->
```

**Important:** Always add your dataset **AFTER** the `<!-- TSV_END -->` marker!

### Step 3: Add Your Dataset
Follow this exact format:

```markdown
## Dataset Name

Brief description of what this dataset contains and its purpose.

**Task:** Task1, Task2, Task3 | **Data Type:** Molecular | **Availability:** 🟢 Open source | **Paper:** [Link](https://paper-url.com)

**Source:** https://dataset-url.com | **Contact:** optional-email@example.com

---
```

### Step 4: Commit and Push
```bash
git checkout -b add-my-dataset
git add README.md
git commit -m "Add: [Dataset Name] - brief description"
git push origin add-my-dataset
```

### Step 5: Create Pull Request
- Go to GitHub and create a Pull Request
- Our automation will:
  - ✅ Recalculate stats including your entry
  - ✅ Validate your entry format
  - ✅ Commit stats updates to your PR

---

## 📋 Dataset Entry Requirements

All datasets must include the following:

### Required Fields
- ✅ **Task** - What the dataset is used for
- ✅ **Data Type** - Type of data (Molecular, Clinical, Food, Omics, etc.)
- ✅ **Availability** - Access level with emoji:
  - `🟢 Open source`
  - `🟡 Gated`

### Conditional Fields
- ✅ **Source** - Required for Open Source datasets, optional for Gated datasets

### Optional Fields
- **Paper** - Link to associated publication
- **Contact** - Contact information (especially useful for gated datasets)

### Example (Correct Format)
```markdown
## AllergenDB

A comprehensive database of allergenic proteins with structural annotations.

**Task:** Allergen Identification, Structural Analysis | **Data Type:** Molecular | **Availability:** 🟢 Open source | **Paper:** [Link](https://example.com/paper)

**Source:** https://allergendb.org

---
```

---

## 🔑 Key Points

- ⚠️ **Never delete or modify HTML comment markers** (<!-- --> tags)
- ✅ Content between `STATS_START/END` markers is auto-updated
- ✅ Add new datasets **after** the `<!-- TSV_END -->` marker
- ✅ Stats are automatically recalculated from all datasets

---

## 🤖 Automated Workflows

When you submit a PR, workflows run automatically:

### 1. Auto-Update README Workflow
**Triggers:** Changes to `README.md`

**Actions:**
- Recalculates stats from complete README
- Commits changes back to your PR branch

### 2. Validation Workflow
**Triggers:** Changes to `README.md`

**Actions:**
- Validates all dataset entries (required fields)
- Posts PR comment with validation results
- Flags missing or incorrect fields

**Note:** Both workflows run independently. You'll see stats updates AND validation comments.

---

## 📝 Submission Process

### Step-by-Step

1. **Fork** the repository
2. **Find** the correct category in README.md
3. **Add** your dataset after `<!-- TSV_END -->` marker
4. **Commit** with a clear message:
   ```
   Add: [Dataset Name] - brief description
   ```
5. **Push** to your fork
6. **Create** a Pull Request with:
   - Clear title
   - Description of what you added
   - Links to dataset/paper (if available)

### What Happens Next

1. ✅ Automation runs (stats update + validation)
2. 👀 Maintainers review your PR
3. 💬 Discussion/feedback if needed
4. ✅ PR gets merged
5. 🎉 Your contribution is live!

### Commit Message Guidelines

**Good examples:**
```
Add: SDAP 2.0 dataset to Drug Design category
Update: AllergenDB availability status to gated
Fix: Broken link for Food Allergy Dataset
```

**Format:**
- `Add:` - New dataset
- `Update:` - Modify existing dataset
- `Fix:` - Correct errors
- `Remove:` - Delete dataset

---

## ❓ FAQ

**Q: Can I add datasets to multiple categories?**
A: Choose the primary category. If truly cross-category, pick the most relevant one.

**Q: What if my dataset doesn't fit any category?**
A: Open an issue to discuss adding a new category.

**Q: Where exactly should I add my dataset in the README?**
A: Always add after the `<!-- TSV_END -->` marker in your chosen category section.

**Q: My PR has merge conflicts, what do I do?**
A: Pull the latest changes from main and resolve conflicts:
```bash
git fetch upstream
git merge upstream/main
# Resolve conflicts
git commit
git push
```

**Q: The validation failed, what should I do?**
A: Check the PR comment for details. Common issues:
- Missing required fields (Task, Data Type, Availability)
- Missing Source for open source datasets
- Incorrect availability emoji
- Malformed markdown syntax

**Q: Can I add datasets without a Source link?**
A: Only if it's a Gated dataset. Open source datasets must include a Source link.

---

## 🤝 Code of Conduct

- Be respectful and constructive
- Follow the dataset entry format
- Provide accurate information
- Cite sources properly
- Respect licensing and access restrictions

---

## 📧 Need Help?

- 💬 Open an [Issue](https://github.com/AI-For-Food-Allergies/awesome-food-allergy-datasets/issues)
- 📖 Check existing PRs for examples
- 📧 Contact maintainers

---

**Thank you for contributing to food allergy research!** 🥜💙
