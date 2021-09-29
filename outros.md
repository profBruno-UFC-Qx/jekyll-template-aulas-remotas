---
title: Atividades práticas
#youtubeId1: x7oWQXAB4fo
jsarr:
- /assets/js/sheetApi.js
---

### Atividades Práticas

<table>
 <thead>
    <tr>
        <th> Nome </th>
        <th> Repositório </th>
        <th> Peso </th>
        <th> Extra </th>
        <th> Link para envio </th>
        <th> Qtd Enviados </th>
    </tr>
 </thead>
 <tbody>
{% assign atividades = site.atividades | sort: "numero" %}
{% for atividade in atividades %}
    <tr>
        <td> {{ atividade.nome }} </td>
        <td> <a href="{{ atividade.repo }}">Repositório</a> </td>
        <td>{{ atividade.peso }} </td>
        <td> {{ atividade.extra }} </td>
        <td> <a href="{{ atividade.link}}" class="btn">Enviar</a></td>
        <td> <span id="pp{{ atividade.numero }}"></span> </td>
    </tr>
{% endfor %}
  </tbody>
</table>

### Passo a passo para iniciar uma atividade prática
{% comment %}
{% include youtubePlayer.html id=page.youtubeId1 %}
{% endcomment %}

