## Welcome to MemArch-Lab!

**Dr. Xin Xin** is a Tenure-Track Assistant Professor in the Department of Electrical and Computer Engineering at the [University of Central Florida](https://www.ucf.edu/) (since Aug. 2023). He received his Ph.D. in Electrical and Computer Engineering from the [University of Pittsburgh](https://www.pitt.edu/) in 2023 (Advisor: Jun Yang), his M.E. from [Tsinghua University](https://www.tsinghua.edu.cn/) in 2016, and his B.S. from [Lanzhou University](https://www.lzu.edu.cn/) in 2013.

His research interests primarily lie in the field of **computer architecture** with a focus on **memory subsystems**, e.g., main memory performance/power/reliability, processing-in-memory (PIM)/near-data-processing (NDP), hybrid DRAM-NVM system, and memory-based accelerators.

[CV]({{ site.baseurl }}/CV-Xin.pdf) | [Email](mailto:xin.xin@ucf.edu)

---

### Research Highlights

<div class="row">
{% for item in site.data.highlights %}
<div class="col-sm-6" style="margin-bottom:15px;">
<div class="well" style="min-height:160px; padding:10px;">
<img src="{{ site.baseurl }}/images/highlights/{{ item.image }}" style="width:100%; max-height:80px; object-fit:cover; margin-bottom:8px;" />
<h5 style="margin:0 0 4px;"><strong>{{ item.title }}</strong> <small>({{ item.venue }})</small></h5>
<p style="font-size:12px; margin:0;">{{ item.description }}</p>
</div>
</div>
{% endfor %}
</div>
