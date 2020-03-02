---
layout: post
title: "Intern Program Brings Problem-solving Skills"
author: "Haemin Ryu"
---

# Intern Program Brings Problem-solving Skills

## First Bugs: Update IWDC Member User form
[link](www.iwdc.coop)
* Problem from Clients: Lela needs the Canandia state to populate when country is selected. In the example she sent, the user chose Montreal and Iowa was added at the Company State. Picture included.
* Problem I confirm: 
* Solution
* Code
'''ruby

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
  </script> 

    <div class="input-row">
	  <span style="color:#FF0000;">*</span>
      <label for="country_code">Country</label>
      <select  id="country_code" name="country_code" onchange="UpdateStatebyCountry()">
        <option value="">--None--</option>
        <option value="CA">Canada</option>
        <option value="MX">Mexico</option>
        <option value="US">United States</option>
      </select>
    </div>

    <div class="input-row">
	  <span style="color:#FF0000;">*</span>
      <label for="street">Address</label>
      <textarea name="street"></textarea>
    </div>

    <div class="input-row">
	  <span style="color:#FF0000;">*</span>
      <label for="city">City</label>
      <input  id="city" maxlength="40" name="city" size="20" type="text" />
    </div>

    <div class="input-row">
	  <span style="color:#FF0000;">*</span>
      <label for="state_code">State/Province</label>
      <select id ="state_ca" name="state_code" style="display:none">
        <option value="">--None--</option>
        <option value="AB">Alberta</option>
        <option value="BC">British Columbia</option>
        <option value="MB">Manitoba</option>
        <option value="NB">New Brunswick</option>
        <option value="NL">Newfoundland and Labrador</option>
        <option value="NS">Nova Scotia</option>
        <option value="NU">Nunavut</option>
        <option value="ON">Ontario</option>
        <option value="PE">Prince Edward Island</option>
        <option value="QC">Quebec</option>
        <option value="SK">Saskatchewan</option>
      </select>
      <select  name="state_code" id ="state_mx" style="display:none">
        <option value="">--None--</option>
        <option value="AG">Aguascalientes</option>
        <option value="BC">Baja California</option>
        <option value="BS">Baja California Sur</option>
        <option value="CM">Campeche</option>
        <option value="CH">Chihuahua</option>
        <option value="CO">Coahuila</option>
        <option value="CL">Colima</option>
        <option value="DG">Durango</option>
        <option value="GT">Guanajuato</option>
        <option value="GR">Guerrero</option>
        <option value="HG">Hidalgo</option>
	<option value="JA">Jalisco</option>
        <option value="ME">Mexico State</option>
        <option value="MI">Michoacan</option>
        <option value="MO">Morelos</option>
        <option value="NA">Nayarit</option>
        <option value="NL">Nuevo Leon</option>
        <option value="OA">Oaxaca</option>
        <option value="PB">Puebla</option>
        <option value="QE">Queretaro</option>
        <option value="QR">Quintana Roo</option>
        <option value="SL">San Luis Potosi</option>
        <option value="SI">Sinaloa</option>
        <option value="SO">Sonora</option>
        <option value="TB">Tabasco</option>
        <option value="TM">Tamaulipas</option>
        <option value="TL">Tlaxcala</option>
        <option value="VE">Veracruz</option>
        <option value="YU">Yucatan</option>
        <option value="ZA">Zacatecas</option>
      </select>
<select  id ="state_us" name="state_code" style="display:none">
        <option value="">--None--</option>
        <option value="AL">Alabama</option>
        <option value="AK">Alaska</option>
        <option value="AZ">Arizona</option>
        <option value="AR">Arkansas</option>
        <option value="CA">California</option>
        <option value="CO">Colorado</option>
        <option value="CT">Connecticut</option>
        <option value="DE">Delaware</option>
        <option value="DC">District of Columbia</option>
        <option value="DF">Federal District</option>
        <option value="FL">Florida</option>
        <option value="GA">Georgia</option>
        <option value="HI">Hawaii</option>
        <option value="ID">Idaho</option>
        <option value="IL">Illinois</option>
        <option value="IN">Indiana</option>
        <option value="IA">Iowa</option>
        <option value="KS">Kansas</option>
        <option value="KY">Kentucky</option>
        <option value="LA">Louisiana</option>
        <option value="ME">Maine</option>
        <option value="MD">Maryland</option>
        <option value="MA">Massachusetts</option>
        <option value="MI">Michigan</option>
        <option value="MN">Minnesota</option>
        <option value="MS">Mississippi</option>
        <option value="MO">Missouri</option>
        <option value="MT">Montana</option>
        <option value="NE">Nebraska</option>
        <option value="NV">Nevada</option>
        <option value="NH">New Hampshire</option>
        <option value="NJ">New Jersey</option>
        <option value="NM">New Mexico</option>
        <option value="NY">New York</option>
        <option value="NC">North Carolina</option>
        <option value="ND">North Dakota</option>
        <option value="OH">Ohio</option>
        <option value="OK">Oklahoma</option>
        <option value="OR">Oregon</option>
        <option value="PA">Pennsylvania</option>
        <option value="PR">Puerto Rico</option>
        <option value="RI">Rhode Island</option>
        <option value="SC">South Carolina</option>
        <option value="SD">South Dakota</option>
        <option value="TN">Tennessee</option>
        <option value="TX">Texas</option>
        <option value="UT">Utah</option>
        <option value="VT">Vermont</option>
        <option value="VA">Virginia</option>
        <option value="WA">Washington</option>
        <option value="WV">West Virginia</option>
        <option value="WI">Wisconsin</option>
        <option value="WY">Wyoming</option>
      </select>
    </div>
'''
* Result

