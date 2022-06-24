---
layout: default
title: Lab Milestones
description: A list of milestones for every lab
nav_order: 3
lab_course: cs10_fa21.html
labs:

---

# Lab Milestones

On this page, you will find a list of questions related to each lab. These questions highlight
what we think are the most important questions / takeaways from the lab and are meant for you to
check your understanding.


{% for lab in page.labs %}
<details open>
  <a name="lab-{{ lab.lab_no }}"></a>
  <summary>
    <div class="label label-lab"><strong>Lab {{ lab.lab_no }}</strong></div>
    {{ lab.lab_name }}
  </summary>
  <br>
  <a href="https://cs10.org/bjc-r/topic/topic.html?topic={{ lab.topic_file |urlencode }}&course={{ page.course }}&novideo&noreading&noassignment" target="_bank">
  View Lab {{ lab.lab_no }}
  </a>
  <ul>
    {% for question in lab.questions %}
      <li>{{ question | markdownify}}</li>
    {% endfor %}
  </ul>
</details>
{% endfor %}

**Lab 1**{: .label .label-lab}[Welcome to Snap!](https://bjc.edc.org/bjc-r/cur/programming/1-introduction/1-building-an-app/1-creating-a-snap-account.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment)
- How do you ensure you are logged into Snap!?
- Show us that you've saved this lab to your Snap! account. This is important so you can refer back to your work for future assignments!
- Show us your Alonzo game.
- Is there anything you found interesting or challenging about Snap!?

**Lab 2**{: .label .label-lab}[Looping and Custom Blocks](https://bjc.edc.org/bjc-r/cur/programming/1-introduction/2-gossip-and-greet/1-pair-programming.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment)
- Why do we create our own blocks (or procedures)?
- What is the difference between a reporter and a command block? What is an example of each?
- Show us your "more complicated gossip" block. 
- In the last exercise, we asked you to have "more complicated who" call itself. What do you think is happening here? Don't worry if you don't fully understand this; we will formalize this in a few days!

**Lab 3**{: .label .label-lab}[Conditional Blocks](https://bjc.edc.org/bjc-r/cur/programming/1-introduction/3-drawing/1-exploring-motion.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment)
- In this lab you learned a few blocks that achieve repetition. Which blocks are these, and when might you use them?
- How do you add an input to a block (or procedure)? Why might you do want to do this?
- Show your most recent pinwheel block. What do the different inputs (or argumnets) control?
- Show us your squiral block.

**Lab 4**{: .label .label-lab}[Collecting Data into Lists](https://cs10.org/bjc-r/topic/topic.html?topic=berkeley_bjc/lists/lists-I.topic&course=cs10_su19.html&novideo&noreading&noassignment)
- What is a list? Why would we use a list of 10 elements instead of just making 10 variables?
- What do `map`, `keep`, and `combine` each do?
- Show us your `acronym` block.
- Show us your `expand` block.
- What is the difference between the `for each (item)` loop and the `for (i)` loop we have used in previous labs?
