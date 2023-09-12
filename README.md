# XTor Klipper Macros

## First
- Open SSH
- Login
- Copy this
  
```command
cd ~/printer_data/config
git clone https://github.com/LastuvkaLukas/xtor_klipper_macros XTOR
```

- Open your klipper config
- Get `XTOR`/`user_variable.cfg`
- Copy `#[gcode_macro _XTOR_VARIABLE]`
- Paste to `printer.cfg`
- Set your variables

## Update
- Open SSH
- Login
- Copy this
  
```command
cd ~/printer_data/config/XTOR
git pull
```
