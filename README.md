# XTor Klipper Macros

## First
- Open SSH
- Login
- Copy this
  
```command
cd ~/printer_data/config
git clone -n --depth=1 --filter=tree:0 https://github.com/XTorLukas/xtor_klipper_macros.git XTOR
cd XTOR
git sparse-checkout set --no-cone macros
git checkout
```

- Open your klipper config
- Get `XTOR`/`macros`/`var`/`user_variable.cfg`
- Copy `#[gcode_macro _XTOR_VARIABLE]`
- Paste to `printer.cfg`
- Set your variables

## Update via Moonraker
- Open your `moonraker.cfg`
- Copy this
  
```command
[update_manager XTOR]
type: git_repo
primary_branch: master
path: ~/printer_data/config/XTOR
origin: https://github.com/XTorLukas/xtor_klipper_macros.git
managed_services: klipper
```
