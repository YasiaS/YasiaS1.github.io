'''markdown
''' meramaid 
sequenceDiagram
  Attacker->>Bots: Instruct to start attack
  Bots->>WebServer: Flood with requests
  Firewall->>WebServer: Forward requests
  WebServer->>Firewall: Overwhelmed by requests
  Firewall->>Bots: Identify suspious activity
  Firewall->> WebServer: Block maliciuos requests
  Attacker->>Bots: Change attack pattern
  Bots->> WebServer: Continue flood with modified requests
  '''
  '''
[![](https://mermaid.ink/img/pako:eNp1ksFuAiEQhl9lwtm-AAeTamPSQ9NDD73sZYRZl8gydhjcbIzvXtaqVZuegOHjZ_h_DsaxJ2NNpq9CydFLwI1g3ySAZ1V0W5Kn-XzBmi28pqxSnIIyZEVRwBMywRNRwU9af5DsSSysIrOHIWgHMolnzRO4CkIDxvgAswwo_o68blf0csrCey0MHcWePKzH_6TPDXtKGtoRcsm7wCUDOg37oOMDDjetLCK7LfQYgwuF890NfyxZdpg2dPYBdnUkSTd-3AovuTaTCkH760zPPrSB7h9uZqYn6TH4GsxhqjRGO-qpMbZOPbVYojamSceKYlH-GJMztoZDMyNcNp2xLcZcV2XnUS-pXqvkg7K8_UR_-gHHby09uZY?type=png)](https://mermaid.live/edit#pako:eNp1ksFuAiEQhl9lwtm-AAeTamPSQ9NDD73sZYRZl8gydhjcbIzvXtaqVZuegOHjZ_h_DsaxJ2NNpq9CydFLwI1g3ySAZ1V0W5Kn-XzBmi28pqxSnIIyZEVRwBMywRNRwU9af5DsSSysIrOHIWgHMolnzRO4CkIDxvgAswwo_o68blf0csrCey0MHcWePKzH_6TPDXtKGtoRcsm7wCUDOg37oOMDDjetLCK7LfQYgwuF890NfyxZdpg2dPYBdnUkSTd-3AovuTaTCkH760zPPrSB7h9uZqYn6TH4GsxhqjRGO-qpMbZOPbVYojamSceKYlH-GJMztoZDMyNcNp2xLcZcV2XnUS-pXqvkg7K8_UR_-gHHby09uZY)

1. Attacker instructs Bots to Start Attack. The attacker sends instructions to multiple compromised systems(bots) t intiate a DDoS attack.
2. Bots Flood WebServer with requests. The Bots receive the attack instructions and begin sending a high volume of request to the web server.
3. Firewall Forwarda Requests to Web Server. Intially, the firewall forwards the incomingg requests from the bots to thebtarget server without filtering them. The firewall acts as a getaway.
4. WebServer overwhelmed by requests. The webserver receives an overwhelming number of requests, leading to a denial of service for legtimate users.
5. Firewall identifies suspicious activity. The firewall detects unusual traffic patterns indicative of a DDoS attack, such as a sudden spike in requests from multiple sources.
6. Firewall Blocks malicious requests. The firewall implements rules to block incoming requests from the bots, mitgating the impact on the webserver.
7. Firewall traces back to source. The firewall attempts to trace the origin of the attack to identify the attacker and the compromised systems involved
8. Attacker changes attack pattern. In reponse to the firewalls defensive measures, the attacker modifies the attack pattern to bypass the current firewall rules
9. Bots continue flood with modified requests. The bots rececive new instructions from the attacker and resume flooding the web server with requests using the modified pattern.
