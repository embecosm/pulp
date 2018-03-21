#
# Copyright (C) 2016-2018 Embecosm Limited
# All rights reserved.
#
# This software may be modified and distributed under the terms
# of the BSD license.  See the LICENSE file for details.
#

# paths
mkfile_path := $(dir $(abspath $(firstword $(MAKEFILE_LIST))))

IPS_PATH=$(mkfile_path)../ips
RTL_PATH=$(mkfile_path)../rtl
TB_PATH=$(mkfile_path)../tb

L2_TCDM_HYBRID_INTERCO_IP=$(IPS_PATH)/L2_tcdm_hybrid_interco/RTL
ADV_DBG_IF_IP=$(IPS_PATH)/adv_dbg_if/rtl
APB2PER_IP=$(IPS_PATH)/apb/apb2per
APB_ADV_TIMER_IP=$(IPS_PATH)/apb/apb_adv_timer
APB_FLL_IF_IP=$(IPS_PATH)/apb/apb_fll_if
APB_GPIO_IP=$(IPS_PATH)/apb/apb_gpio
APB_NODE_IP=$(IPS_PATH)/apb/apb_node
APB_INTERRUPT_CNTRL_IP=$(IPS_PATH)/apb_interrupt_cntrl
AXI_NODE_IP=$(IPS_PATH)/axi/axi_node
AXI_SLICE_IP=$(IPS_PATH)/axi/axi_slice
AXI_SLICE_DC_IP=$(IPS_PATH)/axi/axi_slice_dc
TIMER_UNIT_IP=$(IPS_PATH)/timer_unit
COMMON_CELLS_IP=$(IPS_PATH)/common_cells
FPU_IP=$(IPS_PATH)/fpu/hdl
JTAG_PULP_IP=$(IPS_PATH)/jtag_pulp
RISCV_IP=$(IPS_PATH)/riscv
ZERO_RISCY_IP=$(IPS_PATH)/zero-riscy
SCM_IP=$(IPS_PATH)/scm/latch_scm
TECH_CELLS_GENERIC_IP=$(IPS_PATH)/tech_cells_generic
UDMA_CORE_IP=$(IPS_PATH)/udma/udma_core/rtl
UDMA_UART_IP=$(IPS_PATH)/udma/udma_uart/rtl
UDMA_I2C_IP=$(IPS_PATH)/udma/udma_i2c/rtl
UDMA_I2S_IP=$(IPS_PATH)/udma/udma_i2s/rtl
UDMA_QSPI_IP=$(IPS_PATH)/udma/udma_qspi/rtl
UDMA_SDIO_IP=$(IPS_PATH)/udma/udma_sdio/rtl
UDMA_CAMERA_IP=$(IPS_PATH)/udma/udma_camera/rtl
HWPE_CTRL_IP=$(IPS_PATH)/hwpe-ctrl/rtl
HWPE_STREAM_IP=$(IPS_PATH)/hwpe-stream/rtl
HWPE_MAC_ENGINE_IP=$(IPS_PATH)/hwpe-mac-engine
PULP_SOC_IP=$(IPS_PATH)/pulp_soc/rtl/pulp_soc
AXI2MEM_IP=$(IPS_PATH)/axi/axi2mem
AXI2PER_IP=$(IPS_PATH)/axi/axi2per
PER2AXI_IP=$(IPS_PATH)/axi/per2axi
AXI_SIZE_CONV_IP=$(IPS_PATH)/axi/axi_size_conv
CLUSTER_INTERCONNECT_IP=$(IPS_PATH)/cluster_interconnect/rtl/low_latency_interco
EVENT_UNIT_FLEX_IP=$(IPS_PATH)/event_unit_flex
MCHAN_IP=$(IPS_PATH)/mchan
ICACHE_INTC_IP=$(IPS_PATH)/icache-intc
ICACHE_MP_128_PF_IP=$(IPS_PATH)/icache_mp_128_pf/RTL
CLUSTER_PERIPHERALS_IP=$(IPS_PATH)/cluster_peripherals
PULP_CLUSTER_IP=$(IPS_PATH)/pulp_cluster

