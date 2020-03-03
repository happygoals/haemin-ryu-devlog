---
layout: post
title: "Intern Program Brings Problem-solving Skills"
author: "Haemin Ryu"
---

# Intern Program Brings Problem-solving Skills

## Questions that I asked my supervisor on the First Day of Internship
1. What skills will I need to grow? 
2. How can i be a valuable team member? 
3. How will I fit into the culture? 
4. What do you want me to achieve in this internship program? 
5. What are the things you would like me to accomplish in my first week on the job?
6. How do you prefer to communicate, email or in person? 
7. How often would you like me to give you updates and progress reports? 

## First Bugs: Update IWDC Member User form
[link](https://www.iwdc.coop/membership-information/become-a-member)
* Problem from client's request: The Canandian state to populate when country is selected. For excample, the user chose Montreal and Iowa was added at the Company State. It should be fixed.
* Problem I confirmed: 
The state populating issue by country selection
![Dropdown-previous](../assets/post/030220/dropdown_statebycountry_pre.png)
* Solution
I initially thought the address order is correct because the order of the address input forms was intentionally aligned by the general American style address format. However, as a user perspective, I changed my mind about the address form order. I would like to suggest it to change the order to select the country first and then the state/province. Then, the state/province can populate when country is selected. 

* JavaScript Code
<figure class="highlight"><pre><code class="language-js" data-lang="js"><table class="rouge-table"><tbody><tr><td class="gutter gl">
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
