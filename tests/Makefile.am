## -*- makefile -*-

TESTS_ENVIRONMENT=	\
	GERBV=${GERBV} \
	IM_ANIMATE=${IM_ANIMATE} \
	IM_COMPARE=${IM_COMPARE} \
	IM_COMPOSITE=${IM_COMPOSITE} \
	IM_CONVERT=${IM_CONVERT} \
	IM_DISPLAY=${IM_DISPLAY} \
	IM_MONTAGE=${IM_MONTAGE} \
	XHOST=${XHOST}

RUN_TESTS=	run_tests.sh

check_SCRIPTS=		${RUN_TESTS}

# if we have the required tools, then run the regression test
if HAVE_TEST_TOOLS
  TESTS = ${RUN_TESTS}
else
  TESTS = missing_test
endif

# Instead of recursing into each of the many subdirectories, simply define
# the relevant files here in one place. This is considerably faster and makes
# changes to top level configure.ac unnecessary when adding new tests.
EXTRA_DIST = \
  ${RUN_TESTS} \
  tests.list \
  README.txt \
  inputs/bom.attrs \
  inputs/bom_attribs.pcb \
  inputs/bom_general.pcb \
  inputs/buried.pcb \
  inputs/changeclearsize-sel.script \
  inputs/circles.pcb \
  inputs/clearance.pcb \
  inputs/default.pcb \
  inputs/fileversion.script \
  inputs/drctest-clearance-arcs-arcs.pcb \
  inputs/drctest-clearance-arcs-buriedvias.pcb \
  inputs/drctest-clearance-arcs-lines.pcb \
  inputs/drctest-clearance-arcs-pads.pcb \
  inputs/drctest-clearance-arcs-vias.pcb \
  inputs/drctest-clearance-lines-arcs.pcb \
  inputs/drctest-clearance-lines-buriedvias.pcb \
  inputs/drctest-clearance-lines-lines.pcb \
  inputs/drctest-clearance-lines-pads.pcb \
  inputs/drctest-clearance-lines-vias.pcb \
  inputs/drctest-clearance-misc.pcb \
  inputs/drctest-clearance-pads-arcs.pcb \
  inputs/drctest-clearance-pads-buriedvias.pcb \
  inputs/drctest-clearance-pads-lines.pcb \
  inputs/drctest-clearance-pads-pads.pcb \
  inputs/drctest-clearance-pads-vias.pcb \
  inputs/drctest-clearance-vias-arcs.pcb \
  inputs/drctest-clearance-vias-buriedvias.pcb \
  inputs/drctest-clearance-vias-lines.pcb \
  inputs/drctest-clearance-vias-vias.pcb \
  inputs/drctest-minsize-arcs.pcb \
  inputs/drctest-minsize-lines.pcb \
  inputs/drctest-minsize-pads.pcb \
  inputs/drctest-minsize-pins.pcb \
  inputs/drctest-minsize-polygons.pcb \
  inputs/drctest-minsize-vias.pcb \
  inputs/drctest-polygonclearance-arcs.pcb \
  inputs/drctest-polygonclearance-lines.pcb \
  inputs/drctest-polygonclearance-misc.pcb \
  inputs/drctest-polygonclearance-pads.pcb \
  inputs/drctest-polygonclearance-pins.pcb \
  inputs/drctest-polygonclearance-vias.pcb \
  inputs/drctest.script \
  inputs/fileversion-20091103.pcb \
  inputs/fileversion-20100606.pcb \
  inputs/fileversion-20170218.pcb \
  inputs/fileversion.script \
  inputs/gcode_oneline.pcb \
  inputs/gerber_arcs.pcb \
  inputs/gerber_oneline.pcb \
  inputs/gsvit_board.pcb \
  inputs/ipcd356_board.pcb \
  inputs/ipcd356_cust0.pcb \
  inputs/ipcd356_cust1.pcb \
  inputs/ipcd356_via_1.pcb \
  inputs/ipcd356_via_2.pcb \
  inputs/ipcd356_via_3.pcb \
  inputs/ipcd356_via_4.pcb \
  inputs/ipcd356_via_5.pcb \
  inputs/ipcd356_via_6.pcb \
  inputs/ipcd356_via_7.pcb \
  inputs/ipcd356_via_8.pcb \
  inputs/ipcd356_hole_1.pcb \
  inputs/ipcd356_hole_2.pcb \
  inputs/ipcd356_smt_1.pcb \
  inputs/ipcd356_smt_2.pcb \
  inputs/ipcd356_smt_3.pcb \
  inputs/minmaskgap.pcb \
  inputs/minmaskgap.script \
  inputs/nelma_board.pcb \
  inputs/only_visible.pcb \
  inputs/routestyles.script \
  inputs/screen_layer_order.pcb \
  golden/ChangeClearSize-Sel/clearance-min.pcb \
  golden/ChangeClearSize-Sel/clearance-non-zero.pcb \
  golden/ChangeClearSize-Sel/clearance-zero.pcb \
  golden/Clearance/clearance.bottom.gbr \
  golden/Clearance/clearance.bottommask.gbr \
  golden/Clearance/clearance.fab.gbr \
  golden/Clearance/clearance.group1.gbr \
  golden/Clearance/clearance.group2.gbr \
  golden/Clearance/clearance.group3.gbr \
  golden/Clearance/clearance.plated-drill_01-03.cnc \
  golden/Clearance/clearance.plated-drill_02-04.cnc \
  golden/Clearance/clearance.plated-drill_03-05.cnc \
  golden/Clearance/clearance.plated-drill.cnc \
  golden/Clearance/clearance.top.gbr \
  golden/Clearance/clearance.topmask.gbr \
  golden/Clearance/clearance.toppaste.gbr \
  golden/Clearance/clearance.topsilk.gbr \
  golden/drc-clearance-arcs-arcs/drcreport.txt \
  golden/drc-clearance-arcs-buriedvias/drcreport.txt \
  golden/drc-clearance-arcs-lines/drcreport.txt \
  golden/drc-clearance-arcs-pads/drcreport.txt \
  golden/drc-clearance-arcs-vias/drcreport.txt \
  golden/drc-clearance-lines-arcs/drcreport.txt \
  golden/drc-clearance-lines-buriedvias/drcreport.txt \
  golden/drc-clearance-lines-lines/drcreport.txt \
  golden/drc-clearance-lines-pads/drcreport.txt \
  golden/drc-clearance-lines-vias/drcreport.txt \
  golden/drc-clearance-misc/drcreport.txt \
  golden/drc-clearance-pads-arcs/drcreport.txt \
  golden/drc-clearance-pads-buriedvias/drcreport.txt \
  golden/drc-clearance-pads-lines/drcreport.txt \
  golden/drc-clearance-pads-pads/drcreport.txt \
  golden/drc-clearance-pads-vias/drcreport.txt \
  golden/drc-clearance-vias-arcs/drcreport.txt \
  golden/drc-clearance-vias-buriedvias/drcreport.txt \
  golden/drc-clearance-vias-lines/drcreport.txt \
  golden/drc-clearance-vias-vias/drcreport.txt \
  golden/drc-minsize-arcs/drcreport.txt \
  golden/drc-minsize-lines/drcreport.txt \
  golden/drc-minsize-pads/drcreport.txt \
  golden/drc-minsize-pins/drcreport.txt \
  golden/drc-minsize-polygons/drcreport.txt \
  golden/drc-minsize-vias/drcreport.txt \
  golden/drc-polygonclearance-arcs/drcreport.txt \
  golden/drc-polygonclearance-lines/drcreport.txt \
  golden/drc-polygonclearance-misc/drcreport.txt \
  golden/drc-polygonclearance-pads/drcreport.txt \
  golden/drc-polygonclearance-pins/drcreport.txt \
  golden/drc-polygonclearance-vias/drcreport.txt \
  golden/FileVersions/fileversion-20091103-out.pcb \
  golden/FileVersions/fileversion-20100606-out.pcb \
  golden/FileVersions/fileversion-20170218-out.pcb \
  golden/hid_bom1/bom_general.bom \
  golden/hid_bom1/bom_general.xy \
  golden/hid_bom2/test.bom \
  golden/hid_bom2/bom_general.xy \
  golden/hid_bom3/mm.xy \
  golden/hid_bom4/inches.xy \
  golden/hid_bom5/mil.xy \
  golden/hid_bom6/dmil.xy \
  golden/hid_bom7/cmil.xy \
  golden/hid_bom8/cm.xy \
  golden/hid_bom9/um.xy \
  golden/hid_bom10/bom_attribs.bom \
  golden/hid_gerber1/gerber_oneline.top.gbr \
  golden/hid_gerber1/gerber_oneline.fab.gbr \
  golden/hid_gerber1/gerber_oneline.bottom.gbr \
  golden/hid_gerber1/gerber_oneline.plated-drill.cnc \
  golden/hid_gerber2/out.fab.gbr \
  golden/hid_gerber2/out.top.gbr \
  golden/hid_gerber2/out.bottom.gbr \
  golden/hid_gerber2/out.plated-drill.cnc \
  golden/hid_gerber3/arcs.group1.gbr \
  golden/hid_gerber3/arcs.top.gbr \
  golden/hid_gerber3/arcs.group4.gbr \
  golden/hid_gerber3/arcs.fab.gbr \
  golden/hid_gerber3/arcs.bottom.gbr \
  golden/hid_gerber3/arcs.plated-drill.cnc \
  golden/hid_gerber4/buried.bottom.gbr \
  golden/hid_gerber4/buried.fab.gbr \
  golden/hid_gerber4/buried.group2.gbr \
  golden/hid_gerber4/buried.group4.gbr \
  golden/hid_gerber4/buried.group7.gbr \
  golden/hid_gerber4/buried.plated-drill.cnc \
  golden/hid_gerber4/buried.plated-drill_03-08.cnc \
  golden/hid_gerber4/buried.top.gbr \
  golden/hid_gcode1/gcode_oneline-bottom.gcode \
  golden/hid_gcode1/gcode_oneline-top.gcode \
  golden/hid_gcode1/gcode_oneline-outline.gcode \
  golden/hid_gcode1/gcode_oneline-0.8890.drill.gcode \
  golden/hid_gcode2/out-bottom.gcode \
  golden/hid_gcode2/out-top.gcode \
  golden/hid_gcode2/out-outline.gcode \
  golden/hid_gcode2/out-0.8890.drill.gcode \
  golden/hid_gcode3/gcode_oneline-bottom.gcode \
  golden/hid_gcode3/gcode_oneline-top.gcode \
  golden/hid_gcode3/gcode_oneline-outline.gcode \
  golden/hid_gcode3/gcode_oneline-0.8890.drill.gcode \
  golden/hid_gcode4/gcode_oneline-bottom.gcode \
  golden/hid_gcode4/gcode_oneline-top.gcode \
  golden/hid_gcode4/gcode_oneline-outline.gcode \
  golden/hid_gcode4/gcode_oneline-0.8890.drill.gcode \
  golden/hid_gcode5/gcode_oneline-bottom.gcode \
  golden/hid_gcode5/gcode_oneline-top.gcode \
  golden/hid_gcode5/gcode_oneline-outline.gcode \
  golden/hid_gcode5/gcode_oneline-0.8890.drill.gcode \
  golden/hid_gcode6/gcode_oneline-bottom.gcode \
  golden/hid_gcode6/gcode_oneline-top.gcode \
  golden/hid_gcode6/gcode_oneline-outline.gcode \
  golden/hid_gcode6/gcode_oneline-0.8890.drill.gcode \
  golden/hid_gcode7/gcode_oneline-bottom.gcode \
  golden/hid_gcode7/gcode_oneline-top.gcode \
  golden/hid_gcode7/gcode_oneline-outline.gcode \
  golden/hid_gcode7/gcode_oneline-0.8890.drill.gcode \
  golden/hid_gcode8/gcode_oneline-bottom.gcode \
  golden/hid_gcode8/gcode_oneline-top.gcode \
  golden/hid_gcode8/gcode_oneline-outline.gcode \
  golden/hid_gcode8/gcode_oneline-0.8890.drill.gcode \
  golden/hid_gcode9/gcode_oneline-bottom.gcode \
  golden/hid_gcode9/gcode_oneline-top.gcode \
  golden/hid_gcode9/gcode_oneline-outline.gcode \
  golden/hid_gcode9/gcode_oneline-drillmill.gcode \
  golden/hid_gcode10/gcode_oneline-bottom.gcode \
  golden/hid_gcode10/gcode_oneline-top.gcode \
  golden/hid_gcode10/gcode_oneline-outline.gcode \
  golden/hid_gcode10/gcode_oneline-drillmill.gcode \
  golden/hid_gcode11/gcode_oneline-bottom.gcode \
  golden/hid_gcode11/gcode_oneline-top.gcode \
  golden/hid_gcode11/gcode_oneline-outline.gcode \
  golden/hid_gcode11/gcode_oneline-0.0350.drill.gcode \
  golden/hid_gsvit1/gsvit_board.top.png \
  golden/hid_ipcd3561/ipcd356_board.net \
  golden/hid_ipcd3562/ipcd356_cust0.net \
  golden/hid_ipcd3563/ipcd356_cust1.net \
  golden/hid_ipcd3564/ipcd356_via_1.net \
  golden/hid_ipcd3565/ipcd356_via_2.net \
  golden/hid_ipcd3566/ipcd356_via_3.net \
  golden/hid_ipcd3567/ipcd356_via_4.net \
  golden/hid_ipcd3568/ipcd356_via_5.net \
  golden/hid_ipcd3569/ipcd356_via_6.net \
  golden/hid_ipcd35610/ipcd356_via_7.net \
  golden/hid_ipcd35611/ipcd356_via_8.net \
  golden/hid_ipcd35612/ipcd356_hole_1.net \
  golden/hid_ipcd35613/ipcd356_hole_2.net \
  golden/hid_ipcd35614/ipcd356_smt_1.net \
  golden/hid_ipcd35615/ipcd356_smt_2.net \
  golden/hid_ipcd35616/ipcd356_smt_3.net \
  golden/hid_nelma1/nelma_board.top.png \
  golden/hid_png1/gerber_oneline.png \
  golden/hid_png2/myfile.png \
  golden/hid_png3/gerber_oneline.png \
  golden/hid_png4/gerber_oneline.png \
  golden/hid_png5/screen_layer_order.png \
  golden/hid_png6/only_visible.png \
  golden/hid_png7/gerber_oneline.png \
  golden/hid_png8/gerber_oneline.png \
  golden/hid_png9/gsvit_board.png \
  golden/hid_png101/gerber_oneline.gif \
  golden/hid_png102/myfile.gif \
  golden/hid_png103/gerber_oneline.gif \
  golden/hid_png104/gerber_oneline.gif \
  golden/hid_png105/screen_layer_order.gif \
  golden/hid_png106/only_visible.gif \
  golden/hid_png107/gerber_oneline.gif \
  golden/hid_png108/gerber_oneline.gif \
  golden/hid_png109/gsvit_board.gif \
  golden/hid_png201/gerber_oneline.jpg \
  golden/hid_png202/myfile.jpg \
  golden/hid_png203/gerber_oneline.jpg \
  golden/hid_png204/gerber_oneline.jpg \
  golden/hid_png205/screen_layer_order.jpg \
  golden/hid_png206/only_visible.jpg \
  golden/hid_png207/gerber_oneline.jpg \
  golden/hid_png208/gerber_oneline.jpg \
  golden/hid_png209/gsvit_board.jpg \
  golden/hid_ps1/circles.ps \
  golden/hid_ps2/buried.ps \
  golden/MinMaskGap/minmaskgap.pcb \
  golden/RouteStyles/mixed-apertures-load.pcb \
  golden/RouteStyles/mixed-apertures-save.pcb \
  golden/RouteStyles/non-zero-apertures-save.pcb \
  golden/RouteStyles/zero-apertures-load.pcb \
  golden/RouteStyles/zero-apertures-save.pcb

.PHONY: missing_test
missing_test:
	@echo "Test environment was found to be incomplete at configuration time,"
	@echo "can't run regression tests. Check configure output to find out which"
	@echo "tools are missing."
	@false

# these are created by 'make check'
clean-local:
	rm -rf outputs
