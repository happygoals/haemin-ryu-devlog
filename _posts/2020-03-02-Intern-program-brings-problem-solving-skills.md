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
### Problem from client's request:
* The Canandian state to populate when country is selected. For excample, the user chose Montreal and Iowa was added at the Company State. It should be fixed.
### Problem I confirmed: 
The state populating issue by country selection
![Dropdown-previous](../assets/post/030220/dropdown_statebycountry_pre.png)
### Solution
I initially thought the address order is correct because the order of the address input forms was intentionally aligned by the general American style address format. However, as a user perspective, I changed my mind about the address form order. I would like to suggest it to change the order to select the country first and then the state/province. Then, the state/province can populate when country is selected. 
### Implementation with jQuery, .Net Framework 3.5, xslt, Cirrus Framework, smtp4dev
[jQuery Code](https://happygoals.github.io/takeaways/jquery/jquery-with-dotnet)

### Result
![Dropdown1](../assets/post/030220/dropdown-address-country-state.gif "DropDown button result")