IP_SRC=$(L2_TCDM_HYBRID_INTERCO_IP)/l2_tcdm_demux.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/lint_2_apb.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/lint_2_axi.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/axi_2_lint/axi64_2_lint32.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/axi_2_lint/axi_read_ctrl.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/axi_2_lint/axi_write_ctrl.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/axi_2_lint/lint64_to_32.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/AddressDecoder_Req_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/AddressDecoder_Resp_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/ArbitrationTree_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/FanInPrimitive_Req_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/FanInPrimitive_Resp_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/MUX2_REQ_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/RequestBlock_L2_1CH.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/RequestBlock_L2_2CH.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/ResponseBlock_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/ResponseTree_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/RR_Flag_Req_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_L2/XBAR_L2.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/AddressDecoder_Req_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/AddressDecoder_Resp_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/ArbitrationTree_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/FanInPrimitive_Req_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/FanInPrimitive_Resp_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/MUX2_REQ_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/RequestBlock1CH_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/RequestBlock2CH_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/ResponseBlock_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/ResponseTree_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/RR_Flag_Req_BRIDGE.sv\
       $(L2_TCDM_HYBRID_INTERCO_IP)/XBAR_BRIDGE/XBAR_BRIDGE.sv\
       $(ADV_DBG_IF_IP)/adbg_axi_biu.sv\
       $(ADV_DBG_IF_IP)/adbg_axi_module.sv\
       $(ADV_DBG_IF_IP)/adbg_lint_biu.sv\
       $(ADV_DBG_IF_IP)/adbg_lint_module.sv\
       $(ADV_DBG_IF_IP)/adbg_crc32.v\
       $(ADV_DBG_IF_IP)/adbg_or1k_biu.sv\
       $(ADV_DBG_IF_IP)/adbg_or1k_module.sv\
       $(ADV_DBG_IF_IP)/adbg_or1k_status_reg.sv\
       $(ADV_DBG_IF_IP)/adbg_top.sv\
       $(ADV_DBG_IF_IP)/bytefifo.v\
       $(ADV_DBG_IF_IP)/syncflop.v\
       $(ADV_DBG_IF_IP)/syncreg.v\
       $(ADV_DBG_IF_IP)/adbg_tap_top.v\
       $(ADV_DBG_IF_IP)/adv_dbg_if.sv\
       $(ADV_DBG_IF_IP)/adbg_axionly_top.sv\
       $(ADV_DBG_IF_IP)/adbg_lintonly_top.sv\
       $(APB2PER_IP)/apb2per.sv\
       $(APB_ADV_TIMER_IP)/adv_timer_apb_if.sv\
       $(APB_ADV_TIMER_IP)/comparator.sv\
       $(APB_ADV_TIMER_IP)/lut_4x4.sv\
       $(APB_ADV_TIMER_IP)/out_filter.sv\
       $(APB_ADV_TIMER_IP)/up_down_counter.sv\
       $(APB_ADV_TIMER_IP)/input_stage.sv\
       $(APB_ADV_TIMER_IP)/prescaler.sv\
       $(APB_ADV_TIMER_IP)/apb_adv_timer.sv\
       $(APB_ADV_TIMER_IP)/timer_cntrl.sv\
       $(APB_ADV_TIMER_IP)/timer_module.sv\
       $(APB_FLL_IF_IP)/apb_fll_if.sv\
       $(APB_GPIO_IP)/apb_gpio.sv\
       $(APB_NODE_IP)/apb_node.sv\
       $(APB_NODE_IP)/apb_node_wrap.sv\
       $(APB_INTERRUPT_CNTRL_IP)/apb_interrupt_cntrl.sv\
       $(AXI_NODE_IP)/apb_regs_top.sv\
       $(AXI_NODE_IP)/axi_address_decoder_AR.sv\
       $(AXI_NODE_IP)/axi_address_decoder_AW.sv\
       $(AXI_NODE_IP)/axi_address_decoder_BR.sv\
       $(AXI_NODE_IP)/axi_address_decoder_BW.sv\
       $(AXI_NODE_IP)/axi_address_decoder_DW.sv\
       $(AXI_NODE_IP)/axi_AR_allocator.sv\
       $(AXI_NODE_IP)/axi_ArbitrationTree.sv\
       $(AXI_NODE_IP)/axi_AW_allocator.sv\
       $(AXI_NODE_IP)/axi_BR_allocator.sv\
       $(AXI_NODE_IP)/axi_BW_allocator.sv\
       $(AXI_NODE_IP)/axi_DW_allocator.sv\
       $(AXI_NODE_IP)/axi_FanInPrimitive_Req.sv\
       $(AXI_NODE_IP)/axi_multiplexer.sv\
       $(AXI_NODE_IP)/axi_node.sv\
       $(AXI_NODE_IP)/axi_node_wrap.sv\
       $(AXI_NODE_IP)/axi_node_wrap_with_slices.sv\
       $(AXI_NODE_IP)/axi_regs_top.sv\
       $(AXI_NODE_IP)/axi_request_block.sv\
       $(AXI_NODE_IP)/axi_response_block.sv\
       $(AXI_NODE_IP)/axi_RR_Flag_Req.sv\
       $(AXI_SLICE_IP)/axi_ar_buffer.sv\
       $(AXI_SLICE_IP)/axi_aw_buffer.sv\
       $(AXI_SLICE_IP)/axi_b_buffer.sv\
       $(AXI_SLICE_IP)/axi_buffer.sv\
       $(AXI_SLICE_IP)/axi_r_buffer.sv\
       $(AXI_SLICE_IP)/axi_slice.sv\
       $(AXI_SLICE_IP)/axi_w_buffer.sv\
       $(AXI_SLICE_IP)/axi_slice_wrap.sv\
       $(AXI_SLICE_DC_IP)/axi_slice_dc_master.sv\
       $(AXI_SLICE_DC_IP)/axi_slice_dc_slave.sv\
       $(AXI_SLICE_DC_IP)/dc_data_buffer.sv\
       $(AXI_SLICE_DC_IP)/dc_full_detector.v\
       $(AXI_SLICE_DC_IP)/dc_synchronizer.v\
       $(AXI_SLICE_DC_IP)/dc_token_ring_fifo_din.v\
       $(AXI_SLICE_DC_IP)/dc_token_ring_fifo_dout.v\
       $(AXI_SLICE_DC_IP)/dc_token_ring.v\
       $(AXI_SLICE_DC_IP)/axi_slice_dc_master_wrap.sv\
       $(AXI_SLICE_DC_IP)/axi_slice_dc_slave_wrap.sv\
       $(AXI_SLICE_DC_IP)/axi_cdc.sv\
       $(TIMER_UNIT_IP)/timer_unit.sv\
       $(TIMER_UNIT_IP)/timer_unit_counter.sv\
       $(TIMER_UNIT_IP)/timer_unit_counter_presc.sv\
       $(COMMON_CELLS_IP)/generic_fifo.sv\
       $(COMMON_CELLS_IP)/generic_LFSR_8bit.sv\
       $(COMMON_CELLS_IP)/onehot_to_bin.sv\
       $(COMMON_CELLS_IP)/rstgen.sv\
       $(COMMON_CELLS_IP)/edge_propagator_tx.sv\
       $(COMMON_CELLS_IP)/edge_propagator_rx.sv\
       $(COMMON_CELLS_IP)/edge_propagator.sv\
       $(COMMON_CELLS_IP)/pulp_sync_wedge.sv\
       $(COMMON_CELLS_IP)/pulp_sync.sv\
       $(COMMON_CELLS_IP)/clock_divider.sv\
       $(COMMON_CELLS_IP)/clock_divider_counter.sv\
       $(FPU_IP)/fpu_utils/fpu_ff.sv\
       $(FPU_IP)/fpu_v0.1/fpu_defs.sv\
       $(FPU_IP)/fpu_v0.1/fpexc.sv\
       $(FPU_IP)/fpu_v0.1/fpu_add.sv\
       $(FPU_IP)/fpu_v0.1/fpu_core.sv\
       $(FPU_IP)/fpu_v0.1/fpu_ftoi.sv\
       $(FPU_IP)/fpu_v0.1/fpu_itof.sv\
       $(FPU_IP)/fpu_v0.1/fpu_mult.sv\
       $(FPU_IP)/fpu_v0.1/fpu_norm.sv\
       $(FPU_IP)/fpu_v0.1/fpu_private.sv\
       $(FPU_IP)/fpu_v0.1/riscv_fpu.sv\
       $(FPU_IP)/fpu_v0.1/fp_fma_wrapper.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/fpu_defs_div_sqrt_tp.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/control_tp.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/fpu_norm_div_sqrt.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/iteration_div_sqrt_first.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/iteration_div_sqrt.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/nrbd_nrsc_tp.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/preprocess.sv\
       $(FPU_IP)/fpu_div_sqrt_tp_nlp/div_sqrt_top_tp.sv\
       $(FPU_IP)/fpu_fmac/fpu_defs_fmac.sv\
       $(FPU_IP)/fpu_fmac/preprocess_fmac.sv\
       $(FPU_IP)/fpu_fmac/booth_encoder.sv\
       $(FPU_IP)/fpu_fmac/booth_selector.sv\
       $(FPU_IP)/fpu_fmac/pp_generation.sv\
       $(FPU_IP)/fpu_fmac/wallace.sv\
       $(FPU_IP)/fpu_fmac/aligner.sv\
       $(FPU_IP)/fpu_fmac/CSA.sv\
       $(FPU_IP)/fpu_fmac/adders.sv\
       $(FPU_IP)/fpu_fmac/LZA.sv\
       $(FPU_IP)/fpu_fmac/fpu_norm_fmac.sv\
       $(FPU_IP)/fpu_fmac/fmac.sv\
       $(JTAG_PULP_IP)/src/bscell.sv\
       $(JTAG_PULP_IP)/src/jtag_axi_wrap.sv\
       $(JTAG_PULP_IP)/src/jtag_enable.sv\
       $(JTAG_PULP_IP)/src/jtag_enable_synch.sv\
       $(JTAG_PULP_IP)/src/jtagreg.sv\
       $(JTAG_PULP_IP)/src/jtag_rst_synch.sv\
       $(JTAG_PULP_IP)/src/jtag_sync.sv\
       $(JTAG_PULP_IP)/src/tap_top.v\
       $(RISCV_IP)/include/apu_core_package.sv\
       $(RISCV_IP)/include/riscv_defines.sv\
       $(RISCV_IP)/include/riscv_tracer_defines.sv\
       $(RISCV_IP)/riscv_alu.sv\
       $(RISCV_IP)/riscv_alu_basic.sv\
       $(RISCV_IP)/riscv_alu_div.sv\
       $(RISCV_IP)/riscv_compressed_decoder.sv\
       $(RISCV_IP)/riscv_controller.sv\
       $(RISCV_IP)/riscv_cs_registers.sv\
       $(RISCV_IP)/riscv_debug_unit.sv\
       $(RISCV_IP)/riscv_decoder.sv\
       $(RISCV_IP)/riscv_int_controller.sv\
       $(RISCV_IP)/riscv_ex_stage.sv\
       $(RISCV_IP)/riscv_hwloop_controller.sv\
       $(RISCV_IP)/riscv_hwloop_regs.sv\
       $(RISCV_IP)/riscv_id_stage.sv\
       $(RISCV_IP)/riscv_if_stage.sv\
       $(RISCV_IP)/riscv_load_store_unit.sv\
       $(RISCV_IP)/riscv_mult.sv\
       $(RISCV_IP)/riscv_prefetch_buffer.sv\
       $(RISCV_IP)/riscv_prefetch_L0_buffer.sv\
       $(RISCV_IP)/riscv_core.sv\
       $(RISCV_IP)/riscv_apu_disp.sv\
       $(RISCV_IP)/riscv_fetch_fifo.sv\
       $(RISCV_IP)/riscv_L0_buffer.sv\
       $(ZERO_RISCY_IP)/include/zeroriscy_defines.sv\
       $(ZERO_RISCY_IP)/include/zeroriscy_tracer_defines.sv\
       $(ZERO_RISCY_IP)/zeroriscy_alu.sv\
       $(ZERO_RISCY_IP)/zeroriscy_compressed_decoder.sv\
       $(ZERO_RISCY_IP)/zeroriscy_controller.sv\
       $(ZERO_RISCY_IP)/zeroriscy_cs_registers.sv\
       $(ZERO_RISCY_IP)/zeroriscy_debug_unit.sv\
       $(ZERO_RISCY_IP)/zeroriscy_decoder.sv\
       $(ZERO_RISCY_IP)/zeroriscy_int_controller.sv\
       $(ZERO_RISCY_IP)/zeroriscy_ex_block.sv\
       $(ZERO_RISCY_IP)/zeroriscy_id_stage.sv\
       $(ZERO_RISCY_IP)/zeroriscy_if_stage.sv\
       $(ZERO_RISCY_IP)/zeroriscy_load_store_unit.sv\
       $(ZERO_RISCY_IP)/zeroriscy_multdiv_slow.sv\
       $(ZERO_RISCY_IP)/zeroriscy_multdiv_fast.sv\
       $(ZERO_RISCY_IP)/zeroriscy_prefetch_buffer.sv\
       $(ZERO_RISCY_IP)/zeroriscy_fetch_fifo.sv\
       $(ZERO_RISCY_IP)/zeroriscy_core.sv\
       $(SCM_IP)/register_file_1r_1w_test_wrap.sv\
       $(SCM_IP)/register_file_1w_64b_multi_port_read_32b_1row.sv\
       $(SCM_IP)/register_file_1w_multi_port_read_1row.sv\
       $(SCM_IP)/register_file_1r_1w_all.sv\
       $(SCM_IP)/register_file_1r_1w_all_test_wrap.sv\
       $(SCM_IP)/register_file_1r_1w_be.sv\
       $(SCM_IP)/register_file_1r_1w.sv\
       $(SCM_IP)/register_file_1r_1w_1row.sv\
       $(SCM_IP)/register_file_1w_128b_multi_port_read_32b.sv\
       $(SCM_IP)/register_file_1w_64b_multi_port_read_32b.sv\
       $(SCM_IP)/register_file_1w_64b_1r_32b.sv\
       $(SCM_IP)/register_file_1w_multi_port_read_be.sv\
       $(SCM_IP)/register_file_1w_multi_port_read.sv\
       $(SCM_IP)/register_file_2r_1w_asymm.sv\
       $(SCM_IP)/register_file_2r_1w_asymm_test_wrap.sv\
       $(SCM_IP)/register_file_2r_2w.sv\
       $(SCM_IP)/register_file_3r_2w.sv\
       $(SCM_IP)/register_file_3r_2w_be.sv\
       $(SCM_IP)/register_file_multi_way_1w_64b_multi_port_read_32b.sv\
       $(SCM_IP)/register_file_multi_way_1w_multi_port_read.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_clock_gating.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_clock_gating.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_clock_mux2.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_clock_buffer.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_clock_inverter.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_clock_xor2.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_buffer.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_level_shifter_in.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_level_shifter_in_clamp.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_level_shifter_out.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_level_shifter_out_clamp.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_clock_and2.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_clock_buffer.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_clock_inverter.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_clock_mux2.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_clock_xor2.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_level_shifter_in.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_level_shifter_in_clamp.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_level_shifter_out.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_level_shifter_out_clamp.sv\
       $(TECH_CELLS_GENERIC_IP)/cluster_clock_and2.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_clock_gating_async.sv\
       $(TECH_CELLS_GENERIC_IP)/pulp_power_gating.sv\
       $(TECH_CELLS_GENERIC_IP)/generic_rom.sv\
       $(TECH_CELLS_GENERIC_IP)/generic_memory.sv\
       $(TECH_CELLS_GENERIC_IP)/pad_functional.sv\
       $(UDMA_CORE_IP)/core/udma_ch_addrgen.sv\
       $(UDMA_CORE_IP)/core/udma_filter_au.sv\
       $(UDMA_CORE_IP)/core/udma_filter_bincu.sv\
       $(UDMA_CORE_IP)/core/udma_filter_rx_dataout.sv\
       $(UDMA_CORE_IP)/core/udma_filter.sv\
       $(UDMA_CORE_IP)/core/udma_filter_tx_datafetch.sv\
       $(UDMA_CORE_IP)/core/udma_arbiter.sv\
       $(UDMA_CORE_IP)/core/udma_core.sv\
       $(UDMA_CORE_IP)/core/udma_rx_channels.sv\
       $(UDMA_CORE_IP)/core/udma_tx_channels.sv\
       $(UDMA_CORE_IP)/common/udma_ctrl.sv\
       $(UDMA_CORE_IP)/common/udma_apb_if.sv\
       $(UDMA_CORE_IP)/common/io_clk_gen.sv\
       $(UDMA_CORE_IP)/common/io_event_counter.sv\
       $(UDMA_CORE_IP)/common/io_generic_fifo.sv\
       $(UDMA_CORE_IP)/common/io_tx_fifo.sv\
       $(UDMA_CORE_IP)/common/io_tx_fifo_mark.sv\
       $(UDMA_CORE_IP)/common/io_tx_fifo_dc.sv\
       $(UDMA_CORE_IP)/common/io_shiftreg.sv\
       $(UDMA_CORE_IP)/common/udma_dc_fifo.sv\
       $(UDMA_CORE_IP)/common/udma_clkgen.sv\
       $(UDMA_CORE_IP)/common/udma_clk_div_cnt.sv\
       $(UDMA_UART_IP)/udma_uart_reg_if.sv\
       $(UDMA_UART_IP)/udma_uart_top.sv\
       $(UDMA_UART_IP)/udma_uart_rx.sv\
       $(UDMA_UART_IP)/udma_uart_tx.sv\
       $(UDMA_I2C_IP)/udma_i2c_reg_if.sv\
       $(UDMA_I2C_IP)/udma_i2c_bus_ctrl.sv\
       $(UDMA_I2C_IP)/udma_i2c_control.sv\
       $(UDMA_I2S_IP)/i2s_clk_gen.sv\
       $(UDMA_I2S_IP)/i2s_rx_channel.sv\
       $(UDMA_I2S_IP)/i2s_ws_gen.sv\
       $(UDMA_I2S_IP)/cic_top.sv\
       $(UDMA_I2S_IP)/cic_integrator.sv\
       $(UDMA_I2S_IP)/cic_comb.sv\
       $(UDMA_I2S_IP)/udma_i2s_multich.sv\
       $(UDMA_I2S_IP)/udma_i2s_2ch.sv\
       $(UDMA_I2S_IP)/udma_i2s_reg_if.sv\
       $(UDMA_QSPI_IP)/udma_spim_reg_if.sv\
       $(UDMA_QSPI_IP)/udma_spim_ctrl.sv\
       $(UDMA_QSPI_IP)/udma_spim_txrx.sv\
       $(UDMA_QSPI_IP)/udma_spim_top.sv\
       $(UDMA_SDIO_IP)/sdio_crc7.sv\
       $(UDMA_SDIO_IP)/sdio_crc16.sv\
       $(UDMA_SDIO_IP)/sdio_txrx_cmd.sv\
       $(UDMA_SDIO_IP)/sdio_txrx_data.sv\
       $(UDMA_SDIO_IP)/sdio_txrx.sv\
       $(UDMA_SDIO_IP)/udma_sdio_reg_if.sv\
       $(UDMA_SDIO_IP)/udma_sdio_top.sv\
       $(UDMA_CAMERA_IP)/camera_reg_if.sv\
       $(UDMA_CAMERA_IP)/camera_if.sv\
       $(HWPE_CTRL_IP)/hwpe_ctrl_package.sv\
       $(HWPE_CTRL_IP)/hwpe_ctrl_interfaces.sv\
       $(HWPE_CTRL_IP)/hwpe_ctrl_regfile.sv\
       $(HWPE_CTRL_IP)/hwpe_ctrl_regfile_latch.sv\
       $(HWPE_CTRL_IP)/hwpe_ctrl_slave.sv\
       $(HWPE_CTRL_IP)/hwpe_ctrl_seq_mult.sv\
       $(HWPE_CTRL_IP)/hwpe_ctrl_ucode.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_package.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_interfaces.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_addressgen.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_fifo_earlystall_sidech.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_fifo_earlystall.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_fifo_scm.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_fifo_sidech.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_fifo.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_buffer.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_merge.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_split.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_sink.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_source.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_sink_realign.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_source_realign.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_mux_static.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_demux_static.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_tcdm_fifo_load.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_tcdm_fifo_store.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_tcdm_mux.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_tcdm_mux_static.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_tcdm_reorder.sv\
       $(HWPE_STREAM_IP)/hwpe_stream_tcdm_reorder_static.sv\
       $(HWPE_MAC_ENGINE_IP)/rtl/mac_package.sv\
       $(HWPE_MAC_ENGINE_IP)/rtl/mac_fsm.sv\
       $(HWPE_MAC_ENGINE_IP)/rtl/mac_ctrl.sv\
       $(HWPE_MAC_ENGINE_IP)/rtl/mac_streamer.sv\
       $(HWPE_MAC_ENGINE_IP)/rtl/mac_engine.sv\
       $(HWPE_MAC_ENGINE_IP)/rtl/mac_top.sv\
       $(HWPE_MAC_ENGINE_IP)/wrap/mac_top_wrap.sv\
       $(PULP_SOC_IP)/soc_interconnect.sv\
       $(PULP_SOC_IP)/boot_rom.sv\
       $(PULP_SOC_IP)/l2_ram_multi_bank.sv\
       $(PULP_SOC_IP)/lint_jtag_wrap.sv\
       $(PULP_SOC_IP)/periph_bus_wrap.sv\
       $(PULP_SOC_IP)/soc_clk_rst_gen.sv\
       $(PULP_SOC_IP)/soc_event_arbiter.sv\
       $(PULP_SOC_IP)/soc_event_generator.sv\
       $(PULP_SOC_IP)/soc_event_queue.sv\
       $(PULP_SOC_IP)/soc_interconnect_wrap.sv\
       $(PULP_SOC_IP)/soc_peripherals.sv\
       $(PULP_SOC_IP)/pulp_soc.sv\
       $(AXI2MEM_IP)/axi2mem_busy_unit.sv\
       $(AXI2MEM_IP)/axi2mem_rd_channel.sv\
       $(AXI2MEM_IP)/axi2mem.sv\
       $(AXI2MEM_IP)/axi2mem_tcdm_rd_if.sv\
       $(AXI2MEM_IP)/axi2mem_tcdm_synch.sv\
       $(AXI2MEM_IP)/axi2mem_tcdm_unit.sv\
       $(AXI2MEM_IP)/axi2mem_tcdm_wr_if.sv\
       $(AXI2MEM_IP)/axi2mem_trans_unit.sv\
       $(AXI2MEM_IP)/axi2mem_wr_channel.sv\
       $(AXI2PER_IP)/axi2per_req_channel.sv\
       $(AXI2PER_IP)/axi2per_res_channel.sv\
       $(AXI2PER_IP)/axi2per.sv\
       $(PER2AXI_IP)/per2axi_busy_unit.sv\
       $(PER2AXI_IP)/per2axi_req_channel.sv\
       $(PER2AXI_IP)/per2axi_res_channel.sv\
       $(PER2AXI_IP)/per2axi.sv\
       $(AXI_SIZE_CONV_IP)/AXI_UPSIZE_simple/axi_size_UPSIZE_32_64.sv\
       $(AXI_SIZE_CONV_IP)/AXI_UPSIZE_simple/axi_size_UPSIZE_32_64_wrap.sv\
       $(AXI_SIZE_CONV_IP)/AXI_UPSIZE/Write_UPSIZE.sv\
       $(CLUSTER_INTERCONNECT_IP)/FanInPrimitive_Req.sv\
       $(CLUSTER_INTERCONNECT_IP)/ArbitrationTree.sv\
       $(CLUSTER_INTERCONNECT_IP)/MUX2_REQ.sv\
       $(CLUSTER_INTERCONNECT_IP)/AddressDecoder_Resp.sv\
       $(CLUSTER_INTERCONNECT_IP)/TestAndSet.sv\
       $(CLUSTER_INTERCONNECT_IP)/RequestBlock2CH.sv\
       $(CLUSTER_INTERCONNECT_IP)/RequestBlock1CH.sv\
       $(CLUSTER_INTERCONNECT_IP)/FanInPrimitive_Resp.sv\
       $(CLUSTER_INTERCONNECT_IP)/ResponseTree.sv\
       $(CLUSTER_INTERCONNECT_IP)/ResponseBlock.sv\
       $(CLUSTER_INTERCONNECT_IP)/AddressDecoder_Req.sv\
       $(CLUSTER_INTERCONNECT_IP)/XBAR_TCDM.sv\
       $(CLUSTER_INTERCONNECT_IP)/XBAR_TCDM_WRAPPER.sv\
       $(CLUSTER_INTERCONNECT_IP)/TCDM_PIPE_REQ.sv\
       $(CLUSTER_INTERCONNECT_IP)/TCDM_PIPE_RESP.sv\
       $(CLUSTER_INTERCONNECT_IP)/grant_mask.sv\
       $(CLUSTER_INTERCONNECT_IP)/priority_Flag_Req.sv\
       $(EVENT_UNIT_FLEX_IP)/event_unit_core.sv\
       $(EVENT_UNIT_FLEX_IP)/event_unit_interface_mux.sv\
       $(EVENT_UNIT_FLEX_IP)/event_unit_top.sv\
       $(EVENT_UNIT_FLEX_IP)/soc_periph_fifo.sv\
       $(EVENT_UNIT_FLEX_IP)/interc_sw_evt_trig.sv\
       $(EVENT_UNIT_FLEX_IP)/hw_barrier_unit.sv\
       $(EVENT_UNIT_FLEX_IP)/hw_mutex_unit.sv\
       $(EVENT_UNIT_FLEX_IP)/hw_dispatch.sv\
       $(MCHAN_IP)/misc/mchan_arbiter.sv\
       $(MCHAN_IP)/misc/mchan_arb_primitive.sv\
       $(MCHAN_IP)/misc/mchan_fifo.sv\
       $(MCHAN_IP)/misc/mchan_rr_flag_req.sv\
       $(MCHAN_IP)/ctrl_unit/address_decoder.sv\
       $(MCHAN_IP)/ctrl_unit/address_decoder_pe.sv\
       $(MCHAN_IP)/ctrl_unit/cmd_counter.sv\
       $(MCHAN_IP)/ctrl_unit/core_if.sv\
       $(MCHAN_IP)/ctrl_unit/core_if_pe.sv\
       $(MCHAN_IP)/ctrl_unit/ctrl_unit.sv\
       $(MCHAN_IP)/ctrl_unit/synch_unit.sv\
       $(MCHAN_IP)/ctrl_unit/trans_allocator.sv\
       $(MCHAN_IP)/ctrl_unit/trans_queue.sv\
       $(MCHAN_IP)/ctrl_unit/trans_arbiter_wrap.sv\
       $(MCHAN_IP)/ctrl_unit/trans_unpack.sv\
       $(MCHAN_IP)/ctrl_unit/twd_trans_queue.sv\
       $(MCHAN_IP)/ctrl_unit/twd_trans_splitter.sv\
       $(MCHAN_IP)/ext_unit/ext_ar_buffer.sv\
       $(MCHAN_IP)/ext_unit/ext_aw_buffer.sv\
       $(MCHAN_IP)/ext_unit/ext_b_buffer.sv\
       $(MCHAN_IP)/ext_unit/ext_buffer.sv\
       $(MCHAN_IP)/ext_unit/ext_opc_buf.sv\
       $(MCHAN_IP)/ext_unit/ext_r_buffer.sv\
       $(MCHAN_IP)/ext_unit/ext_rx_if.sv\
       $(MCHAN_IP)/ext_unit/ext_tid_gen.sv\
       $(MCHAN_IP)/ext_unit/ext_tx_if.sv\
       $(MCHAN_IP)/ext_unit/ext_unit.sv\
       $(MCHAN_IP)/ext_unit/ext_w_buffer.sv\
       $(MCHAN_IP)/tcdm_unit/tcdm_cmd_unpack.sv\
       $(MCHAN_IP)/tcdm_unit/tcdm_rx_if.sv\
       $(MCHAN_IP)/tcdm_unit/tcdm_synch.sv\
       $(MCHAN_IP)/tcdm_unit/tcdm_tx_if.sv\
       $(MCHAN_IP)/tcdm_unit/tcdm_unit.sv\
       $(MCHAN_IP)/trans_unit/trans_aligner.sv\
       $(MCHAN_IP)/trans_unit/trans_buffers.sv\
       $(MCHAN_IP)/trans_unit/trans_unit.sv\
       $(MCHAN_IP)/top/mchan.sv\
       $(ICACHE_INTC_IP)/DistributedArbitrationNetwork_Req_icache_intc.sv\
       $(ICACHE_INTC_IP)/DistributedArbitrationNetwork_Resp_icache_intc.sv\
       $(ICACHE_INTC_IP)/icache_intc.sv\
       $(ICACHE_INTC_IP)/Req_Arb_Node_icache_intc.sv\
       $(ICACHE_INTC_IP)/Resp_Arb_Node_icache_intc.sv\
       $(ICACHE_INTC_IP)/RoutingBlock_Req_icache_intc.sv\
       $(ICACHE_INTC_IP)/RoutingBlock_Resp_icache_intc.sv\
       $(ICACHE_INTC_IP)/lint_mux.sv\
       $(ICACHE_INTC_IP)/RoutingBlock_2ch_Req_icache_intc.sv\
       $(ICACHE_MP_128_PF_IP)/cache_controller_to_axi_128_PF.sv\
       $(ICACHE_MP_128_PF_IP)/central_controller_128.sv\
       $(ICACHE_MP_128_PF_IP)/icache_bank_mp_128.sv\
       $(ICACHE_MP_128_PF_IP)/icache_bank_mp_PF.sv\
       $(ICACHE_MP_128_PF_IP)/icache_top_mp_128_PF.sv\
       $(ICACHE_MP_128_PF_IP)/merge_refill_cam_128_16.sv\
       $(ICACHE_MP_128_PF_IP)/pf_miss_mux.sv\
       $(ICACHE_MP_128_PF_IP)/prefetcher_if.sv\
       $(CLUSTER_PERIPHERALS_IP)/cluster_control_unit/cluster_control_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/event_unit_arbiter.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/event_unit_input.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/event_unit_mux.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/event_unit_sm.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/event_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/HW_barrier_logic.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/HW_barrier.sv\
       $(CLUSTER_PERIPHERALS_IP)/event_unit/interrupt_mask.sv\
       $(CLUSTER_PERIPHERALS_IP)/icache_ctrl_unit/icache_ctrl_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/icache_ctrl_unit/new_icache_ctrl_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/icache_ctrl_unit/mp_icache_ctrl_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/icache_ctrl_unit/sp_icache_ctrl_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/icache_ctrl_unit/pri_icache_ctrl_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/icache_ctrl_unit/mp_pf_icache_ctrl_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/mmu_config_unit/mmu_config_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/perf_counters_unit/perf_counters_unit.sv\
       $(CLUSTER_PERIPHERALS_IP)/tcdm_pipe_unit/tcdm_pipe_unit.sv\
       $(PULP_CLUSTER_IP)/packages/pulp_cluster_package.sv\
       $(PULP_CLUSTER_IP)/packages/apu_package.sv\
       $(PULP_CLUSTER_IP)/rtl/core_region.sv\
       $(PULP_CLUSTER_IP)/rtl/core_demux.sv\
       $(PULP_CLUSTER_IP)/rtl/cluster_interconnect_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/tcdm_banks_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/periph_demux.sv\
       $(PULP_CLUSTER_IP)/rtl/per_demux_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/periph_FIFO.sv\
       $(PULP_CLUSTER_IP)/rtl/cluster_peripherals.sv\
       $(PULP_CLUSTER_IP)/rtl/cluster_clock_gate.sv\
       $(PULP_CLUSTER_IP)/rtl/cluster_timer_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/cluster_event_map.sv\
       $(PULP_CLUSTER_IP)/rtl/dmac_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/xne_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/cluster_bus_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/axi_slice_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/axi2mem_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/axi2per_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/per2axi_wrap.sv\
       $(PULP_CLUSTER_IP)/rtl/pulp_cluster.sv

