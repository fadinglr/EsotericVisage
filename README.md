# EsotericVisage
Stealth remote administration tool 
```python
+-------+
| Local |
+-------+

[EV-Installer] --+
                 | - Determine if AVs are running
                 |
                 | - DLL inject into explorer.exe
                 |
                 | - Else: extract dll and run using rundll32.exe
                 |
                 | - Set registry keys and delete installer...
+---------+      
| Network | 
+---------+              
           
[EV-Core] --+ 
            |    Use sendMessage and getUpdates for c&c
            |                     | 
            +--------------api.telegram.org-------------Telegram client
```