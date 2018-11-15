# Project 9 - MHN Honeypot

Time spent: **6** hours spent in total

> Objective: Deploy honeypots and analyze the attack results.

## Attack Report
* Which Honeypot(s) you deployed
  - Dionaea
    - Collects malware samples by pretending to be a vulnerable system
  - Wordpot
    - Collects data on any attempts to scan for WordPress plugins, themes, vulnerabilities
* Any issues you encountered
  - Installation script had a missing package and would corrupt the installation if halted midway (required clean VM)
  - Figuring out how to analyze the malware sample
* A summary of the data collected: number of attacks, number of malware samples, etc.
  - There were a total of 3448 attacks recorded.
  - Two malware samples were captured by Dionaea on port 445 through the Server Message Block (smb) protocol which provides shared access to files.
  - Protocols used: 
    - "pcap": 2980
    - "smbd": 173
    - "mysqld": 50
    - "SipSession": 176
    - "SipCall": 67
    - "epmapper": 2
    - "mssqld": 2
    - "ftpd": 2
    - "microsoft-ds": 3
    - "RtpUdpStream": 2
    - "TftpServerHandler": 2
  - Ports used:
    - 8088 (908 times)
    - 5060 (228 times)
    - 23 (124 times)
    - 445 (97 times)
    - 80 (52 times)
  - Countries 
    - ![United States](US.png "United States") 1724
    - ![Great Britain](GB.png "Great Britain") 718
    - ![Vietnam](VN.png "Vietnam") 718
    - ![Ukraine](UA.png "Ukraine") 359
    - ![India](IN.png "India") 71
  
* Any unresolved questions raised by the data collected
    
## Assets

List any additional assets, such as scripts or files

## Resources

- [Modern Honeypot Network GitHub](https://github.com/threatstream/mhn/)

## Notes

Describe any challenges encountered while doing the work:
- Figure out how to fix broken installation scripts

## License

    Copyright [2018] [James Wong]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
