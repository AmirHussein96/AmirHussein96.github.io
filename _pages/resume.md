---
layout: single
title: "Resume"
permalink: /resume/
author_profile: true
---

<!-- You can view my CV as a PDF:

<a href="{{ '/assets/cv.pdf' | relative_url }}" target="_blank">Download CV (PDF)</a> -->
<div id="cv-embed" class="cv-embed"></div>

<noscript>
  Your browser has JavaScript disabled.
  <a href="{{ '/assets/cv.pdf' | relative_url }}">Open the CV (PDF)</a>.
</noscript>

<link rel="preload" href="{{ '/assets/js/pdfobject.min.js' | relative_url }}" as="script">
<script src="{{ '/assets/js/pdfobject.min.js' | relative_url }}"></script>
<script>
  PDFObject.embed("{{ '/assets/cv.pdf' | relative_url }}", "#cv-embed", {
    pdfOpenParams: { view: "FitH", pagemode: "none" }
  });
</script>

<style>
  .cv-embed { height: calc(100vh - 220px); }
  @media (max-width: 768px) { .cv-embed { height: 75vh; } }
  .cv-embed object, .cv-embed iframe { width: 100%; height: 100%; border: 0; }
</style>