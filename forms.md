# Forms

There should be a forms tutorial, it is currently hard to get started with it!

## 1.9

Good custom method that uses all features:

    {% if form.errors %}
        <ul class="errors">
            {% for error in form.errors %}
                <li>{{ error }}</li>
            {% endfor %}
        </ul>
    {% endif %}
    {% for field in form %}
        {% if field.errors %}
            <div>{{ field.errors }}</div>
        {% endif %}
        <div>{{ field.label_tag }}</div>
        <div>{{ field }}</div>
        {% if field.help_text %}
            <div class="help">{{ field.help_text|safe }}</div>
        {% endif %}
    {% endfor %}

Remove colon from labels: <http://stackoverflow.com/questions/11622513/blank-label-suffix-across-entire-django-project>
