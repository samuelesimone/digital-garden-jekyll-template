---
title: Insertion sort
---
<a class="internal-link" href="{{ site.baseurl }}/" style="display: inline-flex; align-items: center; margin: 20px 0; text-decoration: none; color: #007bff; font-size: 24px;">
 <i class="fa-solid fa-igloo"></i>Go Home
</a>

{% for i in (1..27) %}
<section  style="display:block; margin-top: 64px" data-transition="fade">
  <img data-src="{{ site.baseurl }}/assets/images/ins-{{ i }}.png">
</section>
{% endfor %}

<section  data-auto-animate>
  <h2>Code in Python for Insertion Sort</h2>
  <pre><code data-trim data-noescape>
        array = [7,5,3,10,1]
        i=1
        while i < len(array):
            j = i
            while j > 0 and array[j - 1] > array[j]:
                    tmp = array[j-1]
                    array[j-1] = array[j]
                    array[j] = tmp 
                    j -= 1
                    print(array)
            i += 1

    
  </code></pre>
</section>


