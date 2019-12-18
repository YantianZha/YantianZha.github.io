---
layout: page
title:
permalink: /

pubs:

pubs:

    - title:   "Plan-Recognition-Driven Attention Modeling for Visual Recognition"
      author:  "Zha, Yantian, Yikang Li, Tianshu Yu, Subbarao Kambhampati and Baoxin Li"
      journal: "AAAI 2019 Workshop on Plan, Activity, and Intent Recognition (PAIR)."
      url:     "https://arxiv.org/abs/1812.00301"

    - title:   "Recognizing plans by learning embeddings from observed action distributions"
      author:  "Zha, Yantian, Yikang Li, Sriram Gopalakrishnan, Baoxin Li, and Subbarao Kambhampati"
      journal: "In Precendings of International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2018 as an Extended Abstract."
      url:     "https://dl.acm.org/citation.cfm?id=3238103"
      media:
        - name: "Code"
          url: "https://github.com/YantianZha/Distr2Vec"
  
    - title:   "Discovering Underlying Plans Based on Shallow Models"
      author:  "Zhuo, Hankz Hankui, Zha, Yantian, Kambhampati, Subbarao, and Tian, Xin"
      journal: "In Proceedings of ACM Transactions on Intelligent Systems and Technology (ACM-TIST) 2019."
      url:     "https://yochan-lab.github.io/papers/files/papers/hankz_tist_19.pdf"
      media:
        - name: "Code"
          url: "https://github.com/YantianZha/Discovering-Underlying-Plans-Based-on-Shallow-Models"

    - title:   "Explicability as Minimizing Distance from Expected Behavior"
      author:  "Kulkarni, Anagha, Zha, Yantian, Chakraborti, Tathagata, Vadlamudi, Satya Gautam, Zhang, Yu and Kambhampati, Subbarao"
      journal: "In Precendings of International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2019 as an Extended Abstract."
      url:     "https://yochan-lab.github.io/papers/files/papers/anagha-aamas-2019.pdf"
      media:
        - name: "YouTube"
          url:  "https://youtu.be/iLG-ANQtYms"


---

{% include image.html url="images/photo.png" caption="" max_width="3px" align="right" %}

Yantian is a PhD student working in the [Yochan](https://yochan-lab.github.io/home/){:target="_blank"} research group directed by [Prof. Subbarao Kambhampati](http://rakaposhi.eas.asu.edu/){:target="_blank"}, at [Arizona State University](http://www.asu.edu){:target="_blank"}. Prior to joining Yochan Lab in 2015, he worked with [Prof. Xudong Ma](https://automation.seu.edu.cn/2019/0528/c24505a275234/page.htm){:target="_blank"}, and [Dr. Kun Qian](https://automation.seu.edu.cn/2019/0528/c24504a275190/page.htm){:target="_blank"} in the Institute of Intelligent Robotics and Intelligent Control at Southeast University. 

Yantian is interested in planning, vision, and their applications in robotics. 

If you'd like to contact me, please drop me a mail at [yzha3 at asu dot edu](mailto:yzha3@asu.edu) or find me on [LinkedIn](https://www.linkedin.com/in/ytzha){:target="_blank"}.

# <a name="publications"></a>Publications 

{% for pub in page.pubs %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}){:target="_blank"}<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}}){:target="_blank"}] {% endfor %}{% endif %}

{% endfor %}
