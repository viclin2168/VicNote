![[Pasted image 20241211170333.png]]

![[Pasted image 20241211164644.png]]

==**extra rom file to jbf**==
 w5img.exe extract 1021_faf4a247_osdpkg_lensModel_noOSD 1021\

==jbf to json==
python table2json.py -s syscfg_spec_1.10.json -t table_0x140000.jbf -j table_0x140000.json  in C:\project_others\ponstone\kenny\Phase 3\Customer\PenstoneStep3_FirmwareToolRelease\bin