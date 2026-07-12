# ron-family-tree-private

StatiCrypt-encrypted, password-gated build of the **Tourangeau-Casey** family tree
(image-rich version: Ancestry/Newspapers record scans embedded in the person-cards).

Served via GitHub Pages; the HTML is **AES-encrypted at rest** (StatiCrypt v3.5.4,
PBKDF2 600k → AES-CBC), so a crawler sees only an encrypted blob + a password box.
`robots.txt` + a `noindex` meta keep it out of search indexes.

**Do not edit `index.html` by hand.** Regenerate it from the private research repo
`jitousig/ron-family-tree`:  `tree-build/_make-image-preview.py` → StatiCrypt encrypt
→ `tree-build/_deploy-private.js`.
