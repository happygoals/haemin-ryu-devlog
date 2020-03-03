---
layout: post
title: "Intern Program Brings Problem-solving Skills"
author: "Haemin Ryu"
---

# Intern Program Brings Problem-solving Skills

## First Bugs: Update IWDC Member User form
[link](https://www.iwdc.coop/membership-information/become-a-member)
* Problem from Clients: Lela needs the Canandia state to populate when country is selected. In the example she sent, the user chose Montreal and Iowa was added at the Company State. Picture included.
* Problem I confirm: 
![Dropdown-previous](../assets/post/030220/dropdown_statebycountry_pre.png)
* Solution
* Code

<figure class="highlight"><pre><code class="language-js" data-lang="js"><table class="rouge-table"><tbody><tr><td class="gutter gl">
<pre class="lineno">1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
</pre>
</td>
<td class="code">
<pre>
  <script type="text/javascript">	
    function UpdateStatebyCountry() {
      var cID = document.getElementById("country_code");
      var countryVal = cID.options[cID.selectedIndex].value; 
      var countryTxt = cID.options[cID.selectedIndex].text;

	if (countryVal == "CA"){
                document.getElementById("state_ca").style.display = "block";
		document.getElementById("state_mx").style.display = "none";
		document.getElementById("state_us").style.display = "none";
        }  
	else if (countryVal == "MX"){
               document.getElementById("state_ca").style.display = "none";
	       document.getElementById("state_mx").style.display = "block";
	       document.getElementById("state_us").style.display = "none";
        }
        else if (countryVal == "US"){
               document.getElementById("state_ca").style.display = "none";
	       document.getElementById("state_mx").style.display = "none";
	       document.getElementById("state_us").style.display = "block";
        }else{
               document.getElementById("state_ca").style.display = "none";
	       document.getElementById("state_mx").style.display = "none";
	       document.getElementById("state_us").style.display = "none";	
	}
    }
    
</pre></td></tr></tbody></table></code></pre></figure>


* Result
![Dropdown1](../assets/post/030220/dropdown-address-country-state.gif "DropDown button result")
