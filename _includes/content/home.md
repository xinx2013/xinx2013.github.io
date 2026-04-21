## Welcome to MemArch-Lab!

**Dr. Xin Xin** is a Tenure-Track Assistant Professor in the Department of Electrical and Computer Engineering at the [University of Central Florida](https://www.ucf.edu/) (since Aug. 2023). He received his Ph.D. in Electrical and Computer Engineering from the [University of Pittsburgh](https://www.pitt.edu/) in 2023 (Advisor: Jun Yang), his M.E. from [Tsinghua University](https://www.tsinghua.edu.cn/) in 2016, and his B.S. from [Lanzhou University](https://www.lzu.edu.cn/) in 2013.

His research interests primarily lie in the field of **computer architecture** with a focus on **memory subsystems**, e.g., main memory performance/power/reliability, processing-in-memory (PIM)/near-data-processing (NDP), hybrid DRAM-NVM system, and memory-based accelerators.

---

### Research Highlights

<div class="row">
{% for item in site.data.highlights %}
<div class="col-sm-6" style="margin-bottom:15px;">
<div class="well" style="min-height:160px; padding:10px;">
<div style="width:100%; height:120px; display:flex; align-items:center; justify-content:center; background:#f9f9f9; margin-bottom:8px;">
<img src="{{ site.baseurl }}/images/highlights/{{ item.image }}" style="max-width:100%; max-height:120px; object-fit:contain;" />
</div>
<p style="margin:0 0 4px;"><strong>{{ item.title }}</strong> <small>({{ item.venue }})</small>{% if item.paper %} <a href="{{ item.paper }}" target="_blank" rel="noopener">[paper]</a>{% endif %}{% if item.slide %} <a href="{{ item.slide }}" target="_blank" rel="noopener">[slide]</a>{% endif %}</p>
<p class="small" style="margin:0;">{{ item.description }}</p>
</div>
</div>
{% endfor %}
</div>
