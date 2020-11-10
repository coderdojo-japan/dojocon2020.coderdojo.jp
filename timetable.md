---
layout: post
title: "タイムテーブル"
---
<img src="{{site.url}}/img/timetable.png" alt="タイムテーブル" style="width: 100%;">

<!--
  <div class="table">
    <h2 class="table-timehead">時間</h2>
    <input type="radio" id="radio-session" name="tab_item" checked>
    <label for="radio-session"><h2 class="table-head">セッション</h2></label>
    <input type="radio" id="radio-workshop" name="tab_item">
    <label for="radio-workshop"><h2 class="table-head">ワークショップ</h2></label>

    <div class="table-column table-time">
    <ol>
      <li>10:00</li>
      <li>10:30</li>
      <li>11:00</li>
      <li>11:30</li>
      <li>12:00</li>
      <li>12:30</li>
      <li>13:00</li>
      <li>13:30</li>
      <li>14:00</li>
      <li>14:30</li>
      <li>15:00</li>
      <li>15:30</li>
      <li>16:00</li>
      <li>16:30</li>
      <li>17:00</li>
      <li>17:30</li>
      <li>18:00</li>
    </ol>
    </div>
    <div class="table-column table-session table-content">
    <ol>
      {% for session in site.data.sessions %}
      <li style="height: calc(({{session.etime}} - {{session.stime}}) * 8px - 20px - 8px); top: calc({{session.stime | minus: 600.0}} * 8px);">
        <div class="session-tag">
          {{session.tag}}
        </div>
        {%if session.url %}<a href="{{session.url}}">{% endif %}
        <h3>{{session.title}}</h3>
        {%if session.url %}</a>{% endif %}
        <p>[{{session.stime | floor | divided_by: 60 }}:{{session.stime | floor | modulo: 60}}-{{session.etime | floor | divided_by: 60 }}:{{session.etime | floor | modulo: 60}}] {{session.speaker}}</p>
      </li>
      {% endfor %}
    </ol>
    </div>
    <div class="table-column table-workshop table-content">
    <ol>
      {% for workshop in site.data.workshops %}
      <li style="height: calc(({{workshop.etime}} - {{workshop.stime}}) * 8px - 20px - 8px); top: calc({{workshop.stime | minus: 600.0}} * 8px); left: calc({{workshop.column}} * (33.33% + 8px));">
        {%if workshop.url %}<a href="{{workshop.url}}">{% endif %}
        <h3>{{workshop.title}}</h3>
        {%if workshop.url %}</a>{% endif %}
        <p>[{{workshop.stime | floor | divided_by: 60 }}:{{workshop.stime | floor | modulo: 60}}-{{workshop.etime | floor | divided_by: 60 }}:{{workshop.etime | floor | modulo: 60}}] {{workshop.speaker}}</p>
        {% for tag in workshop.tag %}
          <span class="tag-workshop">{{tag}}</span>
        {% endfor %}
      </li>
      {% endfor %}
    </ol>
    </div>
  </div>
-->
