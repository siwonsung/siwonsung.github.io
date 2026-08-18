---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% assign cv_file = site.static_files | where: "path", "/files/Siwon_Sung_CV.pdf" | first %}

{% if cv_file %}
<p><a href="{{ '/files/Siwon_Sung_CV.pdf' | relative_url }}" target="_blank" rel="noopener">Open CV in a new tab</a> · <a href="{{ '/files/Siwon_Sung_CV.pdf' | relative_url }}" download>Download PDF</a></p>

<iframe src="{{ '/files/Siwon_Sung_CV.pdf' | relative_url }}#view=FitH" width="100%" height="1100" style="border: 1px solid #ddd; border-radius: 4px;" title="Siwon Sung CV"></iframe>
{% else %}
<p>CV PDF will appear here once <code>files/Siwon_Sung_CV.pdf</code> is uploaded.</p>
{% endif %}
