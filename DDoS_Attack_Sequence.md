'''markdow
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
  Firewall->> WebServer Update rules to book new pattern
  '''
  '''
