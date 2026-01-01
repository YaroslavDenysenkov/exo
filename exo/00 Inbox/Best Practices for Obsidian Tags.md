When organizing a technical knowledge base (especially one as dense as IT/DevOps), it is easy to fall into the "Tag Soup" trap—where you have hundreds of unorganized tags like `#git`, `#github`, `#version-control`, `#coding`.

Here are the best practices for tagging in Obsidian, specifically tailored for an IT context.

### 1. The Golden Rule: Links for Topics, Tags for Status

The most common mistake is using tags for _everything_. In Obsidian, **Links (`[[ ]]`) are stronger than Tags (`#`).**

- **Use Links for Nouns (Topics):** `[[Jenkins]]`, `[[AWS]]`, `[[Git]]`.
    
    - _Why?_ You can click `[[Jenkins]]` to see a "hub" of all notes related to it. You can write a summary on that page. You cannot write on a tag.
        
- **Use Tags for Adjectives (Status/Type):** `#status/reading`, `#type/reference`, `#source/book`.
    
    - _Why?_ Tags are best for filtering _across_ different topics (e.g., finding all "Cheatsheets" whether they are for Python or AWS).
        

### 2. Use Nested (Hierarchical) Tags

IT topics have natural hierarchies. Obsidian supports nested tags using the forward slash `/`. This keeps your tag pane clean and allows you to search broadly (`#devops`) or narrowly (`#devops/aws`).

**Bad (Flat):** `#aws` `#azure` `#python` `#javascript` `#react` `#docker` `#k8s`

**Good (Nested):**

- `#lang/python`
    
- `#lang/js/react`
    
- `#cloud/aws/ec2`
    
- `#cloud/azure`
    
- `#tool/docker`
    
- `#tool/k8s`
    

**Why this works for IT:** When you are looking for "infrastructure" notes, you can just search `#cloud` or `#tool`. If you want specifically storage, you search `#cloud/aws/s3`.

### 3. The "IT Taxonomy" Proposal

Here is a battle-tested tag structure for a developer/sysadmin vault:

#### A. The "What" (Topic/Domain)

_Use these sparingly; prefer Links `[[ ]]` if possible, but if you must use tags:_

- `#topic/devops` (CI/CD, Jenkins, Docker)
    
- `#topic/cloud` (AWS, Azure)
    
- `#topic/security` (Auth, OAuth, SSH)
    
- `#topic/lang` (Python, Go, Rust)
    

#### B. The "Type" (Format of the note)

_This is the most useful category._

- `#type/cheatsheet` (Commands you always forget, e.g., Git LFS commands)
    
- `#type/troubleshooting` (Fixes for specific errors)
    
- `#type/concept` (Theory, Architecture patterns)
    
- `#type/snippet` (Copy-paste code blocks)
    
- `#type/meeting` (Notes from work syncs)
    

#### C. The "Status" (Workflow)

- `#status/wip` (Incomplete, needs review)
    
- `#status/toread` (Bookmarks or articles saved for later)
    
- `#status/archived` (Old tech stacks you don't use anymore)
    

### 4. Practical Example: A Note about "Git LFS"

Don't just tag it `#git` `#lfs`.

**Title:** `How to migrate a repo to Git LFS` **Tags:** `#topic/devops` `#type/cheatsheet` **Links:** `[[Git]]`, `[[Git LFS]]`

**Content:**

> Commands to migrate existing large files to `[[Git LFS]]`...

**Why this is better:**

1. If you want to find **all cheatsheets** (Git, AWS, Linux), you search `#type/cheatsheet`.
    
2. If you want to see **everything about Git**, you look at the backlinks for `[[Git]]`.
    

### 5. Tag Wrangler Plugin

If you are starting to organize your IT notes, install the **Tag Wrangler** plugin.

- **Feature:** It allows you to right-click a tag in the sidebar and **Rename** it.
    
- **Benefit:** You can merge `#aws` and `#amazon-web-services` into `#cloud/aws` instantly across 100 notes.
    

### Summary Checklist

1. **Lowercase only:** `#DevOps` and `#devops` are different tags. Stick to lowercase (`#devops`) to avoid duplicates.
    
2. **Kebab-case:** Use hyphens for spaces (`#software-architecture`, not `#softwarearchitecture` or `#software_architecture`).
    
3. **Limit your "Topic" tags:** If you find yourself tagging `#jenkins`, ask yourself: "Should this be a link to a `[[Jenkins]]` note instead?"