TB_SRC=$(RTL_PATH)/tb/jtag_pkg.sv\
       $(RTL_PATH)/tb/dbg_pkg.sv\
       $(RTL_PATH)/tb/tb_clk_gen.sv\
       $(RTL_PATH)/tb/tb_fs_handler.sv\
       $(RTL_PATH)/tb/dev_dpi/dev_dpi.sv\
       $(RTL_PATH)/tb/tb_pulp.sv

VIP_SRC=$(RTL_PATH)/vip/spi_master_padframe.sv\
	$(RTL_PATH)/vip/uart_tb_rx.sv\
	$(RTL_PATH)/vip/camera/cam_vip.sv

PULP_SRC=$(RTL_PATH)/pulp/jtag_tap_top.sv\
         $(RTL_PATH)/pulp/pad_control.sv\
         $(RTL_PATH)/pulp/cluster_domain.sv\
         $(RTL_PATH)/pulp/safe_domain.sv\
         $(RTL_PATH)/pulp/soc_domain.sv\
         $(RTL_PATH)/pulp/rtc_date.sv\
         $(RTL_PATH)/pulp/rtc_clock.sv\
         $(RTL_PATH)/pulp/pad_frame.sv\
         $(RTL_PATH)/pulp/pulp.sv

VERILATOR = verilator
VDIR = obj_dir
CPPFLAGS = -I$(VDIR) `pkg-config --cflags verilator`
CXXFLAGS = -Wall -Werror -std=c++11
CXX = g++
LD = g++

