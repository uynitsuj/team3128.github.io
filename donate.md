---
layout: page
title: Donate
permalink: /donate/
---

The Aluminum Narwhals is a part of the [Canyon Crest Academy Foundation](http://canyoncrestfoundation.org/), a 501(c)3 non-profit organization. Tax ID 03-0542702.

All of your donations to the Aluminum Narwhals are tax deductible. If you would like more information regarding your donation, you can contact the Executive Director, Joanne Couvrette, at [joanne.couvrette@sduhsd.net](mailto:joanne.couvrette@sduhsd.net) or (858) 350-0253 x4005.

### How do your donations help us?
We love what we do, and we wish we could achieve everything we think up. The only problem is that everything we need - electronics, lumber, gear boxes, aluminum, polycarbonate, coaching, travel - costs money. That's why we need you; with your donation, we are able to realize our dreams and learn valuable skills.

<div>
<a href="/resources/">
<div class="button hover_animate" style="text-align: center;">
Additional Team Information
</div>
</a>
</div>
<br>

### How to donate:
In order to keep developing our skills and pursuing our goals, our requested donation is $650. There are two ways to support our team:

<table width="100%">
<tr>
<td width="50%" style="text-align: center; background: #1b1464">
<font style="font-size:20pt; color: white;">Online</font>
<br>
</td>
<td width="50%" style="text-align: center; background: #072682">
<font style="font-size:20pt; color: white;">By Check</font>
</td>
</tr>
<tr>
<td width="50%" style="padding:5px;vertical-align: top;">
<b>You can donate directly to our team using the online donation form.</b>
<ol>
<li>Head over to the <a href="https://interland3.donorperfect.net/weblink/weblink.aspx?name=E113627&id=20">CCA Foundation online donation form</a>.</li>
<li>Select the "Gift to a Quest Program" checkbox.</li>
<li>Select "Robotics Team" from the dropdown.</li>
</ol>

</td>
<td width="50%" style="padding:5px;vertical-align: top; background: #f0f0f0">
<b>You can also donate directly to our team by writing us a check.</b>
<ol>
<li>Make the check payable to:</li>
<i>‘Canyon Crest Academy Foundation’</i>
<li>Include <i>‘QUEST/Robotics’</i> on the memo line</li>
<li>Drop off the check or mail it to:</li>
<i>5951 E Village Middle Loop Rd <br>
San Diego, CA 92130</i>
</ol>
</td>
</tr>
</table>

### Donation Levels
All of our donors are incredibly important to us. We recognize all of our donor in accordance with their giving level.
For additional benefits, see the [CCA Foundation Giving Levels](http://www.canyoncrestfoundation.org/recognition/giving-levels-and-donor-premiums).


<script>
function toggle(level) {
	var elements = document.getElementsByClassName("circle");

	$(document.getElementById("Title")).removeClass('expanded');
	$(document.getElementById("Platinum")).removeClass('expanded');
	$(document.getElementById("Gold")).removeClass('expanded');
	$(document.getElementById("Silver")).removeClass('expanded');
	$(document.getElementById("Bronze")).removeClass('expanded');
	$(document.getElementById(level)).addClass('expanded');

	$(document.getElementById("Titleinfo")).css('display', "none");
	$(document.getElementById("Platinuminfo")).css('display', "none");
	$(document.getElementById("Goldinfo")).css('display', "none");
	$(document.getElementById("Silverinfo")).css('display', "none");
	$(document.getElementById("Bronzeinfo")).css('display', "none");
	$(document.getElementById(level + "info")).css('display', "table");
}

$( document ).ready(function() {
	toggle("Title");
});
</script>

<div class="levels">
<div style="text-align: center;"><i>Click one of the donation levels below to learn about the benefits.</i></div>
<table width="100%" border="0" cellpadding="10" cellspacing="0">
	<tr>
	{% for level in site.data.sponsor_levels %}
	    <td width="172px" height="152px" align="center" class="circle hover_animate" id="{{ level.level }}" style="background: {{ level.color }};" onClick='toggle("{{ level.level }}")'>
				<div>
					{{ level.level }}
				</div>
	    </td>
	{% endfor %}
	</tr>
</table>

{% for level in site.data.sponsor_levels %}
	<table id="{{ level.level }}info" style="display: none;" width="100%" border="0" cellpadding="10" cellspacing="0">
		<tr>
			<td style="width: 250px;" bgcolor="{{ level.color }}" align="center">
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
	</table>
{% endfor %}
</div>

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
