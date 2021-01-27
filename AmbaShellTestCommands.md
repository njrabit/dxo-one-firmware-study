AmbaShell Test Command [Version 1.0.0000]

(C) Copyright 2004-2014 Ambarella Corp.

supported test commands:

* 3rddenoise
* app_fatal
* batt
* cal
* charge
* chk_low_spd

Usage: sd_shmoo mode [uhs] [huge_file] [show_reg]
Usage: sd_shmoo [slot] all
Usage: sd_shmoo [slot] [all_str|3mA|6mA|12mA|18mA|] [set|all_dly] [8 delay value]
 uhs(1/0) - set 1(default) to check uhs mode
 huge_file(1/0) - set 1(default) to access huge file size
 show_reg(0/1) - set 1 to show reg value of delay ctrl (default 0)
 all - test all the driving strength & all the delay ctrl settings
 all_str - test all the driving strength
 3mA|6mA|12mA|18mA - choose one of driving strength
 all_dly - test all the delay ctrl settings

 Example : t sd_shmoo c 12mA all_dly

 set - set 8 delay ctrl settings of start(0-7) & count(1-8) as following order:
 [data_output_delay_start data_output_delay_count data_input_delay_start data_input_delay_count]
 [clk_output_delay_start clk_output_delay_count clk_input_delay_start clk_input_delay_count]

 Example : t sd_shmoo c 12mA set 0 1 1 1 1 1 0 8

Usage: chk_low_spd [slot] [bs] [ms] [lim] [mode]
  bs is an option means block size of each write.
  ms is an option means each sampiling time.
  lim is an option means the lowest write speed in Mbs.
  mode is an option [phy] means phyical access

* clbt
* clbt-off
* dbgcap
* ddr
* ds
* dsp
* dxo
* eng-mode
* ff
* fioprf_randvrfy

Usage: fioprf_randvrfy [slot] [size] [all|times] [delay] [keep]
  size is an option means to the test file size.
  all is an option means to test with all free space
  times means how many files will be tested
  delay is an option means ms delay after each file
  keep is an option means to keep files after test

* fioprf_thruput

Usage: fioprf_thruput [slot]
Usage: fioprf_thruput [slot] [bs]
Usage: fioprf_thruput [slot] [bs] [areas]
Usage: fioprf_thruput [slot] [bs] [align] [size]
Usage: fioprf_thruput [slot] [multi] [num] [bs1] [bs2] ...
Usage: fioprf_thruput [slot] one [fsize]
Usage: fioprf_thruput [slot] rand_write [fsize]
Where
  bs is an option that means block size
  areas is an option that means number of areas in all free space
  one is for 1-file sequential access with continous space test
  rand_write is for 2-file random access with continous space test
  fsize is the file size of MB to create continous space (20 as default)

* frm
* gdma
* gms
* gpio
* gs
* hdmi
* help
* i2c
* img
* imgproc
* lens
* p
* profile
* pwc
* remote
* sd

valid test targets for SD are:
	clkon
	clkoff
	rs
	ws
	max_freq
	parse
	timeout
	erase
	ds
	cmd11
	dump_reg

* sd_shmoo

Usage: sd_shmoo mode [uhs] [huge_file] [show_reg]
Usage: sd_shmoo [slot] all
Usage: sd_shmoo [slot] [all_str|3mA|6mA|12mA|18mA|] [set|all_dly] [8 delay value]
 uhs(1/0) - set 1(default) to check uhs mode
 huge_file(1/0) - set 1(default) to access huge file size
 show_reg(0/1) - set 1 to show reg value of delay ctrl (default 0)
 all - test all the driving strength & all the delay ctrl settings
 all_str - test all the driving strength
 3mA|6mA|12mA|18mA - choose one of driving strength
 all_dly - test all the delay ctrl settings

 Example : t sd_shmoo c 12mA all_dly

 set - set 8 delay ctrl settings of start(0-7) & count(1-8) as following order:
 [data_output_delay_start data_output_delay_count data_input_delay_start data_input_delay_count]
 [clk_output_delay_start clk_output_delay_count clk_input_delay_start clk_input_delay_count]

 Example : t sd_shmoo c 12mA set 0 1 1 1 1 1 0 8

* sevt
* spi
* svc
* syslog
* t
* test-box-sn
* test-mode
* timer
* trace
* tunable
* up
* usb
* usb
* vtuner
* wifi
* xapp_fatal
* xbatt
* xcharge
* xclbt
* xclbt-off
* xds
* xeng-mode
* xff
* xgms
* xgs
* xlens
* xremote
* xtest-box-sn
* xtest-mode
* xup
* xusb
* xwifi
