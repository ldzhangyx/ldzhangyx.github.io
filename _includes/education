<div class="publications">
  <ol class="bibliography">

    <h2 style="margin:0 10px 0;">Education</h2>

    {% for education in site.data.education %}
      <li>
        <div class="pub-row">
          <!-- 左边的列，用于显示学校或机构图标 -->
          <div class="col-sm-3" style="position: relative;padding-right: 15px;padding-left: 15px;">
            {% if education.logo %}
              <img src="{{ education.logo }}" class="teaserinternship img-fluid z-depth-1" style="width=100;height=40%;">
            {% endif %}
          </div>

          <!-- 右边的列，用于显示教育的详细信息 -->
          <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
            <div class="title"><strong>{{ education.institution }}</strong></div>
            <div>Degree: {{ education.degree }}</div>
            <div>Duration: {{ education.duration }}</div>
            {% if education.supervisors %}
              <div>Supervisors: {{ education.supervisors }}</div>
            {% endif %}
            {% if education.thesis %}
              <div>Thesis: <a href="{{ education.thesis.url }}">{{ education.thesis.title }}</a></div>
            {% endif %}
          </div>
        </div>
        <br>
      </li>
    {% endfor %}

  </ol>
</div>
