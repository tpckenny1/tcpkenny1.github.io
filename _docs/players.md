---
layout: default
title: Players DataTables
---

<!-- Page Heading -->
<h1 class="h3 mb-2 text-gray-800">學校</h1>
<script>
$(document).ready(function(){
    schoolfullname = getSchoolFullname();
    if ((schoolfullname !== null) & (typeof schoolfullname !== "undefined") & (schoolfullname !== "")) { 
        $(".h3, .mb-2, .text-gray-800").text(schoolfullname);
    }
});
</script>
<p class="mb-4">The datatable recorded the daily performance data of players.</p>

{% include datatable.html title="Player Datatable" file="table-example" %}
{% include charts/area.html title="Player Stat" width=8 showDetails='true' %}
