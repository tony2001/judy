judy1_macros = J1T.3 \
	    J1S.3 \
	    J1U.3 \
	    J1F.3 \
	    J1N.3 \
	    J1L.3 \
	    J1P.3 \
	    J1FE.3 \
	    J1NE.3 \
	    J1LE.3 \
	    J1PE.3 \
	    J1C.3 \
	    J1BC.3 \
	    J1FA.3 \
	    J1MU.3

judyl_macros = JLG.3 \
	    JLI.3 \
	    JLD.3 \
	    JLF.3 \
	    JLN.3 \
	    JLL.3 \
	    JLP.3 \
	    JLFE.3 \
	    JLNE.3 \
	    JLLE.3 \
	    JLPE.3 \
	    JLC.3 \
	    JLBC.3 \
	    JLFA.3 \
	    JLMU.3

judysl_macros = JSLG.3 \
	    JSLI.3 \
	    JSLD.3 \
	    JSLF.3 \
	    JSLN.3 \
	    JSLL.3 \
	    JSLP.3 \
	    JSLFA.3

judyhs_macros = JHSG.3 \
	    JHSI.3 \
	    JHSD.3 \
	    JHSFA.3

judy1_funcs = Judy1Test.3 \
	    Judy1Set.3 \
	    Judy1Unset.3 \
	    Judy1First.3 \
	    Judy1Next.3 \
	    Judy1Last.3 \
	    Judy1Prev.3 \
	    Judy1FirstEmpty.3 \
	    Judy1NextEmpty.3 \
	    Judy1LastEmpty.3 \
	    Judy1PrevEmpty.3 \
	    Judy1Count.3 \
	    Judy1ByCount.3 \
	    Judy1FreeArray.3 \
	    Judy1MemUsed.3

judyl_funcs = JudyLGet.3 \
	    JudyLIns.3 \
	    JudyLDel.3 \
	    JudyLFirst.3 \
	    JudyLNext.3 \
	    JudyLLast.3 \
	    JudyLPrev.3 \
	    JudyLFirstEmpty.3 \
	    JudyLNextEmpty.3 \
	    JudyLLastEmpty.3 \
	    JudyLPrevEmpty.3 \
	    JudyLCount.3 \
	    JudyLByCount.3 \
	    JudyLFreeArray.3 \
	    JudyLMemUsed.3

judysl_funcs = JudySLGet.3 \
	    JudySLIns.3 \
	    JudySLDel.3 \
	    JudySLFirst.3 \
	    JudySLNext.3 \
	    JudySLLast.3 \
	    JudySLPrev.3 \
	    JudySLFreeArray.3

judyhs_funcs = JudyHSGet.3 \
	    JudyHSIns.3 \
	    JudyHSDel.3 \
	    JudyHSFreeArray.3

judy_mans = Judy.3 \
	    Judy1.3 \
	    Judy1_funcs.3 \
	    JudyL.3 \
	    JudyL_funcs.3 \
	    JudySL.3 \
	    JudySL_funcs.3 \
	    JudyHS.3 \
	    JudyHS_funcs.3

man3_MANS = $(judy_mans) \
			$(judy1_macros) $(judy1_funcs) \
			$(judyl_macros) $(judyl_funcs) \
			$(judysl_macros) $(judysl_funcs) \
			$(judyhs_macros) $(judyhs_funcs)


$(judy_mans):
	../tool/jhton $(top_srcdir)/doc/ext/`echo -n $@ | sed -e 's/\.3/_3/'`.htm | grep -v '^[   ]*$$' | sed -e 's/\.C//' > $@

$(judy1_macros): Judy1.3
	 echo ".so man3/Judy1.3" > $@

$(judy1_funcs): Judy1_funcs.3
	 echo ".so man3/Judy1_funcs.3" > $@

$(judyl_macros): JudyL.3
	 echo ".so man3/JudyL.3" > $@

$(judyl_funcs): JudyL_funcs.3
	 echo ".so man3/JudyL_funcs.3" > $@

$(judysl_macros): JudySL.3
	 echo ".so man3/JudySL.3" > $@

$(judysl_funcs): JudySL_funcs.3
	 echo ".so man3/JudySL_funcs.3" > $@

$(judyhs_macros): JudyHS.3
	 echo ".so man3/JudyHS.3" > $@

$(judyhs_funcs): JudyHS_funcs.3
	 echo ".so man3/JudyHS_funcs.3" > $@

CLEANFILES = $(man3_MANS)
