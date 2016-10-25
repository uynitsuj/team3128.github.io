---
layout: page
title: Donate
permalink: /donate/
---

The Aluminum Narwhals is a part of the [Canyon Crest Academy Foundation](http://canyoncrestfoundation.org/), a 501(c)3 non-profit organization. Tax ID 03-0542702.

All of your donations to the Aluminum Narwhals are tax deductible. If you would like more information regarding your donation, you can contact the Executive Director, Joanne Couvrette, at [joanne.couvrette@sduhsd.net](mailto:joanne.couvrette@sduhsd.net) or (858) 350-0253 x4005.

### How do your donations help us?
We love what we do, and we wish we could achieve everything we think up. The only problem is that everything we need - electronics, lumber, gear boxes, aluminum, polycarbonate, coaching, travel - costs money. That's why we need you; with your donation, we are able to realize our dreams and learn valuable skills.

<table width="100%" cellpadding="5px">
	<tr>
		<td width="50%">
			<div class="newbutton hoverAnimate" style="text-align: center;" onClick="javascript:location.href='/resources/team-info/TeamInfoPacket.pdf'">
				Team Info Packet (.pdf)
			</div>
		</td>
		<td width="50%">
			<div class="newbutton hoverAnimate" style="text-align: center;" onClick="javascript:location.href='/about/budget/'">
				Learn more about why we need donations
			</div>
		</td>
	</tr>
</table>


### How to donate:
+ Use our [online form](http://weblink.donorperfect.com/QuestRobotics) to make a donation directly to our team
+ You can also write a check payable to ‘Canyon Crest Academy Foundation’ with ‘QUEST/Robotics’ on the memo line, and drop it off or mail it to:
  *5951 E Village Middle Loop Rd
  San Diego, CA 92130*

### Donation Levels
All of our donors are incredibly important to us. We recognize all of our donor in accordance with their giving level.
For additional benefits, see the [CCA Foundation Giving Levels]("http://www.canyoncrestfoundation.org/recognition/giving-levels-and-donor-premiums")

<table class="levels" width="100%" border="0" cellpadding="10" cellspacing="0">
	{% for level in site.data.sponsor_levels %}
	  <tr>
	    <td bgcolor="{{ level.color }}" align="center">
	      <b><font color="white" size="40px">{{ level.level }}</font></b>
	      <br>
	      <font color="white">{{ level.money }}</font>
	    </td>
	    <td>
	      <ul>
	         {{ level.benefits }}
	      </ul>
	    </td>
	  </tr>
	{% endfor %}
</table>

<table class="mobilelevels" width="100%" border="0" cellpadding="10" cellspacing="0">
	{% for level in site.data.sponsor_levels %}
  	<tr>
    	<td bgcolor="{{ level.color }}" align="center">
      	<b><font color="white" size="40px">{{ level.level }}</font></b>
      	<br>
      	<font color="white">{{ level.money }}</font>
    	</td>
		</tr>
		<tr>
    	<td>
      	<ul>
         	{{ level.benefits }}
      	</ul>
    	</td>
  	</tr>
	{% endfor %}
</table>
