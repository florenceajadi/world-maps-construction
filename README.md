<h4>Microsoft Sentinel</h4>
<p>is a cloud-based security info and event management (SIEM) solution in Azure. I'll be gathering security data, detecting potential threats, analyzing and understanding security incidents, and automate respond to threats and alerts. </p>
<p>
  <img src="https://github.com/user-attachments/assets/bd16c933-42af-4404-8639-97eff965aa81" height="80%" width="80%" />
</p>
<p>
This is a JSON config code for running KQL in Sentinel. This query runs against the Syslog table, filtering logs related to failed pswd attempts. It extracts IP address from log msgs and uses a watchlist called geoip to match 
IP addresses with geographical locations like latitude, city, country, and longitude. It selects specific colums like time, source IP, destination host, and geographical info.</p>
  <p>
  <img src="https://github.com/user-attachments/assets/76cd034d-3c34-4f2f-9c69-2791c078cc2c" height="80%" width="80%" />
    <p>The results are shown on the map, highlighting locations where failed login attempts are detected.</p>
  </p>
<p>
   <img src="https://github.com/user-attachments/assets/5b889b5a-8d0c-408b-a37f-dddc9ef1c3f5" height="80%" width="80%" />
</p>
<p>this is an attack on an MS SQL server. The GeoIPDB_FULL loads the watchlist 'geoip' that contains geolocation data for IP addresses. I'm able to extract IP: addresses from event logs using IPAddress_REGEX_PATTERN. 
This query is simply looking for events in the Application log with Event ID 18456, which relates to failed login attempts in SQL server. </p>
 <img src="" height="80%" width="80%" />
<p>
The map shows the data is visualized, using a heatmap palette ranging from green to red to show the intensity of attacks. Also the results are on the map, showing the locations of the attackers based on their IP addresses.
</p>
<br />
 <p>
  <img src="" height="80%" width="80%" />
</p>
<p>

</p>
  <img src="" height="80%" width="80%" />
<p>

</p>
<br />
  <img src="" height="80%" width="80%" />
<p></p>
  
  <img src="https://github.com/user-attachments/assets/d93268d8-3a32-4c78-a5c7-95ce53cab27e" height="80%" width="80%" />
<p>This code is a JSON config that creates a visualization of failed login attempts (Event ID 4625) mapped to geographic locations based on IP addresses. It uses a watchlist called 'geoip' to get location data for IP addresses.
It also looks at failed login events, as well as connects the IP addresses from the events to their locations using the watchlist.</p>
<br />
  <img src="https://github.com/user-attachments/assets/9a7d9443-7b86-47a5-aaac-6e62b25a08a1" height="80%" width="80%" />
<p>The data also shows on the map with locations highlighted where more failed logins occur.</p>
