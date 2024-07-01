# Privileged  Exec Mode 
- Move from user Exec Mode to Priviliged Exec Mode 
```bash
Switch > enable 
```

# Global Exec Mode 
- To move in and out of global configuration mode, use the configure terminal command. To return to privilege EXEC mode, use the exit command
```bash
Switch(config) #
Switch(config) # exit
```

# Line Configuration Mode 
- To move in and out of line configuration mode, use the line command followed by the management line type. To return to global configuration mode, use the exit command.
```bash
Switch(config)# line console 0
Switch(config-line)# exit 
Switch(config)# 
```

# Subconfiguration Mode 
-  To move out of any subconfiguration mode to get back to global configuration mode, use the exit command. To return to privilege EXEC mode, use the end command or key combination Ctrl +Z.
```bash
Switch(config)# line console 0 
Switch(config-line)# end
Switch(config)
```
