####################################################################################
####################################################################################
## Copyright 2011(c) Analog Devices, Inc.
## Auto-generated, do not modify!
####################################################################################
####################################################################################

M_DEPS += system_top.v
M_DEPS += system_project.tcl
M_DEPS += system_constr.xdc
M_DEPS += system_bd.tcl
M_DEPS += ../common/fmcadc2_spi.v
M_DEPS += ../common/fmcadc2_bd.tcl
M_DEPS += ../../scripts/adi_project.tcl
M_DEPS += ../../scripts/adi_env.tcl
M_DEPS += ../../scripts/adi_board.tcl
M_DEPS += ../../common/xilinx/sys_adcfifo.tcl
M_DEPS += ../../common/vc707/vc707_system_mig.prj
M_DEPS += ../../common/vc707/vc707_system_constr.xdc
M_DEPS += ../../common/vc707/vc707_system_bd.tcl
M_DEPS += ../../../library/xilinx/common/ad_iobuf.v
M_DEPS += ../../../library/common/ad_sysref_gen.v
M_DEPS += ../../../library/axi_ad9625/axi_ad9625.xpr
M_DEPS += ../../../library/xilinx/axi_adxcvr/axi_adxcvr.xpr
M_DEPS += ../../../library/axi_dmac/axi_dmac.xpr
M_DEPS += ../../../library/util_adcfifo/util_adcfifo.xpr
M_DEPS += ../../../library/xilinx/util_adxcvr/util_adxcvr.xpr

M_VIVADO := vivado -mode batch -source

M_FLIST := *.cache
M_FLIST += *.data
M_FLIST += *.xpr
M_FLIST += *.log
M_FLIST += *.jou
M_FLIST +=  xgui
M_FLIST += *.runs
M_FLIST += *.srcs
M_FLIST += *.sdk
M_FLIST += *.hw
M_FLIST += *.sim
M_FLIST += .Xil
M_FLIST += *.ip_user_files



.PHONY: all lib clean clean-all
all: lib fmcadc2_vc707.sdk/system_top.hdf


clean: 
	rm -rf $(M_FLIST)


clean-all:clean
	make -C ../../../library/axi_ad9625 clean
	make -C ../../../library/xilinx/axi_adxcvr clean
	make -C ../../../library/axi_dmac clean
	make -C ../../../library/util_adcfifo clean
	make -C ../../../library/xilinx/util_adxcvr clean


fmcadc2_vc707.sdk/system_top.hdf: $(M_DEPS)
	-rm -rf $(M_FLIST)
	$(M_VIVADO) system_project.tcl >> fmcadc2_vc707_vivado.log 2>&1


lib:
	make -C ../../../library/axi_ad9625
	make -C ../../../library/xilinx/axi_adxcvr
	make -C ../../../library/axi_dmac
	make -C ../../../library/util_adcfifo
	make -C ../../../library/xilinx/util_adxcvr

####################################################################################
####################################################################################
