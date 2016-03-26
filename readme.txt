README:
<link href="{% static 'reviews/css/reviews.css' %}" rel="stylesheet" />
<style>
        #abstract_map {
            text-align:center;
            padding-bottom: 1em;
            overflow: auto;
            padding-left: 10px;
            padding-right: 10px;
        }
        #abstract_map > h1 {
            color:white;
            line-height: 1.5em;
            text-shadow: 0 2px 0 black;
        }
        .global_map .review_container {
            width: 100%;
            height: 100%;
            max-width: 1000px;
            max-height: 40px;
            left: calc(50% - 500px);
        }
        #abstract_map .global_map {
            margin: 0 auto;
            max-width: 1000px;
            width: 100%;
            height: 500px;
        }
</style>
<html>
<div id="abstract_map" class="tasky_wall_style careers">
    <h1>
        What our interns saying
    </h1>
    <div class="blue_links global_map">
        <div class="review_container">
            {% if selected_layout %}
            {% get_map_layout layout=selected_layout %}
            {% endif %}
        </div>
    </div>
</div>
</html>