# top module name

TOP = pulp_soc

VSRC=$(IP_SRC) $(TB_SRC) $(VIP_SRC) $(PULP_SRC)

VINC = +incdir+$(IPS_PATH)/riscv/include \
       +incdir+$(IPS_PATH)/mchan/include \
       +incdir+$(IPS_PATH)/cluster_peripherals/include \
       +incdir+$(IPS_PATH)/cluster_peripherals/event_unit/include \
       +incdir+$(IPS_PATH)/zero-riscy/include \
       +incdir+$(IPS_PATH)/adv_dbg_if/rtl \
       +incdir+$(IPS_PATH)/axi/axi_node \
       +incdir+$(RTL_PATH)/includes

VOBJS = $(VDIR)/verilated.o       \
        $(VDIR)/verilated_vcd_c.o

VLIB = $(VDIR)/V$(TOP)__ALL.a

VSMK = V$(TOP).mk
VMK  = $(VDIR)/$(VSMK)

# Build the library

all: clean $(VLIB)

$(VLIB): $(VMK)
	make -C $(VDIR) -f V$(TOP).mk

$(VDIR)/$(TOP): $(VDIR) $(VMK)
	$(MAKE) -C $(VDIR) -f $(VSMK)

$(VDIR):
	mkdir -p $@

$(VMK): $(VSRC)
	verilator -O3 -CFLAGS "-O3 -g3 -std=gnu++11" \
                  --top-module top --Mdir $(VDIR) --trace -cc \
	          --Wno-REDEFMACRO -Wno-STMTDLY \
	          $(VINC) $(VSRC)

.PHONY: clean
clean:
	$(RM) -r $(VDIR)
