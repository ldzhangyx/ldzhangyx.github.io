
<div class="publications">
<ol class="bibliography">

<h2 style="margin:0 10px 0;">Internships</h2>

{% for internship in site.data.internships %}
<li>
    <div class="pub-row">
        <!-- 左边的列，用于显示公司图标 -->
        <div class="col-sm-3" style="position: relative;padding-right: 15px;padding-left: 15px;">
            {% if internship.logo %} 
            <img src="{{ internship.logo }}" class="teaserinternship img-fluid z-depth-1" style="width=100;height=40%;">
            {% endif %}
        </div>

        <!-- 右边的列，用于显示实习的详细信息 -->
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
            <div class="title"><strong>{{ internship.company }}</strong></div>
            <div>Topics: {{ internship.topics }}</div>
            <div>Advisors: {{ internship.advisors }}</div>
            {% if internship.topic %}
            <div>Topic: {{ internship.topic }}</div>
            {% endif %}
            <div>{{ internship.duration }}</div>
        </div>
    </div>
    <br>
</li>
{% endfor %}


</ol>
</div>