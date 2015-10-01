---
layout: page
---

# Meetings

{% for meeting in site.categories.meetings %}
### {{ meeting.date | date: '%B %d, %Y' }}
{{ meeting.excerpt }}
<p>
<a class="btn btn-primary btn-lg" href="{{ meeting.url }}" role="button">Read more »</a>
</p>
{% endfor %}

<script type="text/javascript">
  $("#meetingsnav").addClass("active");
</script>
