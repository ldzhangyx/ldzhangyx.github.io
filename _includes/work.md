
<div class="publications">
<ol class="bibliography">

<h2 style="margin:0 10px 0;">Work</h2>

{% for work in site.data.work %}
<li>
    <div class="pub-row">
        <!-- 左边的列，用于显示公司图标 -->
        <div class="col-sm-3" style="position: relative;padding-right: 15px;padding-left: 15px;">
            {% if work.logo %} 
            <img src="{{ work.logo }}" class="teaserinternship img-fluid z-depth-1" style="width=100;height=40%;">
            {% endif %}
        </div>

        <!-- 右边的列，用于显示工作的详细信息 -->
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
            <div class="title"><strong>{{ work.company }}</strong></div>
            <div>Team: {{ work.team }}</div>
            <div>Role: {{ work.role }}</div>
            {% if work.topic %}
            <div>Responsibility: {{ work.topic }}</div>
            {% endif %}
            <div>{{ work.duration }}</div>
        </div>
    </div>
    <br>
</li>
{% endfor %}


</ol>
</div>
