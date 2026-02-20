---
title: 'Dynamically Updating Zotero Collections in Overleaf'
date: 2025-05-24
permalink: /posts/2025/zotero_overleaf_integration/
tags:
  - Zotero
  - Overleaf
---

Zotero in Overleaf
======
Managing citations in projects, especially in collaborations, can be quite a headache. One way to attempt to address this is to use a citation managing service such as Zotero. In it, you can keep your references collected in specific folders; of particular use is making collections for each paper you are working on. Using plugins like Better BibLaTeX you can even export .bib files with journal abbreviations! However, when exporting references to use in LaTeX, you still need to make a .bib file and then copy the contents over to an Overleaf project. Some of the chore of this can be ameliorated by having Zotero automatically update your exported .bib file in the background, but you still need to copy-paste this content into Overleaf every time you add a new reference. 

There does exist functionality in Overleaf to link your Zotero account, but this requires you to do one of the following
- Create a .bib file that contains all of your Zotero references
- Create a references.bib file "on-the-fly" which contains each citation you want as you reference them

Both of these approaches have issues, however. The former requires you to re-generate a references.bib file of your entire Zotero library, while the latter requires a scan of your entire Zotero library that can in practice take a while. Both of these interrupt the writing flow. Perhaps more annoyingly, neither of these methods is able to generate .bib files which use journal abbreviations, a common best practice many journals either require or recommend for publication.

However, there is a workaround that lets you have your cake and eat it too. 

Import a Dynamically Updating .bib File Into Overleaf
======

Using an Overleaf third party supported cloud file service such as Dropbox, it is possible to save your Better BibLaTeX file to the cloud. Then, you can import this file into Overleaf as your references.bib file. Now, every time you add a reference to a particular Zotero collection within seconds you can refresh your Overleaf references file and have the latest version of your collection with journal abbreviations. This method even works with shared collections allowing collaborators to add to the .bib file as well. The file still needs to be refreshed as before, but since the collection is not being generated—only downloaded—and is much smaller, the process is much quicker. The only drawback I have encountered is that if you do not have your PC open to upload the updated local .bib file to the cloud, then collaborators who add to a shared collection will not see their new additions in the Overleaf. Compared to the usual pain of keeping track of references, though, I think this is a small price to pay.